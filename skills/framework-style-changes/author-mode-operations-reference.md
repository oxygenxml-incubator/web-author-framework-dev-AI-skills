# Author Mode Operations (Relevant Subset)

Subset from `ug-editor/topics/dg-default-author-operations.md`, filtered for what is typically useful in `framework-style-changes` work (Author-mode UI behavior, pseudo-classes, fragment insertion, and action chaining).

Parent flow reference: `ug-editor/topics/dg-create-custom-actions.md`.

## URL base

- Docs base: `https://www.oxygenxml.com/doc/ug-editor/`
- Main page: `https://www.oxygenxml.com/doc/ug-editor/topics/dg-default-author-operations.md`

## Core operations to keep handy

### Pseudo-class control (most relevant for style toggles)

- `SetPseudoClassOperation`
  - Sets one pseudo-class on nodes from `elementLocation`.
  - Args: `name`, `elementLocation`, `includeAllNodes`.
- `RemovePseudoClassOperation`
  - Removes one pseudo-class on nodes from `elementLocation`.
  - Args: `name`, `elementLocation`, `includeAllNodes`.
- `TogglePseudoClassOperation`
  - Toggles one pseudo-class on/off.
  - Args: `name`, `elementLocation`, `includeAllNodes`.
- `ChangePseudoClassesOperation`
  - Batch set/remove pseudo-classes with separate XPath selectors.
  - Args: `setLocations`, `setPseudoClassNames`, `removeLocations`, `removePseudoClassNames`, `includeAllNodes`.

### Attribute updates used by style-driven actions

- `ChangeAttributeOperation`
  - Add/modify/remove one attribute.
  - Args: `name`, `namespace`, `elementLocation`, `value`, `editAttribute`, `removeIfEmpty`.
- `ChangeAttributesOperation`
  - Add/modify/remove multiple attributes in one call.
  - Args: `elementLocations`, `attributeNames`, `values`, `removeIfEmpty`.

### Insert/replace/surround actions commonly used with toolbar or form-control flows

- `InsertFragmentOperation`
  - Insert XML fragment at cursor.
  - Args in source page: not fully enumerated there.
  - Follow-up page: `dg-author-op-InsertFragmentOperation-arguments`.
- `InsertOrReplaceFragmentOperation`
  - Replace selection or insert fragment, with configurable insert position.
  - Args in source page:
    - same base arguments as `InsertFragmentOperation` (see dedicated args page);
    - explicit note that `insertPosition` also supports `Replace`.
- `InsertOrReplaceTextOperation`
  - Replace selection with plain text.
  - Args: `text`.
- `SurroundWithFragmentOperation`
  - Wrap selection in XML fragment (content goes in first leaf).
  - Args in source page: not fully enumerated there.
  - Follow-up page: `dg-author-op-SurroundWithFragmentOperation-arguments`.
- `SurroundWithTextOperation`
  - Wrap selection with text header/footer.
  - Args: `header`, `footer`.
- `ToggleSurroundWithElementOperation`
  - Toggle wrap/unwrap with a given element (useful for semantic inline toggles).
  - Args: `element`, `schemaAware`.
- `UnwrapTagsOperation`
  - Remove wrapping tags for current/target node.
  - Args: `unwrapElementLocation`.

### Structural operations useful in focused action workflows

- `RenameElementOperation`
  - Rename matched elements.
  - Args: `elementName`, `elementLocation`.
- `ReplaceElementContentOperation`
  - Replace content of selected/current element with fragment.
  - Args: `fragment`, `elementLocation`.
- `MoveElementOperation`
  - Move content between source and target XPath locations.
  - Args: `sourceLocation`, `deleteLocation`, `surroundFragment`, `targetLocation`, `insertPosition`, `moveOnlySourceContentNodes`, `processTrackedChangesForXpathLocations`, `alwaysPreserveTrackedChangesInMovedContent`.
- `MoveCaretOperation`
  - Reposition caret/selection after action result.
  - Args: `xpathLocation`, `position`, `selection`.
- `DeleteElementOperation` / `DeleteElementsOperation`
  - Delete one or multiple nodes.
  - Args:
    - `DeleteElementOperation`: `elementLocation` (optional; default = node at cursor).
    - `DeleteElementsOperation`: `elementLocations` (optional; default = node at cursor).
- `ToggleCommentOperation`
  - Comment/uncomment selection.
  - Args: none.

### Action composition

- `ExecuteMultipleActionsOperation`
  - Runs action IDs in sequence.
  - Args: `actionIDs`.
- `ExecuteMultipleWebappCompatibleActionsOperation`
  - Runs a sequence of Web Author-compatible action IDs.
  - Args in source page: not explicitly enumerated.

## Other built-in operation names (brief)

If the subset above is not enough, also check these operation names from the same built-in list:

- `ExecuteCommandLineOperation`
- `ExecuteTransformationScenariosOperation`
- `ExecuteValidationScenariosOperation`
- `InsertEquationOperation`
- `InsertXIncludeOperation`
- `JSOperation`
- `OpenInSystemAppOperation`
- `ReloadContentOperation`
- `ShowElementDocumentationOperation`
- `XSLTOperation`
- `XQueryOperation`

For full argument details, verify in:

- `https://www.oxygenxml.com/doc/ug-editor/topics/dg-default-author-operations.md`
- `https://www.oxygenxml.com/doc/ug-editor/topics/dg-create-custom-actions.md`
- The operation chooser in Oxygen (`Document Type Association` -> `Author` -> `Actions` -> `Operation` -> `Choose`), which shows arguments for the selected operation.
- API docs (`AuthorOperation`) and `getArguments()` for exact runtime argument metadata.

## Explicitly not for Web Author (from official page notes)

- `ExecuteCustomizableTransformationScenarioOperation`
- `StopCurrentTransformationScenarioOperation`
- `XQueryUpdateOperation`
- `InvokeAIActionOperation`

## Editor variables worth using in operation parameters

- `${caret}`, `${selection}`
- `${ask(...)}`
- `${uuid}`, `${id}`, `${date(pattern)}`
- `${cf}`, `${cfd}`, `${frameworksDir}`, `${homeDir}`
- `${env(VAR_NAME)}`, `${system(var.name)}`

Use these to avoid hardcoded values and to prompt the user at runtime.

## Related pages (jump list)

- `https://www.oxygenxml.com/doc/ug-editor/topics/dg-create-custom-actions.md`
- `https://www.oxygenxml.com/doc/ug-editor/topics/dg-author-op-InsertFragmentOperation-arguments.md`
- `https://www.oxygenxml.com/doc/ug-editor/topics/dg-author-op-SurroundWithFragmentOperation-arguments.md`
