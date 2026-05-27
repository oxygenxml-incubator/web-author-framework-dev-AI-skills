# Integrating SQF into a Framework

How to ship a Schematron Quick Fix as part of an oXygen framework so authors see the fix automatically — without each user configuring validation.

Full references (read via `oxygen-docs`):

- [Integrating SQF in a Framework and Sharing Them](https://www.oxygenxml.com/doc/ug-editor/topics/sqf-implementing-framework.html) — canonical end-to-end recipe (Desktop dialog flow).
- [Validating Schematron Quick Fixes](https://www.oxygenxml.com/doc/ug-editor/topics/validating-sqf.html)
- [Configuring Validation Scenarios for a Framework](https://www.oxygenxml.com/doc/ug-editor/topics/dg-validation-scenarios.html)
- [Associating a Schema in Validation Scenarios](https://www.oxygenxml.com/doc/ug-editor/topics/associate-schema-framework-validation.html)
- [Sharing a Framework](https://www.oxygenxml.com/doc/ug-editor/topics/author-document-type-extension-sharing.html)

Related local refs: `ai-framework-developer` → `exf-structure.md` (`.exf` shape) and `validation-scenarios-export.md` (`.scenarios` format).

## Two routes — pick one

| Route | When | Pros | Cons |
|---|---|---|---|
| **A. Validation scenario** — `.exf` `<validationScenarios><addScenarios href=…/>` pointing at a `.scenarios` file that references the `.sch`. | Production. Extension over an existing doctype (DITA, DocBook, TEI). | Mirrors the Desktop dialog 1:1. Survives kit upgrades. | Two extra files. |
| **B. Default schema** — `.exf` `<defaultSchema schemaType="sch" href=…/>` pointing directly at the `.sch`. | Standalone framework where the `.sch` *is* the only schema. | One file. | Replaces the framework's default schema entirely — wrong choice for an extension. |

In practice **Route A** for SQF extensions over an existing framework, **Route B** for standalone frameworks built around a `.sch`.

## Schema-detection order (why a fix sometimes doesn't fire)

Per [Associating a Schema to XML Documents](https://www.oxygenxml.com/doc/ug-editor/topics/associate-schema-to-document.html), oXygen picks the schema(s) for validation in this order:

1. Validation scenario **associated with the current document** (per-document attachment).
2. Validation scenario **specified as default** in the framework (document-type config).
3. Schema **associated directly in the document** (`<?xml-model?>` PI, `xsi:schemaLocation`, `DOCTYPE`).
4. Schema declared in the framework's **Schema tab**.

Practical consequence: if you ship SQF via Route A but the user opens a document that has its own per-document validation scenario attached, **your fix won't fire** — stage 1 short-circuits before stage 2 runs. To diagnose: open the doc, check the validation panel header for the actual running scenario, confirm it matches the one your `.exf` set as default.

## Route A — validation scenario (recommended)

### Layout under the kit

```
<EXPANDED_WEBAPP_DIR>/user-frameworks/dita-sqf/
├── dita-sqf.exf
├── rules/
│   └── custom-rules.sch
└── scenarios/
    └── dita-sqf-validation.scenarios
```

### Step 1 — write the `.sch`

```xml
<?xml version="1.0" encoding="UTF-8"?>
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron"
            xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
            queryBinding="xslt2">
  <sch:pattern>
    <sch:rule context="section">
      <sch:assert test="@id" sqf:fix="addId">Every section needs an @id.</sch:assert>
      <sqf:fix id="addId">
        <sqf:description>
          <sqf:title>Add @id to the current section</sqf:title>
        </sqf:description>
        <sqf:add target="id" node-type="attribute" select="generate-id()"/>
      </sqf:fix>
    </sch:rule>
  </sch:pattern>
</sch:schema>
```

Before wiring, **validate the `.sch` itself** by opening it in oXygen and running validation against the built-in SQF schema (catches missing `@target`, undeclared namespaces, unparseable XPath). See `validating-sqf.md`.

### Step 2 — write the `.scenarios` export

The `.scenarios` file is Java XML serialization — full reference: `validation-scenarios-export.md` in `ai-framework-developer`. A framework-level `.scenarios` is a **recipe**: each `<validationUnit>` says "validate the currently-edited document (`${currentFileURL}`) with engine X and (optionally) schema Y", resolved against whatever doc is open under the framework.

Minimal `dita-sqf-validation.scenarios` — **verified to load in WA 29.0** — running DITA validation **plus** the SQF-enabled `.sch`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<serialized xml:space="preserve">
  <serializableOrderedMap>
    <entry>
      <String>validation.scenarios</String>
      <validationScenario-array>
        <validationScenario>
          <field name="pairs">
            <list>
              <validationUnit>
                <field name="validationType">
                  <validationUnitType>
                    <field name="validationInputType"><String>text/xml</String></field>
                  </validationUnitType>
                </field>
                <field name="url"><String>${currentFileURL}</String></field>
                <field name="validationEngine">
                  <validationEngine>
                    <field name="engineType"><String>DITA Validation</String></field>
                    <field name="allowsAutomaticValidation"><Boolean>true</Boolean></field>
                  </validationEngine>
                </field>
                <field name="allowAutomaticValidation"><Boolean>true</Boolean></field>
                <field name="extensions"><null/></field>
                <field name="validationSchema"><null/></field>
              </validationUnit>
              <validationUnit>
                <field name="validationType">
                  <validationUnitType>
                    <field name="validationInputType"><String>text/xml</String></field>
                  </validationUnitType>
                </field>
                <field name="url"><String>${currentFileURL}</String></field>
                <field name="validationEngine">
                  <validationEngine>
                    <field name="engineType"><String>&lt;Default engine></String></field>
                    <field name="allowsAutomaticValidation"><Boolean>true</Boolean></field>
                  </validationEngine>
                </field>
                <field name="allowAutomaticValidation"><Boolean>true</Boolean></field>
                <field name="extensions"><null/></field>
                <field name="validationSchema">
                  <validationUnitSchema>
                    <field name="type"><Integer>7</Integer></field>
                    <field name="uri"><String>${framework}/rules/custom-rules.sch</String></field>
                  </validationUnitSchema>
                </field>
              </validationUnit>
            </list>
          </field>
          <field name="type"><String>Validation_scenario</String></field>
          <field name="name"><String>DITA + Custom SQF</String></field>
        </validationScenario>
      </validationScenario-array>
    </entry>
  </serializableOrderedMap>
</serialized>
```

WA-specific notes (mirroring bundled `frameworks/dita/lw/resources/dita-lw-validation.scenarios`):

- Two units: `DITA Validation` (bundled structure check) + `<Default engine>` with a `<validationSchema>` pointing at the `.sch` (Schematron / SQF). Drop the first unit for Schematron-only.
- The schema reference **must** live inside `<field name="validationSchema">` as a `<validationUnitSchema>` with `<field name="type"><Integer>N</Integer></field>` + `<field name="uri">${framework}/...</field>`. The older flat form (top-level `<field name="schemaURL">`, `<field name="useDocumentSchema">`) is **silently rejected by current Web Author** — `oxygen.log` prints `Invalid field : … cannot be found` and `Skip invalid object` right after `Loading user uploaded frameworks`, and the scenario never registers. Grep those WARN lines to diagnose.
- `<field name="type">` values come from `ro.sync.exml.workspace.api.editor.SchemaTypes`: `1` DTD, `2` XSD, `3` RNC, `4` RNG, `5` XSD+Sch, `6` RNG+Sch, **`7` Schematron**, `9` NVDL, `10` JSON, `11` JSON Schema.
- `${framework}` resolves to the `.exf` directory at load time; `${currentFileURL}` to the doc being validated.
- Cleanest way to obtain a correct `.scenarios` is **Desktop oXygen → configure scenario → export**. Copy-and-modify from a bundled `.scenarios` (e.g. `lw/resources/dita-lw-validation.scenarios`) whenever possible — the format is undocumented.

### Step 3 — write the `.exf`

```xml
<?xml version="1.0" encoding="UTF-8"?>
<script
  xmlns="http://www.oxygenxml.com/ns/framework/extend"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://www.oxygenxml.com/ns/framework/extend
                      http://www.oxygenxml.com/ns/framework/extend/frameworkExtensionScript.xsd"
  base="DITA">
  <name>DITA with custom SQF</name>
  <description>DITA framework extended with custom Schematron Quick Fixes.</description>
  <priority>High</priority>

  <validationScenarios>
    <addScenarios href="scenarios/dita-sqf-validation.scenarios"/>
    <defaultScenarios>
      <name>DITA + Custom SQF</name>
    </defaultScenarios>
  </validationScenarios>
</script>
```

- `@base="DITA"` ties the extension to the bundled DITA framework (use the right base name for the target — see `exf-structure.md`).
- `<priority>High</priority>` makes the extension win over the bundled framework when both match. Recommended for AI-generated extensions.
- `<addScenarios>` registers the scenario(s); `href` is resolved relative to the `.exf`.
- `<defaultScenarios>` flips the new scenario to default so opening a DITA doc runs it without the user picking from a menu. Omit to make it opt-in.
- For real cleanup, also use `<removeScenario name="DITA"/>` to remove the bundled default if your scenario replaces it (see `extend-dita-with-css-and-classpath.exf` in `samples/`).

### Step 4 — restart the kit

`user-frameworks/` is scanned **only at startup**. Full stop + start is mandatory — follow the Web Author restart procedure in the `ai-framework-developer` skill. After restart, tail `tomcat/logs/oxygen.log` for:

```
INFO  [ main ] [ ] ro.sync.servlet.StartupServlet - Loading user uploaded frameworks from: …
```

and confirm your framework name appears in subsequent log lines.

### Step 5 — verify

Open a DITA doc that violates the rule (e.g. `<section>` with no `@id`). Expect a validation warning, a Quick Fix proposal whose title matches your `<sqf:title>`, and the warning clearing after the proposal applies.

For Web Author, use `chrome-mcp-usage.md` in the `ai-framework-developer` skill to screenshot the proposal popup. **Web Author SQF parity with Desktop is not documented one-for-one** — if the fix doesn't surface in WA but works in Desktop, that's a real gap, not a config error; report it with the screenshot and the `.sch` snippet.

## Route B — default schema

For a standalone framework whose primary schema **is** the `.sch`:

```xml
<script
  xmlns="http://www.oxygenxml.com/ns/framework/extend"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://www.oxygenxml.com/ns/framework/extend
                      http://www.oxygenxml.com/ns/framework/extend/frameworkExtensionScript.xsd">
  <name>My Schematron Framework</name>
  <description>Custom framework validated by a Schematron with SQF.</description>
  <priority>High</priority>
  <associationRules inherit="none">
    <addRule rootElementLocalName="my-root" namespace="http://example.org/my-ns"/>
  </associationRules>
  <defaultSchema schemaType="sch" href="${framework}/rules/custom-rules.sch"/>
</script>
```

- `@schemaType="sch"` per `exf-structure.md`. Combined types `xmlschema_sch` / `rng_sch` apply when SQF lives next to a structural XSD/RNG.
- Does **not** combine with `base="…"` — replaces the framework's default schema entirely. For extending DITA, use Route A.

## Common failure modes

| Symptom | Cause | Fix |
|---|---|---|
| Framework not visible after restart | `user-frameworks/<dir>` at wrong path | Move under `<EXPANDED_WEBAPP_DIR>/user-frameworks/`. See `ai-framework-developer/SKILL.md`. |
| Validation runs but no fix proposal | Missing `xmlns:sqf`, missing `queryBinding="xslt2"`, or `.sch` not attached to the active scenario | Re-validate `.sch`; check the `.scenarios` href and that `<defaultScenarios>` name matches. |
| Fix appears but doesn't run | Missing `@target` for non-comment operation, `@match` selects an empty sequence | Re-read `sqf-operations-reference.md`; run in Desktop with the SQF debug view. |
| Fix runs but indent is wrong | Auto-indent kicked in | Add `@xml:space="preserve"` or move whitespace into `<xsl:text>`. |
| `oxygen.log` reports `ExtensionStructureException` on `.exf` load | `.exf` fails XSD or Schematron validation | Validate `.exf` against `frameworkExtensionScript.xsd` + `frameworkExtensionScript.sch`. See `exf-structure.md`. |
| `.scenarios` file silently ignored | `<addScenarios href>` resolves to a missing path; `<defaultScenarios>` name doesn't match the `name` inside the `.scenarios` | Read `oxygen.log` for warning lines; rename or re-export. |

## Sharing the extension

Once verified, `user-frameworks/<dir>/` is what gets shared. Options per [Sharing a Framework](https://www.oxygenxml.com/doc/ug-editor/topics/author-document-type-extension-sharing.html):

- **Zip and distribute** — recipients drop the folder into their own `user-frameworks/`.
- **Promote to an add-on** — package per [Packing and Deploying Add-ons](https://www.oxygenxml.com/doc/ug-editor/topics/packing-and-deploying-addons.html).
- **Promote to a built-in framework** — copy into `frameworks/` (curated kits only).

In all cases the `.sch` travels with the framework directory, so SQF availability stays consistent across machines.
