# CLAUDE.md

## Grounding rule

Anything claimed about Oxygen / Web Author behavior — selectors, `oxy_*` syntax, `.exf` shape, log messages, kit paths, port defaults — must cite the documentation, a skill, a real file in a checked-out frameworks tree or a real log line. Do not invent syntax or paths. If a construct is unverified, mark it explicitly ("not observed in bundled frameworks"). The whole repo's value is that it's grounded; speculative content erodes that.

## Entry point for framework work (required)

**`ai-framework-developer` is the entry point for ALL oXygen / Web Author framework questions — including pure documentation lookups.** Load it first, every time, even when the request looks like "just a docs question" (e.g. "which editor variables are supported in templates?", "what does `-oxy-editable` do?", "how does `.exf` validation work?"). The entry-point skill routes to the right topic skill (`framework-templates`, `framework-style-changes`, `oxygen-docs`, `schematron-quick-fix`, etc.), and those topic skills frequently contain verified Web Author-specific behavior that contradicts or refines the official manual. Skipping the entry point and going straight to `oxygen-docs` (or worse, web search) produces answers that miss the project's own grounded knowledge.

Rule of thumb: if the question mentions Oxygen, Web Author, frameworks, `.exf`, templates, CSS in Author mode, Schematron, validation, or any `oxy_*` / `${...}` syntax — start with `ai-framework-developer`, then follow its routing.

## Documentation lookups

For any question whose answer lives in the official Oxygen manuals — Web Author customization, Author-mode CSS, form controls, `.exf` packaging, validation, document templates, deployment, configuration, etc. — use the `oxygen-docs` skill **before** reaching for web search or rendered `.html` doc pages (but only after `ai-framework-developer` has routed you there, per the rule above). The skill fetches `llms.txt` TOCs and per-topic `.md` pages from `oxygenxml.com/doc/ug-waCustom` and `/ug-editor`; that path is always cheaper, more accurate, and more citable than a search-engine result or a rendered `.html` page. Cite the corresponding `.html` URL in the response, but read the `.md`.

## Restarting Web Author

To restart a Web Author kit:

1. Read the active HTTP connector port from `<KIT_DIR>/tomcat/conf/server.xml` (do not assume `8080`).
2. Probe `http://localhost:<PORT>/oxygen-xml-web-author/app/oxygen.html` (treat `200/302/401` as "running"); if running, run the kit's stop script and poll the port until it stops responding.
3. Launch the kit's start script **detached** — do not call it inline. The vendor `start oXygen XML Web Author.bat` ends with `pause` and will hang the caller. On Windows, wrap it in `Start-Process cmd.exe /c "<start.bat>"` (or equivalent) so the trailing pause stays inside the spawned window.
4. Poll the same probe URL until it answers `200/302/401`.

Not every change needs a restart. A full stop + start is **always** required when changing the `.exf` itself or the `user-frameworks/` structure/config — adding/removing CSS or template references, registering/unregistering templates, etc. (that tree is scanned at startup only). But a **content-only** edit to an already-referenced CSS or template file does **not** need a restart: Web Author re-reads the file from disk on document reopen / page refresh. Because the browser caches CSS, hard-reload the page with cache disabled (Chrome DevTools → Disable cache) to pick up the new content. For fast CSS iteration, reload instead of restarting each time. When a change's effect can't be observed directly, a full restart + checking the logs is the fastest, most reliable way to confirm it took effect.

