# EXF Framework Extension Script Reference

Grounded reference for `.exf` files, external author actions, and the content-completion config file. Anchored in the local `schemas/` (authoritative XSDs + Schematron) and `samples/` (real, working files).

Official doc pages — fetch the `.md` via the `oxygen-docs` flow:

- [Creating a Framework Using an Extension Script](https://www.oxygenxml.com/doc/ug-editor/topics/framework-customization-script.md)
- [Framework Extension Script File](https://www.oxygenxml.com/doc/ug-editor/topics/framework-customization-script-usecases.md) — element/attribute reference

## Schemas (consult before generating XML)

- **`schemas/frameworkExtensionScript.xsd`** — XSD for `.exf`. Root `<script>` in `http://www.oxygenxml.com/ns/framework/extend`. Covers `name`, `description`, `priority`, `associationRules`, `defaultSchema`, `classpath`, `xmlCatalogs`, `author` (CSS, toolbars, menus, contextual menus, content completion, author actions), `documentTemplates`, `transformationScenarios`, `validationScenarios`, `extensionPoints`, `webResources`.
- **`schemas/frameworkExtensionScript.sch`** — Schematron rules: `@base` non-empty if present, `name` non-empty, content-completion `addAction` requires one of `@inCCWindow` / `@inElementsView` / `@inMenus`, no duplicate extension points.
- **`schemas/authorAction.xsd`** — XSD for external author actions. Root `<authorAction>` in `http://www.oxygenxml.com/ns/author/external-action`. Required `@id`; optional `name`, `description`, `smallIconPath`, `largeIconPath`, `accessKey`, `accelerator`, `enabledInReadOnlyContext`, and one or more `<operation>` entries (`@id` = operation class, optional `<xpathCondition>`, `<arguments>`).
- **`schemas/ccConfigSchemaFilter.xsd`** — XSD for `cc_config.xml`. Root `<config>` in `http://www.oxygenxml.com/ns/ccfilter/config` with `elementProposals`, `valueProposals`, `elementRenderings`.
- **`schemas/ccConfigSchemaFilter.sch`** — Schematron rules for `cc_config.xml` (validates `<match>` and recommends `<valueProposals>` over the deprecated `<match>`).

## `.exf` structure (quick reference)

Root element: `<script>` in namespace `http://www.oxygenxml.com/ns/framework/extend`.

- **`@base`** *(optional)* — base framework to extend (`"DITA"`, `"DocBook"`, `"TEI"`, …). Omit for a standalone framework.
- **`<name>`** *(required)*, **`<description>`** *(required)*, **`<priority>`** — `Lowest` | `Low` | `Normal` | `High` | `Highest`.
- **`<associationRules>`** — `<addRule>` with `@rootElementLocalName`, `@namespace`, `@fileName`, `@publicID`, `@attributeLocalName`, `@attributeNamespace`, `@attributeValue`, `@javaRuleClass`. Use `@inherit="none"` to discard base rules.
- **`<defaultSchema>`** — `@schemaType` (`dtd`, `xmlschema`, `rng`, `rnc`, `sch`, `json_schema`, …) + `@href`.
- **`<classpath>`** — `<addEntry path="…"/>` / `<removeEntry path="…"/>`. Supports `@inherit`, `@parentClassLoaderID`.
- **`<xmlCatalogs>`** / **`<documentTemplates>`** — same `<addEntry>` / `<removeEntry>` pattern.
- **`<author>`** — Author-mode customizations:
  - `<css>` — `<addCss path="…" alternate="true|false" title="…"/>`, `<removeCss path="…"/>`.
  - `<toolbars>` — `<toolbar name="…">` with `<addAction id="…"/>`, `<separator/>`, `<group>`, `<removeAction>`, `<removeGroup>`.
  - `<menu>` / `<contextualMenu>` — `<addAction>`, `<submenu>`, `<separator>`, `<removeAction>`, `<removeSubmenu>`.
  - `<contentCompletion>` — `<schemaProposals>` (`<addProposal>` / `<removeProposal>`) and `<authorActions>` (`<addAction id="…" inCCWindow="true" replacedElement="…"/>`).
  - `<authorActions>` — `<removeAction id="…"/>` to remove inherited actions.
- **`<transformationScenarios>`** / **`<validationScenarios>`** — `<addScenarios href="…"/>`, `<removeScenario name="…"/>`, `<defaultScenarios>`.
- **`<extensionPoints>`** — `<extension name="extensionsBundle" value="com.example.MyExtensionsBundle"/>` and other Java extension points.

`@inherit` (`"all"` | `"none"`) controls inheritance from `@base`. `@position` (`"before"` | `"after"`) controls insertion order relative to inherited entries. Use `${framework}` / `${frameworkDir}` for paths relative to the framework directory.

For `<removeCss>` / `<removeEntry>`, the `@path` placeholder must match the base's declared form. Allowed swaps: `${framework}` ↔ `${baseFramework}`, `${frameworkDir}` ↔ `${baseFrameworkDir}`. See `ai-framework-developer/exf-structure.md` "Path placeholders" for details and the sample under `samples/extend-dita-with-css-and-classpath.exf`.

## External author action (quick reference)

Root: `<authorAction>` in `http://www.oxygenxml.com/ns/author/external-action`.

- **`@id`** *(required)* — referenced from toolbars, menus, content completion.
- **`<name>`** *(required)*, **`<description>`** (tooltip).
- **`<smallIconPath>`** / **`<largeIconPath>`** — `${framework}` for framework-relative, `/path` for classpath.
- **`<accelerator>`** — e.g. `"M1+M2+T"` (M1=Cmd/Ctrl, M2=Shift, M3=Alt/Option).
- **`<operations>`** — one or more `<operation>` with `@id` (FQCN or built-in short name like `InsertFragmentOperation`), optional `<xpathCondition>` (XPath 2.0), and `<arguments>` (`<argument name="…">value</argument>`).

External action files live in `{exf-script-name}_externalAuthorActions/` next to the `.exf` (or in `externalAuthorActions/` at the framework root).

## Sample `.exf` files (in `samples/`)

- **`extend-dita-qa.exf`** — extend DITA for Q/A topics: association rules, templates, toolbar, content completion, menus, removing inherited actions.
- **`extend-dita-with-css-and-classpath.exf`** — CSS add/remove (incl. alternate styles), classpath modifications, validation scenarios, Java extensions bundle, toolbar / contextual menu.
- **`extend-dita-map-resolved.exf`** — Java rule matcher for association, transformation/validation scenarios, extensions bundle.
- **`custom-json-framework.exf`** — standalone JSON framework: `javaRuleClass`, `parentClassLoaderID`, `schemaType="json_schema"`, document templates, `selectMultipleAlternateCSS`.

## Sample external author actions (in `samples/actions/`)

- `insert.qagroup.xml` — simple `InsertFragmentOperation`.
- `insert.section.xml` — multiple operations with XPath conditions for context-aware insertion.
- `insert.note.xml` — combines `InsertFragmentOperation` and `SurroundWithFragmentOperation`.
- `insert.table.xml` — multi-line XML fragment with `${caret}` positioning.
- `insert.topicref.xml` — custom Java operation with XPath condition.

## Sample CSS (in `samples/css/`)

- `author-mode-form-controls.css` — `oxy_combobox` (with tooltips), `oxy_urlChooser`, `oxy_editor` + `oxy_action` (insert button), `-oxy-placeholder-content`, `-oxy-collapse-text`, `-oxy-not-foldable-child`, `:before` label pseudo-elements.
