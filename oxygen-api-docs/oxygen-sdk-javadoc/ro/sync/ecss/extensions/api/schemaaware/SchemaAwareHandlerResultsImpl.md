Package [ro.sync.ecss.extensions.api.schemaaware](package-summary.md)

# Class SchemaAwareHandlerResultsImpl

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.schemaaware.SchemaAwareHandlerResultsImpl
   All Implemented Interfaces: [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md), [SchemaAwareHandlerResultInsertConstants](SchemaAwareHandlerResultInsertConstants.md)   @API(type=EXTENDABLE, src=PUBLIC) public class SchemaAwareHandlerResultsImpl extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md)
Default implementation for [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md)}.
  Since: 11.2
## Field Summary

### Fields inherited from interface ro.sync.ecss.extensions.api.schemaaware.[SchemaAwareHandlerResult](SchemaAwareHandlerResult.md)
 [TYPE_HANDLE_DELETE_ELEMENT_TAGS_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_DELETE_ELEMENT_TAGS_OPERATION), [TYPE_HANDLE_DELETE_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_DELETE_OPERATION), [TYPE_HANDLE_DELETE_SELECTION_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_DELETE_SELECTION_OPERATION), [TYPE_HANDLE_INSERT_FRAGMENT_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_INSERT_FRAGMENT_OPERATION), [TYPE_HANDLE_JOIN_ELEMENTS_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_JOIN_ELEMENTS_OPERATION), [TYPE_HANDLE_TYPING_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_TYPING_OPERATION)
### Fields inherited from interface ro.sync.ecss.extensions.api.schemaaware.[SchemaAwareHandlerResultInsertConstants](SchemaAwareHandlerResultInsertConstants.md)
 [RESULT_ID_HANDLE_INSERT_FRAGMENT_OFFSET](SchemaAwareHandlerResultInsertConstants.md#RESULT_ID_HANDLE_INSERT_FRAGMENT_OFFSET)
## Constructor Summary
 Constructors
Constructor

Description
 [SchemaAwareHandlerResultsImpl](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationID)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addResult](#addResult(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resultKey, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) resultValue)
Add result.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getResult](#getResult(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resultId)
Get the result for the given id.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getType](#getType())()
The type of operation that generated the result.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SchemaAwareHandlerResultsImpl

public SchemaAwareHandlerResultsImpl([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationID)
  Parameters: operationID - One of [SchemaAwareHandlerResult.TYPE_HANDLE_INSERT_FRAGMENT_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_INSERT_FRAGMENT_OPERATION) for insert fragment operation or [SchemaAwareHandlerResult.TYPE_HANDLE_TYPING_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_TYPING_OPERATION) for typing operation.
## Method Details

### addResult

public void addResult([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resultKey, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) resultValue)

Add result.
  Parameters: resultKey - The result key. Constants are defined in [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md)}. resultValue - The result value.
### getResult

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getResult([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resultId)
 Description copied from interface: [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md#getResult(java.lang.String))
Get the result for the given id.
  Specified by: [getResult](SchemaAwareHandlerResult.md#getResult(java.lang.String)) in interface [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md) Parameters: resultId - One of the constants defined in this interface. Returns: The value for the result. Can be null for an unknown result id. See Also:
        * [SchemaAwareHandlerResult.getResult(java.lang.String)](SchemaAwareHandlerResult.md#getResult(java.lang.String))

### getType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getType()
 Description copied from interface: [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md#getType())
The type of operation that generated the result. Depending on a result type, different information is available through [SchemaAwareHandlerResult.getResult(String)](SchemaAwareHandlerResult.md#getResult(java.lang.String)) method. Possible values are:
        * [SchemaAwareHandlerResult.TYPE_HANDLE_DELETE_ELEMENT_TAGS_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_DELETE_ELEMENT_TAGS_OPERATION) for delete element tags operation, see [AuthorSchemaAwareEditingHandler.handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode, AuthorAccess)](../AuthorSchemaAwareEditingHandler.md#handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess));
        * [SchemaAwareHandlerResult.TYPE_HANDLE_DELETE_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_DELETE_OPERATION) for a keyboard delete operation, see [AuthorSchemaAwareEditingHandler.handleDelete(int, int, AuthorAccess, boolean)](../AuthorSchemaAwareEditingHandler.md#handleDelete(int,int,ro.sync.ecss.extensions.api.AuthorAccess,boolean));
        * [SchemaAwareHandlerResult.TYPE_HANDLE_DELETE_SELECTION_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_DELETE_SELECTION_OPERATION) for delete selection operation, see [AuthorSchemaAwareEditingHandler.handleDeleteSelection(int, int, int, AuthorAccess)](../AuthorSchemaAwareEditingHandler.md#handleDeleteSelection(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess));
        * [SchemaAwareHandlerResult.TYPE_HANDLE_JOIN_ELEMENTS_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_JOIN_ELEMENTS_OPERATION) for join elements operation, see [AuthorSchemaAwareEditingHandler.handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode, java.util.List, AuthorAccess)](../AuthorSchemaAwareEditingHandler.md#handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List,ro.sync.ecss.extensions.api.AuthorAccess));
        * [SchemaAwareHandlerResult.TYPE_HANDLE_INSERT_FRAGMENT_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_INSERT_FRAGMENT_OPERATION) for insert fragment operation, see [AuthorSchemaAwareEditingHandler.handlePasteFragment(int, ro.sync.ecss.extensions.api.node.AuthorDocumentFragment[], int, AuthorAccess)](../AuthorSchemaAwareEditingHandler.md#handlePasteFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess));
        * [SchemaAwareHandlerResult.TYPE_HANDLE_TYPING_OPERATION](SchemaAwareHandlerResult.md#TYPE_HANDLE_TYPING_OPERATION) for typing operation, see [AuthorSchemaAwareEditingHandler.handleTyping(int, char, AuthorAccess)](../AuthorSchemaAwareEditingHandler.md#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess)).

  Specified by: [getType](SchemaAwareHandlerResult.md#getType()) in interface [SchemaAwareHandlerResult](SchemaAwareHandlerResult.md) Returns: One of the constants from above, describing which schema aware operation generated the result. See Also:
        * [SchemaAwareHandlerResult.getType()](SchemaAwareHandlerResult.md#getType())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
