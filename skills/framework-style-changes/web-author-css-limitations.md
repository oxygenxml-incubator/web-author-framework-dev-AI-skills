# Web Author CSS Limitations

Applies to **Oxygen XML Web Author only**, not Oxygen Desktop (Editor/Author). Source: `ug-waCustom/topics/webapp_css_limitations.md`.

## Selectors

- `+` (adjacent) and `>` (child) do **not** match table-related elements.
- Synthetic DOM nodes (`comment`, `reference`, `cdata`, `pi`, `error`) interfere with `+`.
- Not supported: `:nth-of-type`, `:nth-last-of-type`, `:first-of-type`, `:last-of-type`.
- `:focus`, `:focus-within` not supported.
- `:hover` only on mouse platforms; does not support `content`; cannot combine with Oxygen extension properties/functions or `attr()`.
- Subject selector and `:has` only supported when the rule contains only Oxygen extensions or `content`.
- Attribute selectors with wildcard attribute names not supported.
- `[*|lang]` (any-namespace) not supported; namespace prefix must match between XML and CSS.
- CSS entity selectors not supported.

## Properties

- `-oxy-style` not supported.
- `-oxy-tags-color`, `-oxy-tags-background-color` not supported.
- `-oxy-foldable` does not work on `display: inline`.
- `-oxy-floating-toolbar` only supports `oxy_button`, `oxy_combobox`, `oxy_label`, `oxy_buttonGroup`.
- `width` on inline elements not supported.
- `width`/`height` on non-root or `position: absolute|fixed` elements may show non-disableable resize handles in IE 11.
- `oxy_xpath` in property values is not refreshed on document changes (use `AuthorEditorAccess.refresh()` from Java).
- Oxygen extensions in length values are approximate; in media queries may misbehave.

## Media

- Oxygen CSS extensions are ignored on `print`. If used on `screen`, also applied to `print`.

## Rendering differences

- Web Author does not render non-`table-row` children of tables, nor non-`table-cell` children of `table-row`.
- Pseudo-elements render **inside** their parent (Desktop renders them as siblings). Affects `counter-reset` scope — use it on XML elements, not pseudo-elements.

## Form controls

- `oxy_label` width: long text wraps (Desktop ignores width).
- `columns` unit is `1em` in Web Author (Desktop uses width of "w").

## Workaround

Some limits can be bypassed via media queries — see `customizing_frameworks.md#ol_css_3h1_br`.
