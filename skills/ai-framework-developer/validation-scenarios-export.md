# Validation scenarios — `.scenarios` files (findings)

Reference for **how validation scenarios ship with frameworks** when not authored only via the oXygen GUI.

## Official docs (behavior, not file grammar)

- Wire-up from a Framework Extension Script: **`<validationScenarios>`** in `.exf` with `<addScenarios>`, `<removeScenario>`, `<defaultScenarios>` — see [Framework Extension Script File](https://www.oxygenxml.com/doc/ug-editor/topics/framework-customization-script-usecases.html).

## At a glance

- Extension in practice: **`.scenarios`** (not `.scenario`); Java XML serialization with a `<serialized>` / `<serializableOrderedMap>` wrapper around a `validationScenario-array`.
- The same `<validationScenario>` / `<validationUnit>` subtree also appears inline inside `*.framework` files under `<field name="validationScenarios">` — copy patterns from there.

## On-demand: file grammar reference (always load when generating a `.scenarios` file)

- `schemas/scenarios-guide.md` — prose walkthrough: top-level shape, `<validationScenario>` / `<validationUnit>` field order, known `validationInputType` and `engineType` values, full `SchemaTypes` table, `${...}` URL variables, two complete worked examples (default-engine XML; JSON instance against a bundled JSON Schema), caveats around `&lt;Default engine&gt;` escaping and `xml:space="preserve"`.
- `schemas/scenarios.xsd` — strict-but-permissive XSD covering everything observed in shipped frameworks; enforces field order and the `SchemaTypes` enumeration, uses `xs:any processContents="lax"` for rare engine-specific advanced settings. Useful as a generation target and for catching field-order drift.

## Standalone `.scenarios` files in a Web Author kit

Under `<EXPANDED_WEBAPP_DIR>/frameworks/dita/`:

- `lw/resources/dita-lw-validation.scenarios`
- `dita_map_with_resolved_topics_validation.scenarios`

Referenced from `dita-lw.exf` and `dita_map_with_resolved_topics.exf` via `<addScenarios href="…"/>`.

## Embedded examples (not separate files)

`*.framework` files that embed the structure under `<field name="validationScenarios">`: `dita.framework`, `ditamap.framework`, `docbook5.framework`, `tei/teip5jtei.framework`. Good source for engine patterns (`<Default engine>`, `DITA Validation`, `Table Layout Validation`, map completeness checks) and for real `validationUnitSchema/type` values — e.g. bundled TEI jTEI uses `6` (RNG + embedded Schematron); DITA SQF samples use `7`. Full `SchemaTypes` enum is in `schemas/scenarios-guide.md`.

## Practical guidance

1. Point to the file from `.exf` with `<addScenarios href="…"/>`; use `${framework}`, `${frameworkDir}`, or sample-style `${pdu}` as appropriate for path resolution.
2. For "default grammar only" needs, prefer `<defaultSchema>` in `.exf` over a full scenario — see `exf-structure.md`.

## SQF

For Schematron Quick Fixes themselves (`sqf:fix`, `sqf:add`, `sqf:delete`, `sqf:replace`, `sqf:stringReplace`, `<sqf:user-entry>`, `<sqf:call-fix>`, `<sqf:group>`, `<sqf:fixes>`, `<sqf:param>`, `@use-when`, `@use-for-each`) embedded in `.sch` files referenced by these scenarios, use the `schematron-quick-fix` skill. This file remains the right reference for the `.scenarios` serialized export format itself.
