# Embedding SQF in RELAX NG or XML Schema

When the framework's primary schema is **XSD** or **RNG**, you can ship SQF inside the schema itself instead of a separate `.sch`. oXygen extracts the embedded rules when the document is validated against that schema **and** the validation scenario opts in via **Embedded Schematron rules**.

Full references (read via `oxygen-docs`):

- [Embedding SQF in Relax NG or XML Schema](https://www.oxygenxml.com/doc/ug-editor/topics/embed-sqf-in-rng-xsd.md)
- [Embedding Schematron Rules in XML Schema or RELAX NG](https://www.oxygenxml.com/doc/ug-editor/topics/combined_RNG_and_SCH.md) — broader page; covers RNG compact / annotation form.

## When to embed vs. ship a standalone `.sch`

| Embed in XSD / RNG | Standalone `.sch` |
|---|---|
| Grammar + rules ship as one artifact. | Rules shared across multiple frameworks. |
| Rules are part of the schema's contract. | Rules evolve faster than the structural schema. |
| One validation pass for grammar + rules. | Same rules combined with multiple grammars. |

The `<sqf:fix>` body is identical either way; only the wrapping differs.

## Required validation toggle

Embedded SQF is **not surfaced** unless the validation scenario opts in. In the scenario's validation unit, set **Schema type** = `XML Schema` or `Relax NG` and tick **Embedded Schematron rules**. **This is per-validation-unit and is not enabled by default** — first thing to check when embedded rules don't appear. See [validating XML against a schema](https://www.oxygenxml.com/doc/ug-editor/topics/validating-XML-documents-against-schema.md).

## XSD — inside `<xsd:annotation><xsd:appinfo>`

```xml
<xsd:annotation>
  <xsd:appinfo>
    <sch:pattern xmlns:sch="http://purl.oclc.org/dsdl/schematron"
                 xmlns:sqf="http://www.schematron-quickfix.com/validator/process">
      <sch:rule context="...">
        <sch:assert test="..." sqf:fix="fixId">Message.</sch:assert>
        <sqf:fix id="fixId">
          <sqf:description>
            <sqf:title>Fix title</sqf:title>
          </sqf:description>
          <!-- sqf:add | sqf:delete | sqf:replace | sqf:stringReplace -->
        </sqf:fix>
      </sch:rule>
    </sch:pattern>
  </xsd:appinfo>
</xsd:annotation>
```

`sch:` / `sqf:` declarations can live on `<xsd:schema>` (cleaner) or each `<sch:pattern>`. Multiple `<sch:pattern>` blocks are allowed in one `<xsd:appinfo>`.

## RNG (XML syntax) — at the grammar's top level

```xml
<grammar xmlns="http://relaxng.org/ns/structure/1.0"
         xmlns:sch="http://purl.oclc.org/dsdl/schematron"
         xmlns:sqf="http://www.schematron-quickfix.com/validator/process">
  <sch:pattern>
    <sch:rule context="...">
      <sch:assert test="..." sqf:fix="fixId">Message.</sch:assert>
      <sqf:fix id="fixId">
        <sqf:description>
          <sqf:title>Fix title</sqf:title>
        </sqf:description>
        <!-- operations -->
      </sqf:fix>
    </sch:rule>
  </sch:pattern>
  <start>
    <!-- ... -->
  </start>
</grammar>
```

For RNG **compact** syntax, see `combined_RNG_and_SCH.md` — it documents the annotation form for inline embedding.

## Local samples

`embed-sqf-in-rng-xsd.md` points at `$OXYGEN_INSTALL_DIR/samples/schematron` for end-to-end examples. In a Web Author kit:

```
<KIT_DIR>/tomcat/work/Catalina/localhost/oxygen-xml-web-author/samples/schematron/
```

available once the kit has been started at least once and the webapp has expanded.

## Failure modes specific to embedding

| Symptom | Cause | Fix |
|---|---|---|
| Rules don't run despite the schema validating | **Embedded Schematron rules** toggle is off | Enable per the toggle above. |
| Rules run but no Quick Fix proposal appears | `xmlns:sqf` declared only on `<sqf:fix>` while `@sqf:fix` on `<sch:assert>` resolves to a different prefix | Declare `xmlns:sqf="…"` on a common ancestor (schema root) and use the same prefix on both. |
| Toggle is on but oXygen still doesn't find the rules | Pattern lives inside an `<xsd:annotation>` in an unexpected place, or in RNG inside `<define>` rather than at the grammar level | Move the pattern to schema root (`<xsd:schema>` for XSD, `<grammar>` for RNG). |
