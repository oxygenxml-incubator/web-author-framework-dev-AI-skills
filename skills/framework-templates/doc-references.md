# framework-templates — Documentation Index

Curated subset of the official oXygen manual focused on **document templates in the New File wizard**. Read these via the `oxygen-docs` skill (fetches the `.md`); cite the `.html` URL in the final response.

## Documentation base URLs

- **Editor / framework authoring (desktop + shared topics)** — `/doc/ug-editor/` (spine, `.exf`, custom editor variables, CSS placeholders, sharing).
- **Web Author customization** — `/doc/ug-waCustom/` (Web Author-specific editor variables; do not merge with `ug-editor`).

Both are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching `.md` or giving users a complete URL. Replace `.md` with `.html` for the citation link.

## Spine pages — start here

- [Customizing Document Templates](/doc/ug-editor/topics/customizing-templates.md) — **single most important page.** `displayName`, `filenamePrefix` / `filenameSuffix`, `smallIcon` / `bigIcon`, `type=dita|general`, the `<?oxy-placeholder?>` PI route for hints, i18n via `${i18n(tag)}`. Stable anchors:
  - `#create-properties-file` — icons.
  - `#add_a_prefix_or_suffix_to_file_names_for_a_custom` — filename prefix/suffix and `editor-variables` interaction.
  - `#configure_the_displayed_names_for_document_templa` — `displayName` and i18n.
  - `#adding_placeholders_or_hints_in_a_document_templa` — `<?oxy-placeholder?>` PI route + the "no whitespace inside the element" constraint.
- [Document Templates](/doc/ug-editor/topics/dg-file-templates.md) — developer-facing reference for the `templates/` folder layout inside a framework.
- [Templates Tab](/doc/ug-editor/topics/document-type-templates-tab.md) — GUI counterpart to `<documentTemplates>`. Useful sanity-check when the `.exf` reference is ambiguous.
- [New Document Wizard](/doc/ug-editor/topics/new-dialog-sa.md) — the only page that documents the wizard categories (Recently Used, Popular, New Document, Global Templates, Framework Templates). Read for the **Popular** category contract: `tags=popular` in a template's sibling `.properties` promotes it into Popular across frameworks. Bundled example: `frameworks/dita/templates/topic/Topic.properties`.

Skip these — UI-only, not relevant to authoring an `.exf`:

- [create-your-own-templates.md](/doc/ug-editor/topics/create-your-own-templates.md) — end-user UI workflow.
- [preferences-editor-document-templates.md](/doc/ug-editor/topics/preferences-editor-document-templates.md) — preferences dialog.

## `.exf` integration

- [Creating a Framework Using an Extension Script](/doc/ug-editor/topics/framework-customization-script.md) — `.exf` basics. Already loaded by `ai-framework-developer`.
- [Framework Extension Script File](/doc/ug-editor/topics/framework-customization-script-usecases.md) — canonical reference for every `.exf` element, including `<documentTemplates>` / `<addEntry>` / `inherit`.

## Editor variables in seed content

- [Editor Variables](/doc/ug-editor/topics/editor-variables.md) — authoritative list for desktop Author (`${id}`, `${caret}`, `${date(...)}`, `${user.name}`, …).
- [Editor Variables in Web Author](/doc/ug-waCustom/topics/webapp_editor_variables.md) — documented subset for Web Author. For grounded, tested expansion data specific to template seeds, prefer `editor-variables-web-author.md` in the `ai-framework-developer` skill.
- [Custom Editor Variables](/doc/ug-editor/topics/custom-editor-variables.md) and [Custom Editor Variables Preferences](/doc/ug-editor/topics/preferences-custom-editor-variables.md) — defining your own + the preferences UI.

## CSS-route placeholder hints (alternative to the PI route)

- [Placeholders for Empty Elements: `-oxy-placeholder-content`](/doc/ug-editor/topics/dg-placeholder-css-extension.md) — `-oxy-placeholder-content` / `-oxy-show-placeholder`. Pair with `framework-style-changes` for the `<addCss>` wiring.

## Sharing / promotion

- [Sharing a Framework](/doc/ug-editor/topics/author-document-type-extension-sharing.md) — promoting a session extension to a shared add-on.
- [Packing and Deploying Frameworks as Add-ons](/doc/ug-editor/topics/packing-and-deploying-addons.md) — package format.

## How to read these pages

1. **Label, prefix, icon, hint questions** → straight to [customizing-templates.md](/doc/ug-editor/topics/customizing-templates.md), jump to the relevant anchor.
2. **`<documentTemplates>` element shape** → [framework-customization-script-usecases.md](/doc/ug-editor/topics/framework-customization-script-usecases.md) is canonical; cross-check folder layout against [dg-file-templates.md](/doc/ug-editor/topics/dg-file-templates.md).
3. **Editor-variable expansion** → [editor-variables.md](/doc/ug-editor/topics/editor-variables.md) (desktop) or [webapp_editor_variables.md](/doc/ug-waCustom/topics/webapp_editor_variables.md) (Web Author). For WA template seeds specifically, `editor-variables-web-author.md` in `ai-framework-developer` has grounded tested data on what actually expands.
4. **Cite the `.html` URL** in the final response, but read the `.md`.
5. **If a page is silent on a corner case** (silent failure modes specific to user-frameworks loading) → fall back to `troubleshooting.md` here; it documents WA-specific behaviors not in the manual.
