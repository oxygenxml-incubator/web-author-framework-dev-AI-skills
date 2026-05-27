---
name: oxygen-docs
description: FIRST source for oXygen / Web Author documentation questions. Use for framework extensions, Author-mode CSS, form controls, `.exf` packaging, validation, templates, deployment, configuration, and troubleshooting. Fetches official `.md` topic pages from `oxygenxml.com/doc/ug-waCustom` and `/ug-editor`; never use web search or `.html` rendering for these.
---

# oxygen-docs

Routed to from `ai-framework-developer`. Fetch official oXygen manual pages as plain Markdown and cite the matching `.html` URL.

## References

- `documentation-index.md` — curated TOC of the official `ug-editor` manual, grouped by topic (framework extension scripts, Author-mode CSS, form controls, content completion, scenarios, templates, catalogs, localization, sharing).
- `exf-reference.md` — `.exf` and external author-action structure summary, anchored to the local XSD/Schematron files in `schemas/` and the worked examples in `samples/`.
- `blog-references.md` — supplementary blog posts with practical customization patterns.
- `schemas/` — authoritative `frameworkExtensionScript.xsd`, `authorAction.xsd`, `ccConfigSchemaFilter.xsd` and the matching Schematron rules. Consult before generating `.exf` / action / `cc_config.xml` content.
- `samples/` — real `.exf`, author action XML, and CSS files used as grounded examples.

## Required flow

1. Identify the topic. If it concerns `.exf` shape or external author actions, start with `exf-reference.md` and the matching file under `schemas/` / `samples/`.
2. Find the page in `documentation-index.md`. If nothing fits, fetch the TOC directly:
   - `https://www.oxygenxml.com/doc/ug-waCustom/llms.txt` (Web Author customization)
   - `https://www.oxygenxml.com/doc/ug-editor/llms.txt` (Editor / Author)
3. Read the topic as `.md` (replace `.html` → `.md` in the URL). Drill into child pages when the parent is too terse.
4. For practical examples, check `blog-references.md`.
5. Respond with the answer plus the matching `.html` URL(s). For CSS, check both standard W3C and the **CSS Extensions** sub-tree. For actions, check both declarative actions and Java extensibility.

## Guardrails

- Never web-search for oXygen docs; never scrape `.html` for extraction — read `.md`.
- Do not invent topic URLs; resolve them from `llms.txt` or from the local references.
- If the docs are silent on a corner case, say so and fall back to grounded local evidence (bundled framework files under `<EXPANDED_WEBAPP_DIR>/frameworks/`, `samples/`, `schemas/`).
- Ignore the `webapp-add-framework` topic — it covers manual uploads, which this project does not use.

## URL convention

Both `ug-waCustom` and `ug-editor` paths are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching the `.md` or giving the user a complete URL, and replace `.md` with `.html` for the citation link.
