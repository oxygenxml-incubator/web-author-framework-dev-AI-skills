---
name: framework-templates
description: Use when adding, registering, or customizing document/file templates, OR when answering questions about template behavior — editor variables, expansion rules, properties files, the New File wizard — in oXygen Web Author or desktop. Also packages templates as a user-framework `.exf` extension and verifies they appear after a kit restart.
---

# Framework Templates

Adding **document templates** to a Web Author framework. Templates appear in the New File wizard under a category path you choose; the payload is a `templates/` folder shipped inside an `.exf` extension. If the user wants to **style the Author view** instead, that's `framework-style-changes`.

## References

- `.exf` `<documentTemplates>` shape, extend-vs-new, path placeholders — `exf-templates-block.md`
- Folder layout, `category.properties`, `<Name>.properties`, placeholders, editor variables — `template-files.md`
- Verification + WA-specific failure modes (silent loads, Windows `${framework}` bug, parallel-extension trap) — `troubleshooting.md`
- Curated docs index for templates — `doc-references.md`
- **Web Author-only** `${...}` expansion in template seeds and Author actions (which variables expand at New File time, which stay literal, `${ask(...)}` rules) — `editor-variables-web-author.md` in the `ai-framework-developer` skill. Load when the target is Web Author and the seed contains `${...}`; skip for desktop oXygen.
- `.exf` general structure — `ai-framework-developer` skill (`exf-structure.md`)
- CSS-route placeholder hints (`-oxy-placeholder-content`) — `framework-style-changes` skill
- Browser verification — `chrome-mcp-usage.md` in the `ai-framework-developer` skill
- Server log diagnosis — `web-author-logs.md` in the `ai-framework-developer` skill
- Authoritative manual lookup when stuck — `oxygen-docs` skill

## Required flow

1. Confirm with the user whether the task is `extend` (existing framework, case-sensitive `<base>`) or `new`. Don't infer.
2. Read `exf-templates-block.md` before writing the `.exf`. Read `template-files.md` before writing `category.properties` / `<Name>.properties` / placeholders. For Web Author + `${...}` in seeds, also load `editor-variables-web-author.md` in `ai-framework-developer`.
3. **Ground every seed in the actual DTD / XSD / RNG of the target framework. Never write seed content from memory of the vocabulary.** Open the schema (e.g. `<BUNDLED_FRAMEWORKS_DIR>/dita/dtd/technicalContent/dtd/task.dtd`, or whatever the doctype declares) and confirm element names, allowed children, and required ordering before emitting. Cross-check against a bundled template as a second source. Applies to DITA, DocBook, TEI, or anything else — guessing produces validation errors the user has to report back.
4. Keep all edits under `USER_FRAMEWORKS_DIR/<session>/`. Never write into `BUNDLED_FRAMEWORKS_DIR/`.
5. **Confirming a seed is correct = two steps, and nothing else.** (a) **You** ground every element / attribute / ordering in the actual DTD / XSD / RNG while writing it (step 3) — that is the only correctness work you can do. (b) **The user** runs the live validation: confirming the content validates means *creating a file* from the template, which you can't do — file creation in Web Author needs a writable storage connector (Git / WebDAV / …) that only the user configures. So instruct the user to set up a connector, create a file from the template via the New File wizard, and manually confirm it opens with no validation errors and all `${...}` resolved (see `troubleshooting.md`). **There is no offline / command-line schema validator in scope. Never write or run a standalone program — Java/SAX, Python, Node, an `xmllint`-style tool, anything — and never fabricate a variable-substituted copy of the seed to feed one.** No `xmllint` on the box is expected, not a gap to fill.
6. Restart the kit fully (stop + start). `user-frameworks/` is scanned only at startup.
7. Verify in the browser via the wizard or `template-chooser.html`. If the template doesn't appear, go to `troubleshooting.md` before guessing.
8. If two iterations produce no progress, switch to `oxygen-docs` (start from the topics in `doc-references.md`).

## URL convention

Both `ug-waCustom` and `ug-editor` paths are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching the `.md` or giving the user a complete URL, and replace `.md` with `.html` for the citation link.
