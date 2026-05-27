# Content Completion Actions

How to add a custom action that shows up in Web Author's Content Completion popup (and optionally in toolbars/menus). Two files, no Java.

Content Completion items are sorted **alphabetically by default** (by the label shown in the popup). Custom actions use the action `<name>` (and optional `alias` on `<addAction>`) in that same sort order alongside schema-driven proposals.

## The two files

1. **External author action XML** — `<framework>_externalAuthorActions/<id>.xml`. Filename stem matches the `id` attribute. Defines the display name, the XPath context where it's offered, and the operation(s) it runs.
2. **`.exf` registration** — `<author><contentCompletion><authorActions><addAction id="..."/></authorActions></contentCompletion></author>`. Wires the action into the framework.

## Minimal example

External action — `dita-customization_externalAuthorActions/insert.note.xml`:

```xml
<a:authorAction xmlns:a="http://www.oxygenxml.com/ns/author/external-action" id="insert.note">
  <a:name>Insert note</a:name>
  <a:description>Inserts a &lt;note&gt; element.</a:description>
  <a:operations>
    <a:operation id="op1">
      <a:xpathCondition>oxy:allows-child-element('note')</a:xpathCondition>
      <a:invoke ID="InsertFragmentOperation">
        <a:arguments>
          <a:argument name="fragment"><![CDATA[<note><?caret?></note>]]></a:argument>
          <a:argument name="insertLocation">.</a:argument>
          <a:argument name="insertPosition">Inside</a:argument>
        </a:arguments>
      </a:invoke>
    </a:operation>
  </a:operations>
</a:authorAction>
```

`.exf` snippet:

```xml
<author>
  <contentCompletion>
    <authorActions>
      <addAction id="insert.note" inCCWindow="true" inMenus="true"/>
    </authorActions>
  </contentCompletion>
</author>
```

- `inCCWindow="true"` → shown in the CC popup.
- `inMenus="true"` → also exposed to toolbars / context menus.
- `alias="..."` (optional) → extra label searched when typing in CC.

## Where to look in the kit

The bundled DITA framework ships dozens of real examples — read these before writing your own; they cover the typical `xpathCondition` / `InsertFragmentOperation` / `ChangeAttributeOperation` patterns:

- `<EXPANDED_WEBAPP_DIR>/frameworks/dita/dita-lw_externalAuthorActions/` — e.g. `section.xml`, `note.xml`, `paragraph.xml`, `insert.table2.xml`.
- `<EXPANDED_WEBAPP_DIR>/frameworks/dita/dita-lw.exf` — see the `<addAction>` entries inside `<author><contentCompletion>`.

The `samples/` folder in `oxygen-docs` also has trimmed-down copies (`samples/actions/insert.section.xml`, `samples/actions/insert.table.xml`, etc.) suitable for diffing against.

## Documentation

Read these via the `oxygen-docs` skill (cite the `.html`, read the `.md`). Paths below are site-root-relative; prepend `https://www.oxygenxml.com` for fetch or a full URL.

**Web Author**

- [Configuring Content Completion in Web Author](https://www.oxygenxml.com/doc/ug-waCustom/topics/wa-cc-configuration.html) — [`/doc/ug-waCustom/topics/wa-cc-configuration.md`](/doc/ug-waCustom/topics/wa-cc-configuration.md) — How to customize the CC assistant in Web Author: Document Type dialog (add/remove actions, JavaScript stub actions), `cc_config.xml` in the framework `resources` folder, JS `filterCCItems`, invalid-element insertion behavior, and related options.
- [Customizing the elements order in CC](https://www.oxygenxml.com/doc/ug-waCustom/topics/wa-cc-configuration.html#wa-cc-configuration__section_jkl_sgf_lhb) — [`/doc/ug-waCustom/topics/wa-cc-configuration.md#wa-cc-configuration__section_jkl_sgf_lhb`](/doc/ug-waCustom/topics/wa-cc-configuration.md#wa-cc-configuration__section_jkl_sgf_lhb) — Official way to change proposal order: implement `ContentCompletionSortPriorityAssigner` and raise priority values (Java extension API).

**Editor (`cc_config.xml` and schema-driven proposals)**

- [Customizing the Content Completion Assistant Using a Configuration File](https://www.oxygenxml.com/doc/ug-editor/topics/customize-content-completion.html) — [`/doc/ug-editor/topics/customize-content-completion.md`](/doc/ug-editor/topics/customize-content-completion.md) — Where to put `cc_config.xml` / `cc_config_ext.xml`, classpath ordering when extending a framework, and how file-based rules relate to the GUI Content Completion tab.
- [Configuring the Proposals for Elements and Attributes](https://www.oxygenxml.com/doc/ug-editor/topics/configure-elements-attr-cc-individually.html) — [`/doc/ug-editor/topics/configure-elements-attr-cc-individually.md`](/doc/ug-editor/topics/configure-elements-attr-cc-individually.md) — `elementProposals`: limit or auto-insert child elements and attributes per context (`path`, `insertElements`, `possibleElements`, `rejectElements`, `merge`); only schema-allowed names can be offered.
- [Configuring the Proposals for Attribute and Element Values](https://www.oxygenxml.com/doc/ug-editor/topics/configuring-content-completion-proposals.html) — [`/doc/ug-editor/topics/configuring-content-completion-proposals.md`](/doc/ug-editor/topics/configuring-content-completion-proposals.md) — `valueProposals`: fixed lists or XSLT-generated values for attributes/element text; `append` / `replace` / `addIfEmpty`; affects completion only, not validation.

**External author actions (this how-to)**

- [Content Completion subtab](https://www.oxygenxml.com/doc/ug-editor/topics/the-content-completion-tab.html) — [`/doc/ug-editor/topics/the-content-completion-tab.md`](/doc/ug-editor/topics/the-content-completion-tab.md) — Desktop Document Type UI equivalent of `<addAction>`: which actions appear in CC, Elements view, or insert menus; display name; replace a schema element with an action; filter schema proposals from CC.
- [Creating and Customizing Author Mode Actions for a Framework](https://www.oxygenxml.com/doc/ug-editor/topics/dg-create-custom-actions.html) — [`/doc/ug-editor/topics/dg-create-custom-actions.md`](/doc/ug-editor/topics/dg-create-custom-actions.md) — External action XML files (`*_externalAuthorActions/`), export from the Actions subtab, storage path rules, and how to hook actions into toolbars/menus/CC.
- [Controlling Which Author Operations Get Executed Through XPath Expressions](https://www.oxygenxml.com/doc/ug-editor/topics/xpath-activation-expressions.html) — [`/doc/ug-editor/topics/xpath-activation-expressions.md`](/doc/ug-editor/topics/xpath-activation-expressions.md) — Per-operation `<xpathCondition>` (XPath 2.0); first matching mode runs; documents `oxy:allows-child-element()` and related extension functions used in external actions.

Schema for the action XML: `oxygen-docs/schemas/authorAction.xsd`. `cc_config.xml` filter schema: `oxygen-docs/schemas/ccConfigSchemaFilter.xsd`.
