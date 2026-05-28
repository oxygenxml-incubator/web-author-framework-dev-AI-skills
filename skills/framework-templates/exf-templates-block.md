# `.exf` `<documentTemplates>` Block

How templates are wired into a Web Author framework via a user-uploaded `.exf`. Covers only templates-specific concerns — for the rest of the `.exf` shape, see `exf-structure.md` in the `ai-framework-developer` skill.

Full reference: <https://www.oxygenxml.com/doc/ug-editor/topics/framework-customization-script-usecases.md> (canonical `.exf` element reference, including `<documentTemplates>` / `<addEntry>` / `inherit`).

## Registration

```xml
<documentTemplates>
  <addEntry path="${frameworkDir}/templates/<Category Folder>"/>
  <addEntry path="${frameworkDir}/templates/<Other Category>"/>
</documentTemplates>
```

Web Author treats each `addEntry` path as a **single category**. It does **not** recursively scan a parent `templates/` dir. Pointing `addEntry` at the parent `templates/` makes the extension load silently with no errors and no visible templates — see `troubleshooting.md`.

This matches the bundled DITA framework, whose `templatesLocations` is a flat list of category dirs (`${frameworkDir}/templates/topic`, `${frameworkDir}/templates/sample-project`, …) rather than just `${frameworkDir}/templates`. Cross-check there before emitting.

`<documentTemplates>` entries are **additive** — the wizard merges your entries into the base framework's tree at startup. `<documentTemplates inherit="none">` suppresses base templates (almost never the right call; use only if the user explicitly asks). `<priority>High</priority>` is harmless for `<documentTemplates>` but customary for the surrounding `.exf`.

## `mode = extend` — adding templates to an existing framework

```xml
<?xml version="1.0" encoding="UTF-8"?>
<script
  xmlns="http://www.oxygenxml.com/ns/framework/extend"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://www.oxygenxml.com/ns/framework/extend http://www.oxygenxml.com/ns/framework/extend/frameworkExtensionScript.xsd"
  base="DITA">
  <name>DITA Custom Templates</name>
  <description>Adds workout / mobility plan templates to the DITA framework.</description>
  <priority>High</priority>
  <documentTemplates>
    <addEntry path="${frameworkDir}/templates/Workout"/>
  </documentTemplates>
</script>
```

`<base>` must match the **case-sensitive** `<name>` of the installed framework (`DITA`, not `dita`). Mismatches fail at framework-load time, not at XML validation.

## `mode = new` — registering templates with a brand-new framework

Drop `base=` on `<script>` and add `<associationRules>` (see `association-rules.md` in `ai-framework-developer`). The `<documentTemplates>` block goes in the same `.exf`. `categoryPath=` should start with your framework name, not `DITA/...`.

`${frameworkDir}` resolves to **this** extension's dir (there is no base), so it's the portable form:

```xml
<addEntry path="${frameworkDir}/templates/<Category>"/>
```

## Path placeholder — always `${frameworkDir}`, never `${framework}`

| Placeholder | Form | Use in `<documentTemplates>`? |
|---|---|---|
| `${frameworkDir}` | Plain file path (`D:/.../user-frameworks/<ext>`) | **Yes.** Portable across OSes and across extend / new modes. |
| `${framework}` | URL form (`file:/D:/.../user-frameworks/<ext>`) | **No.** The templates loader doesn't strip the `file:` prefix, so on Windows the SecurityManager rejects the path. (Fine for `<addCss>` — that loader strips it correctly.) See `troubleshooting.md`. |
| Absolute path | Literal filesystem path | **Never.** Breaks when the kit moves or another machine deploys the extension. |

Both placeholders point at the same directory — the `.exf`'s own framework directory. Reference: <https://www.oxygenxml.com/doc/ug-editor/topics/editor-variables.md>.

Same form on Linux, macOS, and Windows; same form for `mode=extend` and `mode=new`.

## Hybrid extensions — templates + CSS placeholders

When using Route B CSS placeholder hints (see `template-files.md`), keep `<documentTemplates>` and `<author><css><addCss .../></css></author>` in the **same** `.exf`. Note the asymmetry: `<addEntry>` uses `${frameworkDir}` (file-path), `<addCss>` uses `${framework}` (URL). Both resolve to the same directory; only the templates loader rejects the URL form.

## One `.exf` per base framework — hard rule

Two extensions with the same `<base>` and the same priority shadow each other; Web Author binds the doctype to one extension's identity and silently drops contributions from the other (templates, CSS, actions). Symptom: extension A's templates appear, B's don't, no log line.

If the user already has an extension for the target base framework, **add the new `<documentTemplates>` block to it** rather than creating a parallel `.exf`. See `troubleshooting.md` for the diagnostic.

## Restart and verify

`user-frameworks/` is scanned only at kit startup — full stop + start required. See `ai-framework-developer` for the exact restart sequence and its `web-author-logs.md` reference for the `Loading user uploaded frameworks from:` log signal. After restart, jump to `troubleshooting.md` for the verification flow.
