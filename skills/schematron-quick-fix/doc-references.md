# schematron-quick-fix — Documentation Index

Curated subset of the official oXygen User Guide focused on **Schematron Quick Fixes**. Read these via the `oxygen-docs` skill (fetches `.md`); cite the matching `.html` URL in answers.

Base: `https://www.oxygenxml.com/doc/ug-editor/` — SQF is a desktop-first authoring feature documented under the Editor UG. Web Author may differ in subtle ways (see "Web Author caveat" at the bottom).

## Spine — start here

- [Editing Schematron Quick Fixes](/doc/ug-editor/topics/editing-schematron-quick-fixes.md) — top-level page / sitemap.
- [Defining Schematron Quick Fixes](/doc/ug-editor/topics/customizing-sqf.md) — **canonical definition** of `<sqf:fix>` structure and every supported element (`<sqf:user-entry>`, `<sqf:call-fix>`, `<sqf:group>`, `<sqf:fixes>`, `<sqf:copy-of>`, `<sqf:param>`).
- [Basic Schematron Quick Fix Operations](/doc/ug-editor/topics/sqf-operations.md) — `<sqf:add>`, `<sqf:delete>`, `<sqf:replace>`, `<sqf:stringReplace>` with attributes and inline examples.
- [Examples of Schematron Rules and Quick Fixes](/doc/ug-editor/topics/examples-schematron-sqf-x.md) — the richest source of pattern recipes; mirrored locally in `sqf-examples.md`.

## Operations and modifiers

- [User Entry SQF Operation](/doc/ug-editor/topics/user-entry-sqf-operation.md) — `<sqf:user-entry>` with `@name` / `@default`.
- [Restricting Quick Fix Operations](/doc/ug-editor/topics/use-when-sqf-condition.md) — `@use-when` for conditional fixes/operations.
- [Formatting/Indenting Content Inserted by SQF Operations](/doc/ug-editor/topics/format-indent-sqf-content.md) — auto-indent and the `@xml:space="preserve"` / `<xsl:text>` opt-outs.
- [Executing SQF in Other Documents](/doc/ug-editor/topics/executing-sqf-in-other-docs.md) — `@match` patterns targeting nodes outside the current document.

## Integration and shipping

- [Integrating SQF in a Framework](/doc/ug-editor/topics/sqf-implementing-framework.md) — canonical end-to-end recipe. Pair with this skill's `framework-integration.md` for the WA-specific path.
- [Validating Schematron Quick Fixes](/doc/ug-editor/topics/validating-sqf.md) — **first thing to do when "the fix doesn't appear"**.
- [Configuring Validation Scenarios for a Framework](/doc/ug-editor/topics/dg-validation-scenarios.md) — dialog that produces `.scenarios` exports.
- [Associating a Schema to XML Documents](/doc/ug-editor/topics/associate-schema-to-document.md) — **schema-detection order** for validation: (1) scenario associated with the document, (2) default scenario from the framework, (3) schema declared directly in the document (`<?xml-model?>` PI, `xsi:schemaLocation`, `DOCTYPE`), (4) framework Schema-tab default. Explains why a framework-shipped fix sometimes doesn't fire for a specific document.
- [Associating a Schema in Validation Scenarios Defined in the Document Type](/doc/ug-editor/topics/associate-schema-framework-validation.md) — how `validationUnit` references resolve.
- [Associating a Schema Directly in XML Documents](/doc/ug-editor/topics/associating-schema-directly.md) — the `<?xml-model?>` PI route (useful for one-off demos with no framework).
- [Sharing a Framework](/doc/ug-editor/topics/author-document-type-extension-sharing.md) — distribution options.
- [Packing and Deploying Frameworks as Add-ons](/doc/ug-editor/topics/packing-and-deploying-addons.md) — add-on packaging.

## Embedding and editor support

- [Embedding SQF in Relax NG or XML Schema](/doc/ug-editor/topics/embed-sqf-in-rng-xsd.md) — pair with this skill's `embedding-sqf.md`.
- [Embedding Schematron Rules in XML Schema or RELAX NG](/doc/ug-editor/topics/combined_RNG_and_SCH.md) — broader topic for RNG-compact / annotation form.
- [Localizing SQF Messages](/doc/ug-editor/topics/localizing-sqf-messages.md) — `${i18n(tag)}` in titles and descriptions.
- Editor-only helpers: [Content Completion in SQF](/doc/ug-editor/topics/content_completion_sqf.md), [Highlight Quick Fix Occurrences](/doc/ug-editor/topics/highlight-qf-occurences.md), [Search and Refactor in SQF](/doc/ug-editor/topics/search-and-refactor-sqf.md).

## Specification and external samples

- [SQF Specification — April 2015 Draft](http://schematron-quickfix.github.io/sqf/publishing-snapshots/April2015Draft/spec/SQFSpec.html) — authoritative on the SQF *language* (oXygen implements this draft). Use for edge cases like operation ordering and scope semantics.
- [Public sample SQF Quick Fixes — `schematron-quickfix/sqf/samples`](https://github.com/schematron-quickfix/sqf/tree/master/samples) — community examples.
- [oXygen User Guide DITA `rulesAdvanced.sch`](https://github.com/oxygenxml/userguide/blob/master/DITA/rules/rulesAdvanced.sch) — large real-world `.sch` with production patterns.
- [Oxygen XML Blog: Schematron Checks to Help Technical Writing](https://blog.oxygenxml.com/topics/SchematronBCs.html).

## Reading strategy

1. **"What's the right operation?"** — `sqf-operations.md`, then `customizing-sqf.md` for advanced elements.
2. **"How do I express X?"** — `examples-schematron-sqf-x.md`, then this skill's `sqf-examples.md`, then the community samples repo.
3. **"How do I ship it in a framework?"** — `sqf-implementing-framework.md` for Desktop dialog flow, this skill's `framework-integration.md` for the file-based / Web Author flow.
4. **"Why doesn't my fix appear?"** — `validating-sqf.md` first (open `.sch`, run validation), then this skill's `framework-integration.md` "Common failure modes" table.
5. **Cite the `.html` URL** in the final response; read the `.md`.

## Web Author caveat

The pages above live under `/doc/ug-editor/` — they describe **Desktop** behavior. The Web Author customization manual (`/doc/ug-waCustom/`) has no dedicated SQF topic at the time of writing. SQF works in WA when the rules are loaded as part of a framework's validation scenario, but specific UI affordances (where the lightbulb / proposal popup appears, keyboard shortcuts) may differ. **Verify visually with `chrome-mcp-usage.md` (in the `ai-framework-developer` skill) rather than promising parity from the docs.**
