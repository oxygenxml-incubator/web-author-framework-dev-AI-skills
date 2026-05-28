# EXF File Structure

Authoritative shape of a `.exf` Framework Extension Script. Cross-check against `frameworkExtensionScript.xsd` (mirrored under `oxygen-docs/schemas/`) before emitting anything unusual.

## Root element

```xml
<script
  xmlns="http://www.oxygenxml.com/ns/framework/extend"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://www.oxygenxml.com/ns/framework/extend http://www.oxygenxml.com/ns/framework/extend/frameworkExtensionScript.xsd"
  base="DITA">
  ...
</script>
```

- **Namespace** — `http://www.oxygenxml.com/ns/framework/extend` (required, fixed).
- **`@base`** *(optional, `xs:string`)* — name of the base framework to extend (`"DITA"`, `"DocBook"`, `"TEI"`, `"XHTML"`, `"JSON"`, …). The schema does not constrain the value; it must match the `<name>` of an installed framework at runtime — mismatches fail at framework-load time, not XML validation. Omit to create a *standalone* framework.

## Required top-level children

| Element | Purpose |
|---|---|
| `<name>` | Framework name. For an extension this is a new label; for a standalone framework it becomes the framework's identity. |
| `<description>` | Short human-readable description. |

## Common top-level children

All children are wrapped in `<xs:all>` — order does not matter.

| Element | Purpose / key attributes |
|---|---|
| `<initialPage>` | Default editor mode when opening a doc for the first time: `EditorSpecific` (default), `Text`, `Author`, `Grid`, `Design`. |
| `<priority>` | `Lowest`, `Low`, `Normal`, `High`, `Highest`. Higher wins when multiple frameworks claim the same document. Use `High` for AI-generated extensions so they override the bundled framework. |
| `<associationRules>` | Container for `<addRule>` entries. See `association-rules.md`. Use `@inherit="none"` to discard the base's rules. |
| `<defaultSchema>` | `@schemaType` (`dtd`, `xmlschema`, `rng`, `rnc`, `xmlschema_sch`, `rng_sch`, `sch`, `nvdl`, `json_schema`, `json_meta_schema`) and `@href` (both required). Used when the document declares no schema. |
| `<classpath>` | `<addEntry path="..."/>` and `<removeEntry path="..."/>`. Supports `@inherit` and `@parentClassLoaderID` (the ID of a plugin whose classes this framework can access). |
| `<xmlCatalogs>` | `<addEntry>` / `<removeEntry>`. |
| `<documentTemplates>` | `<addEntry>` / `<removeEntry>` — see `framework-templates` skill. |
| `<author>` | Container for Author-mode customizations (see below). |
| `<transformationScenarios>` / `<validationScenarios>` | `<addScenarios href="..."/>`, `<removeScenario name="..."/>`, `<defaultScenarios><name>…</name>…</defaultScenarios>`. |
| `<extensionPoints>` | `<extension name="..." value="..."/>` for Java extension hooks. The XSD enumerates ~20 valid `@name` values — most common is `extensionsBundle` (a single bundle exposing every other extension point). Full list: `schemaManagerFilterExtension`, `elementLocatorExtension`, `authorReferenceResolver`, `authorCssStylesFilterExtension`, `authorTableCellSpanProvider`, `authorTableCellSepProvider`, `authorTableColumnWidthProvider`, `authorExtensionStateListener`, `attributesRecognizer`, `xmlNodeCustomizerExtension`, `authorModeExternalObjectInsertionHandler`, `customAttributeValueEditor`, `authorEditPropertiesHandler`, `authorActionEventHandler`, `authorImageDecorator`, `textModeExternalObjectInsertionHandler`, `authorSwingDndExtension`, `authorSWTDndExtension`, `textSWTDndExtension`. Pull the matching doc topic via `oxygen-docs` before using one. |
| `<webResources>` | Web Author-only. `<addEntry>` / `<removeEntry>` — list of JS files or folders to load on the WA client. Supports `@inherit`. *(Present in XSD; not covered in `framework-customization-script-usecases` topic — likely Web Author-only.)* |

## Inside `<author>`

Children are in `<xs:all>` — order does not matter. Available: `<authorActions>`, `<css>`, `<toolbars>`, `<contextualMenu>`, `<menu>`, `<contentCompletion>`.

| Element | Purpose |
|---|---|
| `<css>` | `<addCss path="..." position="before|after" alternate="true|false" title="..."/>`, `<removeCss path="..."/>`. Container attributes: `@selectMultipleAlternateCSS` (default `true` — when `true`, multiple alternate CSSes layer; when `false`, only one alternate at a time) and `@mergeDocumentCSS` (default `false` — controls whether CSS declared inside the document merges with the framework's). **Bread-and-butter for visual customization** — see `framework-style-changes` skill. |
| `<toolbars>` | `<toolbar name="...">` containing `<addAction id="..."/>`, `<separator/>`, `<group>`, `<removeAction>`, `<removeGroup>`. |
| `<menu>` / `<contextualMenu>` | `<addAction>`, `<submenu>`, `<separator>`, `<removeAction>`, `<removeSubmenu>`. |
| `<contentCompletion>` | `<schemaProposals>` (`<addProposal renderName="..."/>` / `<removeProposal renderName="..." fromCCWindow="..." fromElementsView="..." fromEntitiesView="..." fromMenus="..."/>`) and `<authorActions>` (`<addAction id="..." alias="..." displayOnlyWhenElementAllowed="..." inCCWindow="..." inElementsView="..." inMenus="..." replacedElement="..." replacedElementNs="..." useReplaceElementName="..."/>`). The XSD does *not* mark `inCCWindow` / `inElementsView` / `inMenus` as required, but `frameworkExtensionScript.sch` enforces that at least one is set per `addAction` — both schemas must validate. |
| `<authorActions>` *(directly under `<author>`)* | Contains only `<removeAction id="..."/>` — drops inherited actions from the base framework. **Distinct** from `<author>/<contentCompletion>/<authorActions>`, which adds new actions. New actions themselves are *defined* in external XML files (see "External Author Action Files" below) and *referenced* by `id` from toolbars / menus / content completion. |

## Universal attributes

These appear on many child elements and behave consistently:

- **`@inherit`** — `"all"` (default) inherits the base framework's entries; `"none"` discards them.
- **`@position`** — `"before"` or `"after"` controls insertion order relative to inherited entries.

## Path placeholders

Two axes: **which framework** (current, named, base, parent) × **which form** (URL or file path). All eight combinations:

| Variable | Resolves to | Form |
|---|---|---|
| `${framework}` | current framework dir | URL |
| `${frameworkDir}` | current framework dir | file path |
| `${framework(NAME)}` | named framework dir (e.g. `DITA`) | URL |
| `${frameworkDir(NAME)}` | named framework dir | file path |
| `${baseFramework}` | base framework dir (only meaningful with `@base`) | URL |
| `${baseFrameworkDir}` | base framework dir | file path |
| `${frameworks}` | parent `frameworks/` dir | URL |
| `${frameworksDir}` | parent `frameworks/` dir | file path |

Pick by use case:

- **`<addCss>`, `<addEntry>` under `<classpath>`/`<xmlCatalogs>`/`<webResources>`, `<smallIconPath>`** — `${framework}` (your own files) or `${framework(NAME)}` (another framework's files).
- **`<documentTemplates>/<addEntry>`** — `${frameworkDir}` (file-path form required). See `framework-templates` skill.
- **`<removeCss>` / `<removeEntry>`** — see the rule below; placeholder form must match what the base declared.


- editor variables: <https://www.oxygenxml.com/doc/ug-editor/topics/editor-variables.md>

**Never ship absolute machine paths.** They break the moment the kit moves.

### `removeCss` / `removeEntry` — match the base's placeholder form

The base framework declares each entry with some `${...}/<rest>` path. To remove that entry, your `.exf` must use a matching form. The equivalence rule (from the `.exf` docs):

| Base declared | You can remove with |
|---|---|
| `${framework}/<rest>` | `${framework}/<rest>` or `${baseFramework}/<rest>` |
| `${frameworkDir}/<rest>` | `${frameworkDir}/<rest>` or `${baseFrameworkDir}/<rest>` |


## External Author Action Files

Custom Author actions are defined in separate XML files, **not inline** in the `.exf`. They are then referenced from the `.exf` by `@id`.

- **Location** — folder named `{exf-script-name}_externalAuthorActions/` next to the `.exf`, OR `externalAuthorActions/` at the framework dir level.
- **Root element** — `<authorAction>` in namespace `http://www.oxygenxml.com/ns/author/external-action`.

| Element / attribute | Purpose |
|---|---|
| `@id` *(required)* | Unique action identifier. References from `<addAction id="..."/>` in toolbars / menus / content completion target this id. |
| `<name>` *(required)* | Display name. |
| `<description>` | Tooltip text. |
| `<smallIconPath>` / `<largeIconPath>` | Icon paths. Use `${framework}` for relative paths, or `/path` for classpath resources. |
| `<accelerator>` | Keyboard shortcut. `M1` = Cmd/Ctrl, `M2` = Shift, `M3` = Alt/Option. Example: `M1+M2+T`. |
| `<enabledInReadOnlyContext>` | `true`/`false`. |
| `<operations>` | Container for one or more `<operation>` elements. Each: `@id` (fully qualified Java class or built-in operation short name like `InsertFragmentOperation`), optional `<xpathCondition>`, `<arguments>` (`<argument name="...">value</argument>`). Multiple operations let you switch behavior by `xpathCondition`. |

## Validation

Two schemas constrain `.exf`:

- **`frameworkExtensionScript.xsd`** — element/attribute structure.
- **`frameworkExtensionScript.sch`** — Schematron rules. Notably enforces: non-empty `@base` if present, non-empty `<name>`, content-completion `addAction` requires at least one of `@inCCWindow` / `@inElementsView` / `@inMenus`, no duplicate extension points.

If a `.exf` is rejected with `ExtensionStructureException`, validate against both schemas locally before re-uploading.

## Minimal extension example

```xml
<?xml version="1.0" encoding="UTF-8"?>
<script
  xmlns="http://www.oxygenxml.com/ns/framework/extend"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://www.oxygenxml.com/ns/framework/extend http://www.oxygenxml.com/ns/framework/extend/frameworkExtensionScript.xsd"
  base="DITA">
  <name>DITA Custom</name>
  <description>Custom CSS layered over the bundled DITA framework.</description>
  <priority>High</priority>
  <author>
    <css>
      <addCss path="${framework}/css/custom.css" position="after"/>
    </css>
  </author>
</script>
```

## Minimal standalone (new framework) example

```xml
<?xml version="1.0" encoding="UTF-8"?>
<script
  xmlns="http://www.oxygenxml.com/ns/framework/extend"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://www.oxygenxml.com/ns/framework/extend http://www.oxygenxml.com/ns/framework/extend/frameworkExtensionScript.xsd">
  <name>My Framework</name>
  <description>Custom standalone framework.</description>
  <priority>High</priority>
  <associationRules inherit="none">
    <addRule rootElementLocalName="my-root" namespace="http://example.org/my-ns"/>
  </associationRules>
  <defaultSchema schemaType="rng" href="${framework}/schemas/main.rng"/>
  <author>
    <css>
      <addCss path="${framework}/css/main.css" position="after"/>
    </css>
  </author>
</script>
```

For a fuller standalone-framework starter (folder layout, `catalog.xml`, dev-scaffold CSS), see [examples/starter-framework.md](examples/starter-framework.md).

## XSD spec links (W3C)

External references for **XSD syntax and semantics** (not fetchable via `oxygen-docs`). Starting point and normative specs listed on [XML Schema (namespace)](https://www.w3.org/2001/XMLSchema):

- [W3C XML Schema 1.0 Part 1: Structures (2nd Edition)](https://www.w3.org/TR/xmlschema-1/)
- [W3C XML Schema 1.0 Part 2: Datatypes (2nd Edition)](https://www.w3.org/TR/xmlschema-2/)
- [W3C XML Schema Definition Language (XSD) 1.1 Part 1: Structures](https://www.w3.org/TR/xmlschema11-1/)
- [W3C XML Schema Definition Language (XSD) 1.1 Part 2: Datatypes](https://www.w3.org/TR/xmlschema11-2/)
