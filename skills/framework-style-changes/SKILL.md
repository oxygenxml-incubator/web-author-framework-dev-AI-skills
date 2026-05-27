---
name: framework-style-changes
description: Use when changing Author-mode rendering in oXygen / Web Author — element styling, form controls (`oxy_combobox`, `oxy_textfield`, `oxy_popup`, `oxy_button`, `oxy_datePicker`, `oxy_checkbox`, `oxy_label`, `oxy_editor`), CSS functions (`oxy_xpath`, `oxy_action`, `oxy_url`, `oxy_concat`, `oxy_name`, `oxy_capitalize`, …), vendor properties (`-oxy-morph`, `-oxy-foldable`, `-oxy-editable`, `-oxy-placeholder-content`, `-oxy-show-placeholder`, `-oxy-display-tags`), priority pseudo-elements (`:before(N)` / `:after(N)`), `@media oxygen` rules, or Web Author-specific CSS limitations. Routed to from `ai-framework-developer`; for canonical doc lookups defer to `oxygen-docs`.
---

# Framework Style Changes

Use this skill for Author-mode CSS changes in Web Author.

## References

- Grounded CSS reference (form controls, functions, vendor props, pseudo-elements, WA gotchas, patterns) — `oxy-css-reference.md`
- Web Author-only CSS limitations (selectors, properties, media, rendering) — `web-author-css-limitations.md`
- Author-mode operations reference (pseudo-class control, attribute updates, insert/replace, action composition) — `author-mode-operations-reference.md`
- Adding a Content Completion / external author action (two-file pattern, kit examples) — `content-completion-actions.md`
- Curated docs index for CSS extensions — `doc-references.md`
- For any pure documentation lookup not covered above — `oxygen-docs` skill (fetches the `.md` from the official manual)
- `.exf` shape (where `<addCss>` lives) — `ai-framework-developer` (`exf-structure.md`)
- Browser verification (CSS not rendering, console errors, screenshot before/after) — `chrome-mcp-usage.md` in the `ai-framework-developer` skill

## Test document placement and URL

- Web Author blocks `file://` URLs by default. Do not try to bypass this.
- Keep the canonical `test-document.xml` in the session directory under `USER_FRAMEWORKS_DIR` so the framework change and sample document stay together.
- Also copy the document into `<SAMPLES_CONTENT_DIR>/dita/<unique-name>.xml` (or matching subdir like `docbook`, `xhtml`, etc., based on framework). Reuse the existing samples tree; never create a parallel samples content root.
- Open the document in Web Author at:
  - `http://localhost:<PORT>/oxygen-xml-web-author/app/oxygen.html?url=samples%3A%2F%2Fsamples%2Fdita%2F<unique-name>.xml`
  - Decoded: `samples://samples/dita/<unique-name>.xml`. The double `samples/` is expected — connector scheme is `samples://` and its content root is also named `samples/`.
  - `<PORT>` comes from `<KIT_DIR>/tomcat/conf/server.xml`; do not assume `8080` (see `ai-framework-developer` rules).
- Confirm the exact pattern once per kit from the dashboard **Samples** tab by inspecting the `?url=` of any sample tile.

## Required flow

1. Confirm whether the task is `extend` or `new`.
2. Read `oxy-css-reference.md` before introducing any `oxy_*` / `-oxy-*` construct. For Web Author specifically, also scan `web-author-css-limitations.md` so you don't ship a selector or property that's silently dropped in WA.
3. Keep all edits in user extension paths under `USER_FRAMEWORKS_DIR`; never touch `BUNDLED_FRAMEWORKS_DIR`.
4. Place the test document per the rules above before browser verification.
5. Restart the kit per the `ai-framework-developer` rules (full stop+start; verify the port stops responding before starting again — a half-stopped Tomcat will silently no-op the next start).
6. Verify in browser:
   - (a) The custom CSS is loaded (look for the `<addCss>` `path` in the page source / network tab).
   - (b) The expected rules win precedence (use the Author CSS inspector reasoning: bundled `!important` rules in `frameworks/<base>/css/core/` and `actions/actions.css` often need matching `!important` in your override).
   - (c) UI sanity check — note any rendering issues (wrong layout, missing widget, console errors).
7. If behavior is unclear after two iterations, switch to `oxygen-docs` for the relevant property / function page before guessing further.

## URL convention

Both `ug-waCustom` and `ug-editor` paths are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching the `.md` or giving the user a complete URL, and replace `.md` with `.html` for the citation link.
