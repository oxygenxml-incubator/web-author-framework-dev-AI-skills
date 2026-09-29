Package [ro.sync.ecss.extensions.api.schemaaware](package-summary.md)

# Interface SchemaAwareHandlerResultInsertConstants
    All Known Subinterfaces: [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md)   All Known Implementing Classes: [SchemaAwareHandlerResultsImpl](SchemaAwareHandlerResultsImpl.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface SchemaAwareHandlerResultInsertConstants
Result informations available for an schema aware insert operation (either typing or insert fragment).
  Since: 11.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RESULT_ID_HANDLE_INSERT_FRAGMENT_OFFSET](#RESULT_ID_HANDLE_INSERT_FRAGMENT_OFFSET)
A schema aware insert might choose to insert a fragment at a different location in order to keep the document valid or might choose to change the document structure in order to accept the fragment.

## Field Details

### RESULT_ID_HANDLE_INSERT_FRAGMENT_OFFSET

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RESULT_ID_HANDLE_INSERT_FRAGMENT_OFFSET

A schema aware insert might choose to insert a fragment at a different location in order to keep the document valid or might choose to change the document structure in order to accept the fragment. This is the offset at which the inserted fragment can be found. Can be -1 value, if the last insert fragment event was not handled.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.schemaaware.SchemaAwareHandlerResultInsertConstants.RESULT_ID_HANDLE_INSERT_FRAGMENT_OFFSET)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
