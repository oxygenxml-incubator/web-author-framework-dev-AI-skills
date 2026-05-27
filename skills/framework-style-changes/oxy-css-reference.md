# oXygen CSS Extensions Reference

oXygen's Author / Web Author rendering engine extends CSS 2.1 with form controls (`oxy_combobox`, …), functions (`oxy_xpath`, …), vendor properties (`-oxy-morph`, …), and dynamic content chains in `::before` / `::after`.

For canonical property lists and full syntax, read the linked `.md` doc page via the `oxygen-docs` skill. Bundled framework CSS lives under `<EXPANDED_WEBAPP_DIR>/frameworks/{dita,docbook,xhtml,tei,json,…}/css/`.

---

## 1. Form controls

Used inside `content:` on `::before` / `::after`. They render as live editing widgets bound to attributes (or, less commonly, elements). Master doc: <https://www.oxygenxml.com/doc/ug-editor/topics/form-controls.md>.

| Control | Purpose | Doc |
|---|---|---|
| `oxy_combobox` | Dropdown; supports literal values, `oxy_xpath` dynamic values, `onChange` | [combo-box-editor](https://www.oxygenxml.com/doc/ug-editor/topics/combo-box-editor.md) |
| `oxy_textfield` | Single-line text input bound to an attribute | [text-field-editor](https://www.oxygenxml.com/doc/ug-editor/topics/text-field-editor.md) |
| `oxy_datePicker` | Date picker with `format` + `validateInput` | [date-picker-editor](https://www.oxygenxml.com/doc/ug-editor/topics/date-picker-editor.md) |
| `oxy_checkbox` | Boolean toggle with explicit `values` / `uncheckedValues` | [check-box-editor](https://www.oxygenxml.com/doc/ug-editor/topics/check-box-editor.md) |
| `oxy_editor` | Polymorphic editor; `type` ∈ `text`, `combo`, `urlChooser`, `check` | — |
| `oxy_button` | Button with `actionID` or inline `action, oxy_action(...)` | [button-editor](https://www.oxygenxml.com/doc/ug-editor/topics/button-editor.md) |
| `oxy_popup` | Dropdown menu with `values` + `labels` + `selectionMode` | [pop-up-editor](https://www.oxygenxml.com/doc/ug-editor/topics/pop-up-editor.md) |
| `oxy_label` | Non-editable text (`text` accepts literals, `attr(...)`, `oxy_concat`, `oxy_xpath`) | [dg-oxy-label-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-oxy-label-function.md) |

Representative shapes:

```css
oxy_combobox(edit, "@keyref", editable, false, columns, 15);
oxy_textfield(edit, '@title', width, 85%);
oxy_datePicker(edit, "@year", format, "yyyy", validateInput, false, columns, 12);
oxy_checkbox(edit, "@state", values, "yes", uncheckedValues, "no", labels, oxy_name());
oxy_editor(type, urlChooser, edit, "@href", width, 95%, fontInherit, true);
oxy_button(actionID, 'bold');
oxy_label(text, attr(title, string, 'No title'), styles, 'font-weight:bold;');
```

Inline action on a button — anchor `frameworks/dita/css/edit/alternate-map-edit-attributes-inplace.css:8-14`:

```css
oxy_button(transparent, true, action, oxy_action(
    name, 'Edit',
    operation, 'ro.sync.ecss.extensions.commons.operations.ChangePseudoClassesOperation',
    arg-setPseudoClassNames, '-oxy-edit'
), enableInReadOnlyContext, true);
```

**`oxy_popup` constraints** (renders as `<button class="popupSelContainer">`, not stylable from framework CSS):

- `color` accepts **named CSS colors only** (`teal`, `crimson`, …) or `inherit`; hex (`"#0F7B6C"`) silently drops the rule.
- No `background` / `border` properties — style via the function's own properties.
- **Empty-default trick**: leading space in `values` (e.g. `" , tip, warning"`) maps to a placeholder label when the bound attribute is missing. Used by the bundled codeblock language picker — anchor `frameworks/dita/css/core/-domain-pr-d.css:56-62`.

**`oxy_button` constraints** (verified in bundled `frameworks/**/*.css`):

- Real, recognized parameters: `actionID` / `action`, `transparent` (boolean), `color` (hex like `#59ACFF` or named like `navy` / `white` — both work, no name-only restriction), `fontInherit`, `showText`, `showIcon`, `name` (label override), `hoverPseudoclassName`, `enableInReadOnlyContext`, `actionContext`.
- **No `backgroundColor` parameter** — appears in zero bundled framework CSS. Passing it (or any other unknown key) makes the entire `oxy_button(...)` call silently fail and the button vanishes from its pseudo-element. To style the chrome around buttons, set `padding` / `border` / `background-color` / `font-size` on the parent pseudo (`:before` / `:after`), not on the button itself. Anchor for hex `color` usage: `frameworks/xhtml/css/dark-theme.css:64`.

---

## 2. Functions

Usable inside `content:`, inside form-control property values, and inside other functions. Master doc: <https://www.oxygenxml.com/doc/ug-editor/topics/dg-oxygen-css-functions.md>.

| Function | Returns | Doc |
|---|---|---|
| `oxy_xpath(expr)` | string (XPath 2.0; numeric / boolean coerced) | [dg-xpath-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-xpath-function.md) |
| `oxy_url(base, rel)` | resolved URL; supports `${framework}/` placeholder | [dg-url-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-url-function.md) |
| `oxy_base-uri()` | base URI of the edited document | [dg-base-uri-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-base-uri-function.md) |
| `oxy_unescapeURLValue(s)` | URL-decoded string | [dg-oxy-unescapeURLValue](https://www.oxygenxml.com/doc/ug-editor/topics/dg-oxy-unescapeURLValue.md) |
| `oxy_action(...)` | inline action handle; `operation` is FQN of `AuthorOperation`, custom params as `arg-<name>` | [dg-action-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-action-function.md) |
| `oxy_action_list(...)` | groups `oxy_action` results | [dg-action-list-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-action-list-function.md) |
| `oxy_concat(s1, s2, …)` | concatenated string | [dg-concat-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-concat-function.md) |
| `oxy_local-name()` / `oxy_name()` | local element name | [dg-name-function](https://www.oxygenxml.com/doc/ug-editor/topics/dg-name-function.md) |
| `oxy_capitalize(s)` | titlecased string | — |
| `oxy_replace(s, regex, repl[, isRegex])` | regex / literal replacement | — |

**Don't nest** `oxy_xpath` inside `oxy_xpath` — build the expression with `oxy_concat` and pass it once:

```css
values, oxy_xpath(oxy_concat('string-join(doc("',
                              oxy_url('${framework}/', 'xml/metadatas.xml'),
                              '")//otherMeta/@val,",")'))
```

`oxy_attributes`: not observed in bundled framework CSS — avoid until confirmed.

---

## 3. Vendor properties

Master doc: <https://www.oxygenxml.com/doc/ug-editor/topics/dg-css-additional-properties.md>.

| Property | Values | Effect |
|---|---|---|
| `display: -oxy-morph` | (display value) | Collapses element nesting; content reads inline |
| `-oxy-foldable` | `true` / `false` | Enables/disables fold triangle UI |
| `-oxy-editable` | `true` / `false` | Read-only when `false` |
| `-oxy-placeholder-content` | string | Text shown when element is empty |
| `-oxy-show-placeholder` | `always`, `default`, `inherit`, `no` | Visibility of placeholder text. `default` suppresses when `:before`/`:after` content exists. Deprecated unprefixed aliases `show-placeholder` / `placeholder-content` still work — prefer prefixed. [doc](https://www.oxygenxml.com/doc/ug-editor/topics/dg-placeholder-css-extension.md) |
| `-oxy-display-tags` | `full`, `partial`, `none` | Tag-display mode |

`-oxy-tags-visibility`, `::oxy-decoration`: not observed in bundled CSS — treat as legacy.

**Empty-element hint pattern** — anchor `frameworks/dita/css/hints/hints.css:95`:

```css
@media oxygen {
  task:empty {
    -oxy-show-placeholder: always;
    -oxy-placeholder-content: "Enter task content";
  }
}
```

Placeholder text is a CSS rendering, never persisted to XML. To scope hints to one template, put a marker attribute on the seed's root (e.g. `outputclass="faq"`) and use `[outputclass~="faq"]` in the selector.

---

## 4. Pseudo-elements and content chains

`::before` / `::after` accept a **numeric priority**: `:before(N)` / `:after(N)`. Multiple matching pseudo-elements with different priorities stack. Doc: <https://www.oxygenxml.com/doc/ug-editor/topics/ch_advanced_styling_multiple_before_and_after_pseudo_elements.md>.

`content:` may chain string literals, `oxy_*` functions, and form controls — anchor `frameworks/dita/css/core/-topic-specialization.css:36-44`:

```css
*[class~="topic/data"]:before(3)        { content: oxy_capitalize(oxy_name()) " "; }
*[class~="topic/data"][name]:before(2)  { content: oxy_textfield(edit, '@name', columns, 10); }
*[class~="topic/data"][value]:before(1) { content: " " oxy_textfield(edit, '@value', columns, 10); }
```

`::marker`: standard CSS list marker, no oXygen-specific behavior.

---

## 5. Common patterns

- **Attribute-driven labels** — chain `oxy_label(...)` + `oxy_textfield(edit, '@…')` in `content:`. Anchor `…/alternate-map-edit-attributes-inplace.css:127-128`.
- **Inline mixed content** — `display: -oxy-morph` on wrapper elements. Anchor `frameworks/docbook/css/elements.css:1484`.
- **Read-only regions** — `-oxy-editable: false`. Anchor `frameworks/dita/css/core/-domain-ut-d.css:290`.
- **Empty-element placeholders** — `-oxy-show-placeholder: always` + `-oxy-placeholder-content`. Anchor `frameworks/dita/css/hints/hints.css:41-42`.
- **Toolbar of buttons** — chain `oxy_button(actionID, '…')` in `:before { content: … }`. Anchor `frameworks/dita/css/floating_toolbar/topic.css:16`.
- **Foldable sections** — `-oxy-foldable: true|false`. Anchor `…/topic-content-mode.less:7`.

### Extending a base framework

When `mode = extend` (`.exf` with `base="DITA"` / `base="DocBook"` / …), your CSS lands on top of the base framework's full stylesheet. DITA elements inherit DITA-OT class hierarchies (e.g. `task/step` inherits from `topic/li`), so the base already sets `display`, counters, `list-style`, `:before` / `:after` content, etc.

1. Grep `frameworks/<base>/css/` for the element name and its DITA-OT class. Check `core/` (structural) and `hints/` (empty-state).
2. Read matching rules — bundled rules often use `!important`; matching is the only way to win.
3. The `:before(N)` priority syntax only overrides bundled `:before(N)` rules; it does **not** suppress list-item rendering. If a "looks like a `:before`" number won't go away, reset `display`, `list-style`, `counter-reset`, `counter-increment`, plus `:marker { content: none !important; }` — bundled template at `frameworks/dita/css/core/-task.css:209-219` (`task/stepsection`).

---

## 6. How to explore further

- `<EXPANDED_WEBAPP_DIR>/frameworks/dita/css/` — largest body of real `oxy_*` usage; start here for DITA questions.
- `<EXPANDED_WEBAPP_DIR>/frameworks/docbook/css/` — rich CALS-table examples.
- `<EXPANDED_WEBAPP_DIR>/frameworks/{xhtml,tei,json}/css/` — smaller, useful for cross-framework confirmation.
- `oxygen-docs` skill for canonical user-guide pages (search `oxy_` / `-oxy-` in the property/function indexes).
