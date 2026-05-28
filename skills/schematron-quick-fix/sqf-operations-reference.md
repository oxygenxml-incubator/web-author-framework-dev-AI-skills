# SQF Operations Reference

Attribute-level reference for the Schematron Quick Fix vocabulary. For the canonical attribute lists, defaults, and accepted values, **read the linked `.md` doc pages** via the `oxygen-docs` skill — the tables below cover what's actually needed when authoring, plus the Web Author-specific gotchas not in the manual.

Source pages (cite `.html`, read `.md`):

- [Defining Schematron Quick Fixes](https://www.oxygenxml.com/doc/ug-editor/topics/customizing-sqf.md)
- [Basic Schematron Quick Fix Operations](https://www.oxygenxml.com/doc/ug-editor/topics/sqf-operations.md)
- [User Entry SQF Operation](https://www.oxygenxml.com/doc/ug-editor/topics/user-entry-sqf-operation.md)
- [Restricting Quick Fix Operations](https://www.oxygenxml.com/doc/ug-editor/topics/use-when-sqf-condition.md)
- [Formatting/Indenting Content Inserted by SQF Operations](https://www.oxygenxml.com/doc/ug-editor/topics/format-indent-sqf-content.md)
- [SQF Specification (April 2015 Draft)](http://schematron-quickfix.github.io/sqf/publishing-snapshots/April2015Draft/spec/SQFSpec.html)

Required namespace on the schema root, plus `queryBinding="xslt2"` (SQF needs XPath 2.0+):

```xml
xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
```

## Structural elements

### `<sqf:fix>`

Defines a single Quick Fix. Full reference: `customizing-sqf.md`. Key attributes: `@id` (required, unique), `@use-when` (XPath predicate), `@use-for-each` (XPath sequence; produces one proposal per item with `$sqf:current` bound), `@role` (SQF-spec hint).

Children: `<sqf:description>` (first; required for a label), zero or more `<sqf:param>` / `<sqf:user-entry>`, then operation elements (`<sqf:add>` / `<sqf:delete>` / `<sqf:replace>` / `<sqf:stringReplace>`) **or** a single `<sqf:call-fix>` (must not mix with sibling operations). `<sch:let>` / `<sqf:copy-of>` may appear for intermediate computation.

### `<sqf:description>`

Contains `<sqf:title>` (required — proposal label) and zero or more `<sqf:p>` (tooltip paragraphs).

### `<sqf:group>` and `<sqf:fixes>`

`<sqf:group>` groups multiple `<sqf:fix>` so they can be referenced together. `<sqf:fixes>` is the top-level container for **global** fixes visible to any rule in the schema — use for shared libraries. Full reference: `customizing-sqf.md`.

### `<sqf:param>` and `<sqf:with-param>`

Parameters on a `<sqf:fix>`; the name becomes a `$name` XPath variable inside the fix body. `@abstract="true"` means the value must be supplied by a calling abstract pattern (and `@type` / default must then be omitted). `<sqf:with-param name="…" select="…"/>` passes a value via `<sqf:call-fix>`. Full reference: `customizing-sqf.md`.

### `<sqf:call-fix>`

Calls another fix (defined globally in `<sqf:fixes>` or in the same `<sch:rule>`). `@ref` points at the target ID. The calling fix **adopts** the called fix's operations; do not put other operation siblings next to `<sqf:call-fix>`.

### `<sqf:copy-of>`

Treated as `xsl:copy-of`. Copies the `@select` nodes into the current context (typically inside an operation body) for verbatim reproduction.

## The four basic operations

All four operations resolve their target through an **anchor**: if `@match` is set its XPath selects the anchor, otherwise the anchor is the enclosing `<sch:rule>`'s `@context`. Inside the operation body, the XPath default context is the anchor (with the documented exception for `<sqf:stringReplace>` — see below).

Full reference: `sqf-operations.md`. Attribute matrix at the bottom of this file.

### `<sqf:add>` — insert a node

Specific cases (from `sqf-operations.md`):

- **Element** — `node-type="element"` + `target="qname"`. If empty content and the element has a required child structure, **oXygen inserts the required content** for that element.
- **Attribute** — `node-type="attribute"` + `target="qname"`. Do not set `@position`.
- **Fragment** — omit `@node-type`. Content (or `@select`) must be well-formed XML.
- **Comment** — `node-type="comment"`. No `@target`.
- **PI** — `node-type="pi"` (or `processing-instruction`) + `target="piTarget"`.

`@position` is `first-child` (default) / `last-child` / `before` / `after`, relative to the anchor; ignored for attributes. QName prefixes on `@target` must be declared on the schema (e.g. `<sch:ns prefix="x" uri="…"/>`).

```xml
<sqf:fix id="addTitle">
  <sqf:description>
    <sqf:title>Insert title element.</sqf:title>
  </sqf:description>
  <sqf:add target="title" node-type="element">Title text</sqf:add>
</sqf:fix>
```

### `<sqf:delete>` — remove a node

`@match` selects the node(s) to delete; defaults to `.` (rule's context). Can match elements, attributes, text, comments, PIs.

```xml
<sqf:fix id="remove_lang">
  <sqf:description>
    <sqf:title>Remove "xml:lang" attribute</sqf:title>
  </sqf:description>
  <sqf:delete match="@xml:lang"/>
</sqf:fix>
```

### `<sqf:replace>` — replace nodes

Key attributes (see attribute matrix at bottom): `@match` (defaults to rule context), `@node-type` (`keep` / `element` / `attribute` / `pi` / `comment`), `@target` (QName of the replacement; required unless `node-type="comment"`), `@select` (alt to body content).

```xml
<sqf:fix id="resolvePh">
  <sqf:description>
    <sqf:title>Change the ph element into text</sqf:title>
  </sqf:description>
  <sqf:replace match="ph">
    <value-of select="."/>
  </sqf:replace>
</sqf:fix>
```

### `<sqf:stringReplace>` — patch a sub-string of text

Key attributes: `@match` (selects text nodes), `@regex`, `@flags`, `@select` (alt to body).

Engine gotchas (not all obvious from the docs):

- Regex is **Java regex**; the `j` flag (e.g. `flags=";j"` patterns in examples) switches to Saxon's native Java regex syntax, enabling `\b` etc. — see Saxonica's [`fn:matches`](https://www.saxonica.com/html/documentation/functions/fn/matches.html).
- "Dot matches all" is **always on** for SQF stringReplace, so `.` matches line terminators too.
- **Critical context gotcha:** inside `<sqf:stringReplace>` the XPath default context is the **whole text node**, not the matched sub-string. Plan `@select` accordingly.

```xml
<sqf:fix id="changeWord">
  <sqf:description>
    <sqf:title>Replace word with product</sqf:title>
  </sqf:description>
  <sqf:stringReplace regex="Oxygen" flags="i">
    <ph keyref="product"/>
  </sqf:stringReplace>
</sqf:fix>
```

## Advanced elements

### `<sqf:user-entry>` — prompt the user

`@name` becomes `$name` inside the fix body. `@default` is an XPath pre-populated in the dialog. Multiple `<sqf:user-entry>` elements produce a dialog per element in sequence. Full reference: `user-entry-sqf-operation.md`.

```xml
<sqf:fix id="editTitle">
  <sqf:description>
    <sqf:title>Edit the journal title</sqf:title>
  </sqf:description>
  <sqf:user-entry name="newTitle" default="@title">
    <sqf:description>
      <sqf:title>Edit the title:</sqf:title>
    </sqf:description>
  </sqf:user-entry>
  <sqf:replace match="@title" target="title" node-type="keep" select="$newTitle"/>
</sqf:fix>
```

### `@use-when` — gate a fix or operation

XPath predicate on `<sqf:fix>` or any operation. False → fix not offered (or operation skipped). Full reference: `use-when-sqf-condition.md`.

### `@use-for-each` + `$sqf:current` — one proposal per item

On `<sqf:fix>`, generates one Quick Fix proposal per item in the XPath sequence. `$sqf:current` is the current item, usable in title and operations.

```xml
<sch:let name="articleTypes" value="('abstract','addendum','announcement','article-commentary')"/>
…
<sqf:fix id="setArticleType" use-for-each="$articleTypes">
  <sqf:description>
    <sqf:title>Set article type to '<sch:value-of select="$sqf:current"/>'</sqf:title>
  </sqf:description>
  <sqf:replace node-type="attribute" target="article-type" select="$sqf:current"/>
</sqf:fix>
```

## Referencing fixes from `<assert>` / `<report>`

```xml
<sch:assert test="@id" sqf:fix="addId">…</sch:assert>          <!-- one fix -->
<sch:assert test="@id" sqf:fix="addId addIds">…</sch:assert>    <!-- two proposals shown -->
```

Only the namespace URI matters; the prefix is conventional. Declare `xmlns:sqf="http://www.schematron-quickfix.com/validator/process"` on the schema root.

## Formatting and whitespace

Source: `format-indent-sqf-content.md`. Inserted content is **automatically indented** unless you opt out:

- `<xsl:text>` inside the operation body — surgical whitespace control while keeping auto-indent elsewhere.
- `@xml:space="preserve"` on the operation element — disables auto-indent, preserves spacing as authored. Use for code blocks, `<pre>`-like content, or anywhere indentation is semantic.

## Attribute quick-reference matrix

| Attribute | `<sqf:add>` | `<sqf:delete>` | `<sqf:replace>` | `<sqf:stringReplace>` |
|---|---|---|---|---|
| `@match` | optional (anchor) | optional (defaults to `.`) | optional (defaults to `.`) | **required for text-node selection** |
| `@target` | required for non-comment | n/a | required unless `node-type="comment"` | n/a |
| `@node-type` | `element` / `attribute` / `comment` / `pi`; omit for fragment | n/a | `keep` / `element` / `attribute` / `comment` / `pi` | n/a |
| `@position` | `first-child` (default) / `last-child` / `before` / `after` | n/a | n/a | n/a |
| `@select` | yes (alt to body) | n/a | yes (alt to body) | yes (alt to body) |
| `@regex` / `@flags` | n/a | n/a | n/a | yes |
| `@xml:space` | yes (formatting) | n/a | yes (formatting) | yes (formatting) |
| `@use-when` | yes | yes | yes | yes |

## Failure modes

- **Fix not offered.** Check (1) SQF namespace declared on the schema root, (2) `queryBinding="xslt2"` set, (3) `@sqf:fix` ID matches a `<sqf:fix>/@id`, (4) the `.sch` is actually attached to the active validation scenario.
- **Fix offered but does nothing.** Usually missing `@target` for a non-comment operation, or `@match` selects nothing. `validating-sqf.md` catches both at edit time.
- **Insert fragment fails silently.** Fragment must be well-formed XML; if using `@select`, the XPath must return a node sequence.
- **stringReplace replaces too much.** Dot-matches-all is always on, and the operation context is the whole text node — not the matched sub-string.
- **Wrong indent after fix.** Switch to `xml:space="preserve"` or move whitespace into `<xsl:text>`.
