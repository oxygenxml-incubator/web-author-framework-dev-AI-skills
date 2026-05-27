---
name: schematron-quick-fix
description: Use when authoring, debugging, or shipping Schematron Quick Fixes (SQF) — `sqf:fix`, `sqf:add`, `sqf:delete`, `sqf:replace`, `sqf:stringReplace`, `sqf:user-entry`, `sqf:call-fix`, `sqf:group`, `sqf:fixes`, `use-when`, `use-for-each`, `$sqf:current`. Covers defining fixes inside an `<assert>` / `<report>`, embedding SQF in RELAX NG or XML Schema, and wiring the resulting `.sch` file into a framework via `.exf` validation scenarios. Routed to from `ai-framework-developer`; for canonical doc lookups defer to `oxygen-docs`.
---

# Schematron Quick Fixes (SQF)

Use this skill for any work involving the Schematron Quick Fix extension to ISO Schematron — defining fixes, the four operation elements, user-entry dialogs, conditional / iterated fixes, parameterized fixes, and shipping them as part of a framework.

## References

- Operation-level reference (`<sqf:fix>`, the four operations, `<sqf:user-entry>`, `<sqf:call-fix>`, `<sqf:group>`, `<sqf:fixes>`, `<sqf:copy-of>`, `<sqf:param>`, `@use-when`, `@use-for-each`, attribute matrix, formatting) — `sqf-operations-reference.md`
- Grounded working examples (DITA prolog, `@id` generation, abstract restructuring, enum picker via `@use-for-each`, CALS attributes, move-node idiom, user-entry, conditional) — `sqf-examples.md`
- Shipping a `.sch` as part of a framework (`.exf` + `.scenarios` route, schema-detection order, WA-specific gotchas) — `framework-integration.md`
- Embedding SQF inside an RNG / XSD grammar — `embedding-sqf.md`
- Curated docs index (`/doc/ug-editor/` SQF pages, spec, community samples) — `doc-references.md`
- For any pure documentation lookup not covered above — `oxygen-docs` skill (fetches `.md`; cite `.html`)
- `.exf` shape and `.scenarios` export format — `ai-framework-developer` (`exf-structure.md`, `validation-scenarios-export.md`)
- Browser verification of the Quick Fix proposal popup — `chrome-mcp-usage.md` in the `ai-framework-developer` skill
- Diagnosing "fix not loaded" at startup — `web-author-logs.md` in the `ai-framework-developer` skill

## When NOT to use

- Plain Schematron `<assert>` / `<report>` with no fix → just write the rule. SQF is opt-in via `sqf:fix`.
- Wiring a `.sch` into a validation scenario without a fix → `validation-scenarios-export.md` in the `ai-framework-developer` skill.
- Author-mode CSS / form controls → `framework-style-changes`.

## Required flow

1. Identify the firing `<assert>` / `<report>` and its rule `@context` — that's the fix's anchor unless an operation overrides via `@match`.
2. Pick the operation (`sqf-operations-reference.md` has the matrix): add → `<sqf:add>`, remove → `<sqf:delete>`, swap → `<sqf:replace>`, patch text → `<sqf:stringReplace>`. Use `<sqf:user-entry>` only when the value can't be computed from the document.
3. Decide modifiers: `@use-when` for conditional, `@use-for-each` + `$sqf:current` for enum-style multi-proposal.
4. **Always declare the SQF namespace on the schema root and set `queryBinding="xslt2"`** — these are the two single most common "fix doesn't appear" causes:
   ```xml
   xmlns:sqf="http://www.schematron-quickfix.com/validator/process"
   ```
5. Validate the `.sch` itself in oXygen against the built-in SQF schema — see <https://www.oxygenxml.com/doc/ug-editor/topics/validating-sqf.html>. Catches missing `@target`, malformed XPath, undeclared namespaces the engine would otherwise silently skip.
6. Ship via a framework: `framework-integration.md` (Route A — `.exf` `<validationScenarios>` + `.scenarios`, recommended; Route B — `<defaultSchema schemaType="sch">` for standalone frameworks).
7. Restart the kit per the `ai-framework-developer` rules (full stop + start; `user-frameworks/` is scanned at startup only).
8. Verify in the running editor. For Web Author, use `chrome-mcp-usage.md` (in `ai-framework-developer`) to screenshot the proposal popup — **WA SQF parity with Desktop is not documented one-for-one; verify visually**, do not promise parity from the manual alone.
9. If the fix doesn't surface after two restart cycles, stop tweaking XPath — read `validating-sqf.md` and check `framework-integration.md` "Common failure modes".

## Rules

- **Grounding.** Anything about SQF semantics (attributes, defaults, evaluation order, dialog behavior) must come from `doc-references.md` or a real `.sch`. The engine silently ignores unknown attributes — an invented one just makes the fix "not appear" and burns an iteration.
- **One fix per remedy.** If a single `<assert>` has fundamentally different remedies, make them separate `<sqf:fix>` elements and list both IDs in `@sqf:fix` (space-separated) — see Example 7 in `sqf-examples.md`. Don't branch inside one fix with `@use-when` on each operation.

## URL convention

Both `ug-waCustom` and `ug-editor` paths are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching the `.md` or giving the user a complete URL, and replace `.md` with `.html` for the citation link.
