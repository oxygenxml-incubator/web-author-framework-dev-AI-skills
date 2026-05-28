# SQF Examples (Curated)

Working SQF patterns from the official oXygen User Guide — primarily [Examples of Schematron Rules and Quick Fixes](https://www.oxygenxml.com/doc/ug-editor/topics/examples-schematron-sqf-x.md), plus embedded examples in [Defining Schematron Quick Fixes](https://www.oxygenxml.com/doc/ug-editor/topics/customizing-sqf.md) and [Basic SQF Operations](https://www.oxygenxml.com/doc/ug-editor/topics/sqf-operations.md). Tweak XPath to match the user's vocabulary.

More patterns: [community samples repo](https://github.com/schematron-quickfix/sqf/tree/master/samples), [oXygen UG `rulesAdvanced.sch`](https://github.com/oxygenxml/userguide/blob/master/DITA/rules/rulesAdvanced.sch), `$OXYGEN_INSTALL_DIR/samples/schematron/`.

## Index

| # | Pattern | Operation(s) | Source |
|---|---|---|---|
| 1 | Insert missing `title` child | `<sqf:add>` element | `sqf-operations.md` |
| 2 | Delete forbidden attribute | `<sqf:delete>` | `sqf-operations.md` |
| 3 | Replace element with its text | `<sqf:replace>` | `sqf-operations.md` |
| 4 | Replace word in text via regex | `<sqf:stringReplace>` | `sqf-operations.md` |
| 5 | DITA `<prolog>` / `<critdates>` / `<revised>` chain | Three chained `<sqf:add>` across three rules | Use Case 1 |
| 6 | Add `@id` to a DITA `<section>` (current + all) | `<sqf:add>` (attribute) × 2 | Use Case 2 |
| 7 | Wrap a `<shortdesc>` inside `<abstract>` | `<sqf:replace>` + `<sqf:add>` + `<sqf:delete>` with `@use-when` | Use Case 3 |
| 8 | Enumerate allowed `@article-type` values | `<sqf:replace>` with `@use-for-each` + `$sqf:current` | Use Case 4 |
| 9 | Enforce CALS `@rowsep` / `@colsep` on `<colspec>` | Two `<sqf:add>` (attribute) | Use Case 5 |
| 10 | Move a DITA `<fig>` out of its parent `<p>` | `<sqf:add>` + `<sqf:delete>` | `sqf-implementing-framework.md` |
| 11 | User-supplied value for `@title` rewrite | `<sqf:user-entry>` + `<sqf:replace>` | `user-entry-sqf-operation.md` |
| 12 | Conditional fix gated by XPath | `@use-when` on `<sqf:fix>` | `use-when-sqf-condition.md` |

## 1. Insert missing element

```xml
<schema xmlns="http://purl.oclc.org/dsdl/schematron"
        xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
        queryBinding="xslt2">
  <pattern>
    <rule context="head">
      <assert test="title" sqf:fix="addTitle">title element missing.</assert>
      <sqf:fix id="addTitle">
        <sqf:description>
          <sqf:title>Insert title element.</sqf:title>
        </sqf:description>
        <sqf:add target="title" node-type="element">Title text</sqf:add>
      </sqf:fix>
    </rule>
  </pattern>
</schema>
```

## 2. Delete a forbidden attribute

```xml
<schema xmlns="http://purl.oclc.org/dsdl/schematron" queryBinding="xslt2"
        xmlns:sqf="http://www.schematron-quickfix.com/validator/process">
  <pattern>
    <rule context="*[@xml:lang]">
      <report test="@xml:lang" sqf:fix="remove_lang">
        The attribute "xml:lang" is forbidden.</report>
      <sqf:fix id="remove_lang">
        <sqf:description>
          <sqf:title>Remove "xml:lang" attribute</sqf:title>
        </sqf:description>
        <sqf:delete match="@xml:lang"/>
      </sqf:fix>
    </rule>
  </pattern>
</schema>
```

## 3. Replace element with its text

```xml
<schema xmlns="http://purl.oclc.org/dsdl/schematron"
        xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
        queryBinding="xslt2">
  <pattern>
    <rule context="title">
      <report test="exists(ph)" sqf:fix="resolvePh" role="warn">
        ph element is not allowed in title.</report>
      <sqf:fix id="resolvePh">
        <sqf:description>
          <sqf:title>Change the ph element into text</sqf:title>
        </sqf:description>
        <sqf:replace match="ph">
          <value-of select="."/>
        </sqf:replace>
      </sqf:fix>
    </rule>
  </pattern>
</schema>
```

## 4. Replace text via regex

```xml
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron"
            xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
            queryBinding="xslt2">
  <sch:pattern>
    <sch:rule context="text()">
      <sch:report test="matches(., 'Oxygen', 'i')" sqf:fix="changeWord">
        The oXygen word is not allowed</sch:report>
      <sqf:fix id="changeWord">
        <sqf:description>
          <sqf:title>Replace word with product</sqf:title>
        </sqf:description>
        <sqf:stringReplace regex="Oxygen" flags="i">
          <ph keyref="product"/>
        </sqf:stringReplace>
      </sqf:fix>
    </sch:rule>
  </sch:pattern>
</sch:schema>
```

## 5. DITA `<prolog>` / `<critdates>` / `<revised>` chain

Three separate `<sch:rule>`s, each with its own fix, so each missing layer resolves independently.

```xml
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron" queryBinding="xslt2"
            xmlns:sqf="http://www.schematron-quickfix.com/validator/process">
  <sch:pattern>
    <sch:rule context="*[contains(@class, ' topic/topic ')]">
      <sch:assert sqf:fix="add_prolog" test="prolog" role="warn">
        Every topic must contain prolog/critdates/revised elements where the revised
        modified date is in YYYY-MM-DD format.</sch:assert>
      <sqf:fix id="add_prolog">
        <sqf:description>
          <sqf:title>Add prolog/critdates/revised, with revised/@modified = current date (YYYY-MM-DD).</sqf:title>
        </sqf:description>
        <sqf:add match="*[contains(@class, ' topic/body ')]" node-type="element"
                 position="before" target="prolog">
          <critdates>
            <revised modified=""/>
          </critdates>
        </sqf:add>
      </sqf:fix>
    </sch:rule>

    <sch:rule context="*[contains(@class, ' topic/prolog ')]">
      <sch:report role="warn" test="not(critdates)" sqf:fix="add_critdates">
        The prolog element must have critdates/revised.</sch:report>
      <sqf:fix id="add_critdates">
        <sqf:description>
          <sqf:title>Add the critdates element.</sqf:title>
        </sqf:description>
        <sqf:add node-type="element" target="critdates">
          <revised modified=""/>
        </sqf:add>
      </sqf:fix>
    </sch:rule>

    <sch:rule context="*[contains(@class, ' topic/critdates ')]">
      <sch:report role="warn" test="not(revised)" sqf:fix="add_revised">
        The critdates element must have a revised child.</sch:report>
      <sqf:fix id="add_revised">
        <sqf:description>
          <sqf:title>Add the revised element.</sqf:title>
        </sqf:description>
        <sqf:add node-type="element" target="revised"/>
      </sqf:fix>
    </sch:rule>
  </sch:pattern>
</sch:schema>
```

## 6. Add `@id` to a DITA `<section>` (current + "fix all")

Two fixes offered (space-separated IDs in `@sqf:fix`): one for the current section, one for **all** sections (the `@match="//…"` idiom re-targets the operation document-wide).

```xml
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron"
            queryBinding="xslt2"
            xmlns:sqf="http://www.schematron-quickfix.com/validator/process">
  <sch:pattern>
    <sch:rule context="section">
      <sch:assert test="@id" sqf:fix="addId addIds">
        All sections should have an @id attribute</sch:assert>

      <sqf:fix id="addId">
        <sqf:description>
          <sqf:title>Add @id to the current section</sqf:title>
          <sqf:p>Generated from the section title; falls back to a random id.</sqf:p>
        </sqf:description>
        <sqf:add target="id" node-type="attribute"
          select="concat('section_',
            if (exists(title) and string-length(title) &gt; 0)
            then substring(lower-case(replace(replace(
                   normalize-space(string(title)), '\s', '_'),
                   '[^a-zA-Z0-9_]', '')), 0, 50)
            else generate-id())"/>
      </sqf:fix>

      <sqf:fix id="addIds">
        <sqf:description>
          <sqf:title>Add @id to all sections</sqf:title>
        </sqf:description>
        <sqf:add match="//section[not(@id)]" target="id" node-type="attribute"
          select="concat('section_',
            if (exists(title) and string-length(title) &gt; 0)
            then substring(lower-case(replace(replace(
                   normalize-space(string(title)), '\s', '_'),
                   '[^a-zA-Z0-9_]', '')), 0, 50)
            else generate-id())"/>
      </sqf:fix>
    </sch:rule>
  </sch:pattern>
</sch:schema>
```

## 7. Restructure into an `<abstract>` (complementary `@use-when`)

If no `<abstract>` exists, wrap. If one already exists, move the `<shortdesc>` into it.

```xml
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron" queryBinding="xslt2"
            xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
            xmlns:xsl="http://www.w3.org/1999/XSL/Transform">
  <sch:pattern>
    <sch:rule context="shortdesc">
      <sch:assert test="parent::abstract" sqf:fix="moveToAbstract moveToExistingAbstract">
        The short description must be added in an abstract element</sch:assert>

      <sch:let name="abstractElem"
               value="preceding-sibling::abstract | following-sibling::abstract"/>

      <sqf:fix id="moveToAbstract" use-when="not($abstractElem)">
        <sqf:description>
          <sqf:title>Move short description in an abstract element</sqf:title>
        </sqf:description>
        <sqf:replace>
          <abstract>
            <xsl:apply-templates mode="copyExceptClass" select="."/>
          </abstract>
        </sqf:replace>
      </sqf:fix>

      <sqf:fix id="moveToExistingAbstract" use-when="$abstractElem">
        <sqf:description>
          <sqf:title>Move short description in the existing abstract element</sqf:title>
        </sqf:description>
        <sch:let name="shortDesc">
          <xsl:apply-templates mode="copyExceptClass" select="."/>
        </sch:let>
        <sqf:add match="$abstractElem" select="$shortDesc"/>
        <sqf:delete/>
      </sqf:fix>
    </sch:rule>
  </sch:pattern>

  <xsl:template match="node() | @*" mode="copyExceptClass">
    <xsl:copy copy-namespaces="no">
      <xsl:apply-templates select="node() | @*" mode="copyExceptClass"/>
    </xsl:copy>
  </xsl:template>
  <xsl:template match="@class" mode="copyExceptClass"/>
</sch:schema>
```

## 8. Enumerate allowed attribute values

Generate one fix per allowed value automatically.

```xml
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron" queryBinding="xslt2"
            xmlns:sqf="http://www.schematron-quickfix.com/validator/process">
  <sch:let name="articleTypes"
           value="('abstract','addendum','announcement','article-commentary')"/>
  <sch:pattern>
    <sch:rule context="article/@article-type">
      <sch:assert test=". = $articleTypes" sqf:fix="setArticleType">
        Should be one of the article types: <sch:value-of select="$articleTypes"/></sch:assert>

      <sqf:fix id="setArticleType" use-for-each="$articleTypes">
        <sqf:description>
          <sqf:title>Set article type to '<sch:value-of select="$sqf:current"/>'</sqf:title>
        </sqf:description>
        <sqf:replace node-type="attribute" target="article-type" select="$sqf:current"/>
      </sqf:fix>
    </sch:rule>
  </sch:pattern>
</sch:schema>
```

## 9. Enforce CALS `@rowsep` / `@colsep`

```xml
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron" queryBinding="xslt2"
            xmlns:sqf="http://www.schematron-quickfix.com/validator/process">
  <sch:pattern>
    <sch:rule context="colspec">
      <sch:assert test="@rowsep = 1" sqf:fix="addRowsep">The @rowsep should be set to 1</sch:assert>
      <sch:assert test="@colsep = 1" sqf:fix="addColsep">The @colsep should be set to 1</sch:assert>

      <sqf:fix id="addRowsep">
        <sqf:description><sqf:title>Add @rowsep attribute</sqf:title></sqf:description>
        <sqf:add node-type="attribute" target="rowsep" select="'1'"/>
      </sqf:fix>

      <sqf:fix id="addColsep">
        <sqf:description><sqf:title>Add @colsep attribute</sqf:title></sqf:description>
        <sqf:add node-type="attribute" target="colsep" select="'1'"/>
      </sqf:fix>
    </sch:rule>
  </sch:pattern>
</sch:schema>
```

## 10. Move a child node out of its parent (canonical "move DITA `<fig>` out of `<p>`")

```xml
<schema xmlns="http://purl.oclc.org/dsdl/schematron"
        xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
        queryBinding="xslt2">
  <pattern id="check.figure.location">
    <rule context="p/fig">
      <report test="true()" role="warn" sqf:fix="moveAfter">
        A figure inside a paragraph doesn't transform well into PDF.</report>
      <sqf:fix id="moveAfter">
        <sqf:description>
          <sqf:title>Move after the paragraph.</sqf:title>
        </sqf:description>
        <let name="figToMove" value="."/>
        <sqf:add match="parent::p" select="$figToMove" position="after"/>
        <sqf:delete match="."/>
      </sqf:fix>
    </rule>
  </pattern>
</schema>
```

## 11. User-supplied value via `<sqf:user-entry>`

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

## 12. Conditional fix via `@use-when`

```xml
<sqf:fix id="last" use-when="$colWidthSummarized - 100 lt $lastWidth" role="replace">
  <sqf:description>
    <sqf:title>Subtract excessive width from the last element.</sqf:title>
  </sqf:description>
  <let name="delta" value="$colWidthSummarized - 100"/>
  <sqf:add match="html:col[last()]" target="width" node-type="attribute">
    <let name="newWidth" value="number(substring-before(@width,'%')) - $delta"/>
    <value-of select="concat($newWidth,'%')"/>
  </sqf:add>
</sqf:fix>
```

## Patterns to memorize

- **Multiple fixes per assert** — `sqf:fix="id1 id2"`, define both `<sqf:fix>` siblings.
- **"Fix current" vs "fix all"** — second copy overrides `@match` with a document-wide XPath.
- **Move-node idiom** — `<sqf:add match="parent::…" select="." position="after"/>` + `<sqf:delete/>`.
- **Enum picker** — `@use-for-each="$allowedValues"` + `$sqf:current` in title and `@select`.
- **Conditional branches** — complementary `@use-when` on sibling fixes, not branching inside one fix.
- **Auto-content insertion** — `<sqf:add>` of an element with required children lets oXygen fill them in automatically.
