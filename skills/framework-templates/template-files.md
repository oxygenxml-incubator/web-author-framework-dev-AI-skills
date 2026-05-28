# Template Files

Authoritative shape for the `templates/` folder shipped inside the `.exf` extension. Cross-check against a bundled framework (e.g. `<BUNDLED_FRAMEWORKS_DIR>/dita/templates/topic/`) before emitting anything unusual.

Full reference: <https://www.oxygenxml.com/doc/ug-editor/topics/customizing-templates.md> (`displayName`, prefix/suffix, icons, i18n, `<?oxy-placeholder?>` PI) and <https://www.oxygenxml.com/doc/ug-editor/topics/dg-file-templates.md>. Read via the `oxygen-docs` skill.

## Folder layout

```
templates/
└── <Category Folder>/
    ├── category.properties        # categoryPath=Top/Sub
    ├── <Template Name>.dita       # the seed document (or .xml, .docbook, …)
    └── <Template Name>.properties # metadata (type, displayName, icons, prefixes, tags)
```

**Terminology** — "seed" / "seed document" / "seed file" all mean the same thing: the `<Name>.dita` (or `.xml`, …) file Web Author copies and opens when the author picks the template from the New File wizard. Editor variables (`${id}`, `${caret}`, …) are expanded against this file at copy time.

**One `<addEntry>` in the `.exf` per category folder** — Web Author does *not* recursively scan a parent `templates/` dir. See `exf-templates-block.md`.

## `category.properties`

One line, in the same folder as the `.dita` / `.properties` pair:

```
categoryPath=DITA/Workout
```

Slash-separated, no leading slash. For `mode=new` extensions, start the path with your framework name, not `DITA/...`.

## `<Template Name>.properties`

Filename **without** the extension matches the seed file's name (`Workout Plan.dita` ↔ `Workout Plan.properties`). All fields are documented at the customizing-templates page above; the WA-relevant subset:

| Field | Notes |
|---|---|
| `type` | `dita` for DITA topics, `general` otherwise. **`type=dita` is required for the template to appear in DITA Maps Manager flows** — otherwise it silently disappears from those entry points. |
| `displayName` | Wizard label override. Without it, the wizard shows the filename. With it, you can rename the seed file freely. Supports `${i18n(tag)}` against the framework's `i18n/translation.xml`. |
| `tags` | Comma-separated. `tags=popular` promotes the template to the wizard's top-level **Popular** category — see below. |
| `smallIcon` / `bigIcon` | Paths relative to the `.properties` file. New-file wizard only, not used elsewhere in the UI. |
| `filenamePrefix` / `filenameSuffix` | Prepended / appended in the new-file dialog. Editor variables allowed **except** `${ask()}` and `${answer()}`. |
| `longDescriptionReference` | Optional HTML file (relative path) shown as the wizard's long description. |

## Popular category

The wizard's top-level **Popular** category aggregates templates from *all* frameworks via the `tags` property. Any template whose sibling `.properties` lists `popular` in `tags=` appears there, regardless of framework or template type (DITA topic, DocBook chapter, TEI doc, plain XML — same mechanism).

Bundled reference: `<BUNDLED_FRAMEWORKS_DIR>/dita/templates/topic/Topic.properties` ships with `tags=popular`.

Reference: <https://www.oxygenxml.com/doc/ug-editor/topics/new-dialog-sa.md>.

## Templates are skeletons, not sample documents

A template is structural scaffolding plus hints — the author should *type into* it, not *delete from* it. Prefer empty elements with placeholder hints over pre-written prose; keep one or two skeletal entries in lists / `<steps>` / tables; put worked examples under `samples/`, not in the template body.

Heuristic: if you removed every placeholder hint, would what's left still read like a finished document? If yes, strip it back to scaffolding.

## Placeholders inside the seed

Two routes for "type-here" hints — pick by scope.

**Route A — `<?oxy-placeholder?>` PI** (per-template, no CSS). Drop a PI inside each empty element:

```xml
<topic id="workout_${id}">
  <title><?oxy-placeholder content="Type the workout name"?></title>
  <body>
    <p><?oxy-placeholder content="Describe the workout"?></p>
  </body>
</topic>
```

The element holding the PI must contain *no other content, not even whitespace* (indentation inside the element breaks rendering). Default choice for a one-off template. Reference: <https://www.oxygenxml.com/doc/ug-editor/topics/customizing-templates.md#adding_placeholders_or_hints_in_a_document_templa>.

**Route B — `-oxy-placeholder-content` CSS** (per-doctype, scoped). Leave elements empty; add a CSS rule. Used in bundled `<BUNDLED_FRAMEWORKS_DIR>/dita/css/hints/hints.css`:

```css
@media oxygen {
  task[outputclass~="faq"] > title:empty {
    -oxy-show-placeholder: always;
    -oxy-placeholder-content: "Type the question";
  }
}
```

Scope hints to documents from *this* template with an `outputclass` (or another marker) on the seed's root and a `[outputclass~="..."]` selector. Hybrid extensions (templates + CSS) keep both blocks in the **same** `.exf` — see `exf-templates-block.md`. Reference: <https://www.oxygenxml.com/doc/ug-editor/topics/dg-placeholder-css-extension.md>.

**When to pick which**:

| Situation | Route |
|---|---|
| One template, hints in a few elements | A (PI) |
| Same hint across many documents sharing a marker | B (CSS) |
| Element must contain whitespace or other content | B — A's no-whitespace rule disqualifies it |
| Want translated hints via `translation.xml` | B (`oxy_xpath` / i18n) |

## Editor variables in seed content

Expanded **once**, at file-creation time. Common ones in templates: `${id}` (generated unique id — use as `id="prefix_${id}"`), `${caret}` (cursor landing position), `${date(yyyy-MM-dd)}`, `${user.name}`. Full list: <https://www.oxygenxml.com/doc/ug-editor/topics/editor-variables.md>. For **Web Author**, the grounded subset of what actually expands in seeds lives in `editor-variables-web-author.md` in the `ai-framework-developer` skill — load it whenever a WA seed contains `${...}`.

Typo traps that fail silently in the saved file: `$ {id}` (extra space) and `${Id}` (wrong case) — neither is expanded. Keep `${id}` inside text or attribute values.

## Before emitting — cross-checks and schema grounding

1. Open one bundled `<Name>.properties` and one bundled `category.properties` for the target framework (e.g. `<BUNDLED_FRAMEWORKS_DIR>/dita/templates/topic/`) and copy the field shape that framework actually uses. For DITA, double-check `type=dita`.
2. **Ground the seed in the actual schema.** Never write seed content from memory of the vocabulary — real DITA / DocBook / TEI content models have ordering and placement constraints that look fine when written from intuition and fail validation as soon as the user opens the file.
3. Open the schema: DITA DTD via the doctype declaration of the bundled template (e.g. `<!DOCTYPE task PUBLIC "-//OASIS//DTD DITA Task//EN" "task.dtd">` → `<BUNDLED_FRAMEWORKS_DIR>/dita/dtd/technicalContent/dtd/task.dtd` via the framework's catalog). DocBook 5.x: RNG under `<BUNDLED_FRAMEWORKS_DIR>/docbook/<version>/rng/`. TEI: RNG under `<BUNDLED_FRAMEWORKS_DIR>/tei/...`.
4. Validate each seed against its schema before moving on — don't batch-write a dozen and validate at the end.
