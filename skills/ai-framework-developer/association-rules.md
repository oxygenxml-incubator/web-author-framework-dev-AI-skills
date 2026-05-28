# Association Rules — Matching a File to a Framework

When oXygen / Web Author opens a document, it walks every installed framework's `<associationRules>` and picks the highest-priority match. Wrong rules → document opens in the generic XML editor with no styling, no actions, "no schema or DTD associated".

The XSD documents `<associationRules>` as: *"Oxygen XML Editor identifies the framework associated with a document when the document matches at least one of the association rules."* — i.e. multiple `<addRule>` siblings combine with **OR**.

## Where association lives

Inside `<script>`:

```xml
<associationRules inherit="all">
  <addRule rootElementLocalName="topic" namespace="" />
</associationRules>
```

- **`@inherit="all"`** *(default)* — keep the base framework's rules and add yours.
- **`@inherit="none"`** — discard the base's rules. Only your rules decide. Use for standalone frameworks (no `@base`) so a generic root element doesn't accidentally claim every doc.

## `<addRule>` attributes

**Every declarative attribute defaults to `"*"` (any).** Leaving an attribute off is the same as `*`: that dimension simply does not constrain the match. A rule with only `rootElementLocalName="topic"` matches a `<topic>` in *any* namespace, *any* file name, *any* public ID. AND-within-rule emerges naturally from this — each non-`*` attribute adds a constraint that must hold. (The XSD does not state AND-within-rule explicitly; it's the only consistent reading of attribute-level `*` defaults.)

| Attribute | Default | Matches when… | Typical use |
|---|---|---|---|
| `rootElementLocalName` | `*` | The document's root element local-name equals the value. | Primary signal for most XML formats. |
| `namespace` | `*` | The document's root namespace URI equals the value. **Set to the empty string** (XSD doc verbatim: *"If you want to apply the rule only when the root element has no namespace, leave this field empty (remove the *)."*) to match no-namespace docs. | Disambiguate two formats sharing a root name. |
| `fileName` | `*` | The file name matches the value. (XSD doc says only "Specifies the name of the file" — does not document glob/regex semantics. Verify in a real kit before relying on patterns.) | Non-XML or schema-less formats — JSON, CSV. Useful when the root element is generic (`<root>`, `<document>`). |
| `publicID` | `*` | The DOCTYPE's public identifier equals the value. | DTD-driven formats (legacy DocBook, DITA, JATS). |
| `attributeLocalName` + `attributeNamespace` + `attributeValue` | each `*` | The root element has an attribute with the given local name (and optional namespace) whose value equals `attributeValue`. | DITA-class disambiguation, schema-via-attribute, profile attributes. |
| `javaRuleClass` | *(no default — attribute optional)* | A class implementing `ro.sync.ecss.extensions.api.DocumentTypeCustomRuleMatcher` returns `true`. | Anything declarative attributes can't express — content sniffing, multi-condition logic. Used by bundled DITA-map-resolved and custom-JSON frameworks. |

## Example — extending DITA only for a specialization

```xml
<associationRules inherit="all">
  <addRule
    rootElementLocalName="topic"
    attributeLocalName="class"
    attributeValue="- topic/topic concept/concept "/>
</associationRules>
```

Activates only for DITA topics carrying a specific `class` value. `inherit="all"` keeps base DITA rules in place for unspecialized topics.

> **Verify `attributeValue` semantics** before relying on a pattern. The XSD says only that the attribute "specifies the value of the attributes for the root element" — it does not document whether comparison is exact-equality, substring (DITA's `class` uses surrounding-space conventions), or whitespace-normalized. Confirm against a bundled `.exf` (e.g. `<EXPANDED_WEBAPP_DIR>/frameworks/dita/dita-lw.exf`) or a doc topic before assuming substring matching.

## Example — standalone framework with multiple match conditions (OR)

```xml
<associationRules inherit="none">
  <addRule rootElementLocalName="catalog" namespace="http://example.org/cat"/>
  <addRule fileName="*.cat.xml"/>
</associationRules>
```

Activates if root is `<catalog>` in the right namespace **OR** the file name ends with `.cat.xml`. Use multi-rule OR sparingly — easy to over-claim.

## Example — Java rule class

```xml
<associationRules inherit="none">
  <addRule javaRuleClass="com.example.MyDocumentMatcher"/>
</associationRules>
```

The class must be on the framework's `<classpath>` and implement `ro.sync.ecss.extensions.api.DocumentTypeCustomRuleMatcher` (XSD doc, verbatim). Whether `javaRuleClass` and the declarative attributes can be combined on the *same* `<addRule>` is not documented in the XSD — the safe pattern is one or the other per rule. Use multiple `<addRule>` siblings (OR) when both styles are needed.

## Priority interaction

The `<priority>` element documentation in the XSD: *"When multiple frameworks match on a document, the one with the highest priority will be used."* Values: `Lowest`, `Low`, `Normal`, `High`, `Highest`. The official topic adds: *"The `<priority>` element might be needed to instruct Oxygen XML Editor to use this new framework instead of the one being extended or another framework that matches the same document."*

Tie-breaking when two frameworks share the same priority — by rule specificity, by load order, by name — is **not documented**. Don't rely on a specific tie-breaker; resolve ties by raising priority or narrowing rules so only one framework matches.

## Diagnosing a wrong match

If a document opens in plain-text / generic-XML, the validation rail says "no schema or DTD associated", or custom CSS doesn't apply (framework didn't activate at all):

1. Read the document's actual root element (local name + namespace) and any DOCTYPE / root-attribute. Don't guess from filename.
2. Check `OXYGEN_LOG` for `Loading user uploaded frameworks from:` — confirms your extension was scanned.
3. Walk the rules: do *all* attributes on at least one `<addRule>` match the document?
4. Check priority: is anything else `High` for the same base?
5. Compare against the bundled equivalent (`<EXPANDED_WEBAPP_DIR>/frameworks/<base>/`) — bundled rule shape is ground truth.

For deep diagnosis see `web-author-logs.md` in this skill — enable the relevant logger via `logback.xml` rather than guessing.

## Reference

Official topic: <https://www.oxygenxml.com/doc/ug-editor/topics/framework-customization-script-usecases.md> (read the `.md` via `oxygen-docs`).
