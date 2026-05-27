# Oxygen `.scenarios` files - generation guide

This document describes the format of Oxygen `.scenarios` files (validation
scenarios bundled with a framework) so that an AI model can generate them
reliably. The companion XSD is [`scenarios.xsd`](scenarios.xsd).

## Purpose

A `.scenarios` file ships a list of pre-configured validation scenarios for a
framework. Oxygen loads it on startup and exposes the scenarios in the
"Configure Validation Scenario..." dialog. Examples in this repository:

- [`frameworks/dita/dita_map_with_resolved_topics_validation.scenarios`](../../frameworks/dita/dita_map_with_resolved_topics_validation.scenarios)
- [`frameworks/dita/lw/resources/dita-lw-validation.scenarios`](../../frameworks/dita/lw/resources/dita-lw-validation.scenarios)

The same `<validationScenario>` sub-format also appears inline inside
`.framework` files (look for `<validationScenario-array>`).

## Top-level shape

```xml
<?xml version="1.0" encoding="UTF-8"?>
<serialized xml:space="preserve">
  <serializableOrderedMap>
    <entry>
      <String>validation.scenarios</String>
      <validationScenario-array>
        <!-- one or more <validationScenario> -->
      </validationScenario-array>
    </entry>
    <entry>
      <String>validation.scenarios.load.from.project</String>
      <Boolean>false</Boolean>
    </entry>
  </serializableOrderedMap>
</serialized>
```

Both entries are required, in this order. The second entry is almost always
`false` for shipped frameworks (the project's own scenarios are not merged in).

## `<validationScenario>`

Three fields, in this exact order:

| Field   | Type                       | Notes                                       |
|---------|----------------------------|---------------------------------------------|
| `pairs` | `<list>` of `validationUnit` | One or more units, executed top to bottom |
| `type`  | `<String>`                 | Constant `Validation_scenario`              |
| `name`  | `<String>`                 | Display name in the Oxygen UI               |

## `<validationUnit>`

Fields in order:

| Field                       | Body                                | Required | Notes |
|-----------------------------|-------------------------------------|----------|-------|
| `validationType`            | `<validationUnitType>`              | yes      | Wraps `validationInputType` |
| `url`                       | `<String>`                          | yes      | URL of the document to validate; usually `${currentFileURL}` |
| `validationEngine`          | `<validationEngine>`                | yes      | Engine + auto-validation flag |
| `allowAutomaticValidation`  | `<Boolean>`                         | yes      | Enables on-the-fly validation for this unit |
| `extensions`                | `<null/>`                           | yes      | Reserved; keep `<null/>` |
| `validationSchema`          | `<null/>` or `<validationUnitSchema>` | yes    | See below |
| `validationAdvancedSettings`| `<null/>` or PO object              | optional | Engine-specific (e.g. DITA Map completeness options) |

### `validationInputType` (known values)

- `text/xml` - XML/DITA/DocBook/XHTML/...
- `text/sch` - Schematron
- `text/any` - JSON, YAML, generic content (used for AsyncAPI, OpenAPI, JSON-LD)

### `engineType` (commonly seen, non-exhaustive)

| Value                                                       | When to use |
|-------------------------------------------------------------|-------------|
| `<Default engine>`                                          | Whatever the document type is associated with by default |
| `DITA Validation`                                           | DITA-specific checks |
| `DITA Map Validation and Completeness Check`                | Validates a map and checks key/topic resolution |
| `DITA-OT Project Validation and Completeness Check`         | Same, for DITA-OT projects |
| `Table Layout Validation`                                   | CALS/HTML table layout |
| `Saxon-EE`, `Xerces`                                        | XSD validation with a specific engine |
| `W3C HTML Validator`                                        | HTML files |
| `HTML Schematron Validator`, `JSON Schematron Validator`    | Schematron applied to HTML/JSON |

Note: in XML attributes/text the value is encoded as `&lt;Default engine&gt;`
(or `&lt;Default engine>` - both occur in the repository).

Custom engines registered by add-ons are also valid; AI generators should not
reject unknown engine names.

## `<validationEngine>`

```xml
<validationEngine>
  <field name="engineType"><String>...</String></field>
  <field name="allowsAutomaticValidation"><Boolean>true|false</Boolean></field>
</validationEngine>
```

`allowsAutomaticValidation` advertises whether the engine *supports* automatic
validation. Per-unit on/off is `validationUnit/allowAutomaticValidation`.

## `<validationUnitSchema>` (when not null)

```xml
<validationUnitSchema>
  <field name="dtdSchemaPublicID"><null/></field>          <!-- or <String> -->
  <field name="schematronPhase"><null/></field>            <!-- or <String> -->
  <field name="type"><Integer>10</Integer></field>         <!-- SchemaTypes -->
  <field name="uri"><String>${framework}/schemas/foo.json</String></field>
</validationUnitSchema>
```

### `SchemaTypes` (from `ro.sync.basic.xml.schema.SchemaTypes`)

| `type` | Constant            | Meaning                                  |
|--------|---------------------|------------------------------------------|
| 0      | `ST_NOT_SPECIFIED`  | Not specified                            |
| 1      | `ST_DTD`            | DTD                                      |
| 2      | `ST_XMLSCHEMA`      | XML Schema (`.xsd`)                      |
| 3      | `ST_RNC`            | Relax NG compact                         |
| 4      | `ST_RNG`            | Relax NG XML syntax                      |
| 5      | `ST_XMLSCHEMA_SCH`  | XML Schema with embedded Schematron      |
| 6      | `ST_RNG_SCH`        | Relax NG XML with embedded Schematron    |
| 7      | `ST_SCH`            | Schematron                               |
| 9      | `ST_NVDL`           | NVDL                                     |
| 10     | `ST_JSON`           | JSON instance (validated against JSON Schema) |
| 11     | `ST_JSON_SCHEMA`    | JSON meta schema                         |

(Values 8 is intentionally absent.)

## URL variables

The `url` and `validationUnitSchema/uri` fields commonly use Oxygen editor
variables:

- `${currentFileURL}` - the file currently being edited
- `${framework}` - root URL of the framework folder; ideal for built-in schemas
- `${cfdu}`, `${cfd}`, `${pd}` - other Oxygen variables (see Oxygen docs)

## Field order matters

Oxygen's serializer writes object fields in a fixed order. Generators should
follow the order in the XSD and in the examples below; otherwise the file
still parses but diffs against shipped scenarios become noisy.

## Example 1 - simplest, default engine, no schema

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
                    <field name="engineType"><String>&lt;Default engine></String></field>
                    <field name="allowsAutomaticValidation"><Boolean>true</Boolean></field>
                  </validationEngine>
                </field>
                <field name="allowAutomaticValidation"><Boolean>true</Boolean></field>
                <field name="extensions"><null/></field>
                <field name="validationSchema"><null/></field>
              </validationUnit>
            </list>
          </field>
          <field name="type"><String>Validation_scenario</String></field>
          <field name="name"><String>My XML</String></field>
        </validationScenario>
      </validationScenario-array>
    </entry>
    <entry>
      <String>validation.scenarios.load.from.project</String>
      <Boolean>false</Boolean>
    </entry>
  </serializableOrderedMap>
</serialized>
```

## Example 2 - JSON instance validated against a bundled JSON Schema

```xml
<validationUnit>
  <field name="validationType">
    <validationUnitType>
      <field name="validationInputType"><String>text/any</String></field>
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
      <field name="dtdSchemaPublicID"><null/></field>
      <field name="schematronPhase"><null/></field>
      <field name="type"><Integer>10</Integer></field>
      <field name="uri"><String>${framework}/schemas/asyncapi/v3.x/3.0.0.json</String></field>
    </validationUnitSchema>
  </field>
  <field name="validationAdvancedSettings"><null/></field>
</validationUnit>
```

## Caveats

- The XSD is "best effort, strict": it covers everything observed in the
  shipped frameworks. Oxygen itself accepts more shapes (e.g. an `extensions`
  list, advanced settings POs). Such extras are modeled with `xs:any
  processContents="lax"` so the schema does not reject valid-but-rare files.
- The `<` in `<Default engine>` may appear escaped as `&lt;` or `&lt;...&gt;`
  in the wild - both forms are produced by Oxygen's serializer and are
  semantically identical.
- `xml:space="preserve"` on the root is part of the canonical output; keep it
  when generating new files.
