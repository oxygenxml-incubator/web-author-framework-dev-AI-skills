# framework-style-changes — Documentation Index

Curated subset of the official oXygen manual focused on **Author-mode CSS**: extensions, vendor properties (`-oxy-*`), functions (`oxy_*`), form controls, pseudo-classes, content chains, and how a CSS gets wired to a framework. Read these via the `oxygen-docs` skill (fetches the `.md`); cite the `.html` URL in the response.

This index mirrors the tree under **CSS Support in Author Mode** in the Editor manual:

```
dg-css-support-in-author
└── dg-oXygen-css-extensions     ← the spine for this skill
    ├── builtin-css-selectors
    ├── dg-additional-custom-selectors
    ├── dg-css-additional-properties   ← every -oxy-* vendor property
    ├── dg-oxygen-css-functions        ← every oxy_* function
    ├── form-controls                  ← every oxy_* form control
    ├── dg-custom-css-pseudo-classes
    └── ch_advanced_styling_multiple_before_and_after_pseudo_elements
```

## Documentation base URL

All topics in this file are under the Editor user guide:

```
/doc/ug-editor/
```

These paths are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching `.md` or when giving users a complete URL. Replace `.md` with `.html` for the citation link you show to people.

## Spine pages — start here

- [CSS Support in Author Mode](/doc/ug-editor/topics/dg-css-support-in-author.md) — top-level entry. Lists everything below.
- [CSS Extensions](/doc/ug-editor/topics/dg-oXygen-css-extensions.md) — single most important page. Every `-oxy-*` and `oxy_*` page is a child of this one.
- [Standard W3C CSS Supported Features](/doc/ug-editor/topics/dg-standard-css-support.md) — what's actually implemented vs. spec.
- [CSS At-Rules](/doc/ug-editor/topics/dg-standard-css-at-rules.md) — `@media oxygen and (platform:webapp) { … }` lives here.

## Wiring CSS to a framework

- [Associating a CSS with an XML Document](/doc/ug-editor/topics/dg-css-stylesheet.md) — how documents pick up a stylesheet.
- [Specifying Media Types in the CSS](/doc/ug-editor/topics/dg-oxygen-media-type.md) — `@media oxygen` and the `(platform:…)` predicate.
- [Handling CSS Imports](/doc/ug-editor/topics/handling-css-imports.md) — `@import` resolution rules.
- [Configuring and Managing Multiple CSS Styles for a Framework](/doc/ug-editor/topics/selecting-combining-multiple-css-styles.md) — the Styles menu.
- [Customizing Colors and Styles for Rendering Profiling in Author Mode](/doc/ug-editor/topics/apply-styles.md) — profile-driven styling.
- [Specify Custom CSS Properties](/doc/ug-editor/topics/adding-custom-css-properties.md) — register custom property names so the validator stops flagging them.

## Selectors

- [Built-in CSS Selectors](/doc/ug-editor/topics/builtin-css-selectors.md) — selectors oXygen ships with.
- [Additional CSS Selectors](/doc/ug-editor/topics/dg-additional-custom-selectors.md) — oXygen-specific extension selectors.
- [Custom CSS Pseudo-classes](/doc/ug-editor/topics/dg-custom-css-pseudo-classes.md) — `:oxy-*` pseudo-classes.

## Vendor properties (`-oxy-*`)

Every page listed under [Additional CSS Properties](/doc/ug-editor/topics/dg-css-additional-properties.md):

- [Append / Prepend Content: `-oxy-append-content` / `-oxy-prepend-content`](/doc/ug-editor/topics/dg-oxygen-extension-properties.md)
- [Collapse Text: `-oxy-collapse-text`](/doc/ug-editor/topics/dg-visibility-css-extension.md)
- [Cyrillic Counters: `-oxy-lower-cyrillic`](/doc/ug-editor/topics/dg-list-style-type-css-extension.md)
- [Display Tag Markers: `-oxy-display-tags`](/doc/ug-editor/topics/dg-display-tags.md)
- [Editable: `-oxy-editable`](/doc/ug-editor/topics/dg-editable-css-extension.md)
- [Floating Toolbar: `-oxy-floating-toolbar`](/doc/ug-editor/topics/floating-toolbar-property.md)
- [Folding Elements: `-oxy-foldable` / `-oxy-folded` / `-oxy-not-foldable-child`](/doc/ug-editor/topics/dg-folding-elements.md)
- [Links: `-oxy-link`](/doc/ug-editor/topics/dg-link-elements.md)
- [Link Navigation: `-oxy-link-activation-trigger`](/doc/ug-editor/topics/oxy-link-activation-trigger.md)
- [Morph Elements: `-oxy-morph`](/doc/ug-editor/topics/dg-morph-css-extension.md)
- [Placeholders for Empty Elements: `-oxy-placeholder-content`](/doc/ug-editor/topics/dg-placeholder-css-extension.md)
- [Style Elements: `-oxy-style`](/doc/ug-editor/topics/dg-style-element-property.md)
- [Tags Color: `-oxy-tags-color`](/doc/ug-editor/topics/custom-colors-for-element-tags.md)

## Custom CSS functions (`oxy_*`)

Every page listed under [Custom CSS Functions](/doc/ug-editor/topics/dg-oxygen-css-functions.md):

- [Arithmetic Functions](/doc/ug-editor/topics/dg-css-arithmetic-functions.md)
- [Actions: `oxy_action()`](/doc/ug-editor/topics/dg-action-function.md)
- [Action Lists: `oxy_action_list()`](/doc/ug-editor/topics/dg-action-list-function.md)
- [Attributes Concatenation: `oxy_attributes()`](/doc/ug-editor/topics/dg-attributes-function.md)
- [Base URL: `oxy_base-uri()`](/doc/ug-editor/topics/dg-base-uri-function.md)
- [Capitalization: `oxy_capitalize()`](/doc/ug-editor/topics/dg-capitalize-function.md)
- [Compound Actions: `oxy_compound_action()`](/doc/ug-editor/topics/dg-compound-action-function.md)
- [Concatenation: `oxy_concat()`](/doc/ug-editor/topics/dg-concat-function.md)
- [Get Text: `oxy_getSomeText(text, length)`](/doc/ug-editor/topics/dg-getsometext-function.md)
- [Indexing: `oxy_indexof()`](/doc/ug-editor/topics/dg-index-of-function.md)
- [Label: `oxy_label()`](/doc/ug-editor/topics/dg-oxy-label-function.md)
- [Last Occurrence: `oxy_lastindexof()`](/doc/ug-editor/topics/dg-last-index-of-function.md)
- [Link Text: `oxy_link-text()`](/doc/ug-editor/topics/dg-oxy-link-text.md)
- [Local Name: `oxy_local-name()`](/doc/ug-editor/topics/dg-local-name-function.md)
- [Lowercase: `oxy_lowercase()`](/doc/ug-editor/topics/dg-lowercase-function.md)
- [Name: `oxy_name()`](/doc/ug-editor/topics/dg-name-function.md)
- [Parent URL: `oxy_parent-url()`](/doc/ug-editor/topics/dg-parent-url-function.md)
- [Replace: `oxy_replace()`](/doc/ug-editor/topics/dg-replace-function.md)
- [Substring of Text: `oxy_substring()`](/doc/ug-editor/topics/dg-substring-function.md)
- [Unescape URL Value: `oxy_unescapeURLValue(string)`](/doc/ug-editor/topics/dg-oxy-unescapeURLValue.md)
- [Unparsed Entity URI: `oxy_unparsed-entity-uri()`](/doc/ug-editor/topics/dg-unparsed-entity-uri-function.md)
- [Uppercase: `oxy_uppercase()`](/doc/ug-editor/topics/dg-uppercase-function.md)
- [URL: `oxy_url()`](/doc/ug-editor/topics/dg-url-function.md)
- [XPath: `oxy_xpath()`](/doc/ug-editor/topics/dg-xpath-function.md)

## Form controls

Master page: [Form Controls](/doc/ug-editor/topics/form-controls.md). Each control is a child:

- [Audio File Player: `oxy_audio`](/doc/ug-editor/topics/oxy-audio-form-control.md)
- [Browser: `oxy_browser`](/doc/ug-editor/topics/oxy-browser-form-control.md)
- [Button: `oxy_button`](/doc/ug-editor/topics/button-editor.md)
- [Button Group: `oxy_buttonGroup`](/doc/ug-editor/topics/button-group-editor.md)
- [Checkbox: `oxy_checkbox`](/doc/ug-editor/topics/check-box-editor.md)
- [Combo Box: `oxy_combobox`](/doc/ug-editor/topics/combo-box-editor.md)
- [Date Picker: `oxy_datePicker`](/doc/ug-editor/topics/date-picker-editor.md)
- [HTML Content: `oxy_htmlContent`](/doc/ug-editor/topics/html-content-form-control.md)
- [Pop-up: `oxy_popup`](/doc/ug-editor/topics/pop-up-editor.md)
- [Text Area: `oxy_textArea`](/doc/ug-editor/topics/dg-text-area-form-control.md)
- [Text Field: `oxy_textfield`](/doc/ug-editor/topics/text-field-editor.md)
- [URL Chooser: `oxy_urlChooser`](/doc/ug-editor/topics/url-chooser-editor.md)
- [Video Player: `oxy_video`](/doc/ug-editor/topics/oxy-video-form-control.md)

User-side counterpart (when the user-facing behavior is the question, not the CSS API): [Using Form Controls in Author Mode](/doc/ug-editor/topics/using-form-controls.md).

## Pseudo-elements and content chains

- [Using the `:before(n)` and `:after(n)` Pseudo-Elements](/doc/ug-editor/topics/ch_advanced_styling_multiple_before_and_after_pseudo_elements.md) — multi-`::before` / multi-`::after` chains, the foundation for putting form controls into content.

## XPath activation expressions (in actions, not strictly CSS — but adjacent)

`oxy:*` XPath functions used inside `xpath-activation-expressions` for actions, content completion, and conditional rendering:

- [Controlling Which Author Operations Get Executed Through XPath Expressions](/doc/ug-editor/topics/xpath-activation-expressions.md)
- [`oxy:allows-child-element()`](/doc/ug-editor/topics/oxy-allows-child-element.md)
- [`oxy:allows-global-element()`](/doc/ug-editor/topics/oxy-allows-global-element.md)
- [`oxy:current-selected-element()`](/doc/ug-editor/topics/oxy-current-selected-element.md)
- [`oxy:selected-elements()`](/doc/ug-editor/topics/oxy-selected-elements.md)
- [`oxy:is-required-element()`](/doc/ug-editor/topics/oxy-is-required-element.md)
- [`oxy:is-editable-element()`](/doc/ug-editor/topics/oxy-is-editable-element.md)
- [`oxy:platform()`](/doc/ug-editor/topics/oxy-platform.md)

## Diagnosis and tooling

- [CSS Inspector View](/doc/ug-editor/topics/author-css-inspector-view.md) — desktop-only, but the rule-resolution model it documents is the same in WA. Useful when "the rule isn't applying."
- [Debugging CSS Stylesheets](/doc/ug-editor/topics/debugging-css-stylesheets.md)
- [Validating CSS Stylesheets](/doc/ug-editor/topics/validating-css-stylesheets.md) — when your `custom.css` itself is rejected.

## How to read these pages

1. **Start at the spine:** [CSS Extensions](/doc/ug-editor/topics/dg-oXygen-css-extensions.md). It enumerates every extension surface; you can usually pick the right child page from one read.
2. **For a specific construct, jump straight to its child page** — the property pages are tight (one or two screens) and worth reading in full.
3. **Cite the `.html` URL** in your final response, but read the `.md`.
4. **If a page is silent on a corner case** — fall back to `oxy-css-reference.md` (grounded in shipped framework CSS) and to a real bundled CSS file under `<EXPANDED_WEBAPP_DIR>/frameworks/<base>/css/`. Bundled CSS is the most reliable ground truth.
5. **If a page covers a property the local reference omits** — read it. The local `oxy-css-reference.md` deliberately lists only properties demonstrated by bundled CSS examples; the docs page has the canonical list.
