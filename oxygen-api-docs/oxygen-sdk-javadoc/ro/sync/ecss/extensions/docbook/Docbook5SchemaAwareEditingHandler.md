Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class Docbook5SchemaAwareEditingHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md)
        * [ro.sync.ecss.extensions.docbook.DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md)
            * ro.sync.ecss.extensions.docbook.Docbook5SchemaAwareEditingHandler
   All Implemented Interfaces: [AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md)   @API(type=INTERNAL, src=PUBLIC) public class Docbook5SchemaAwareEditingHandler extends [DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md)
Specific schema aware editing cases for Docbook5.

## Nested Class Summary

## Nested classes/interfaces inherited from class ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md)
 [AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions](../api/AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions.md)
## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.docbook.[DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md)
 [documentNamespace](DocbookSchemaAwareEditingHandler.md#documentNamespace), [INFO_SUFIX](DocbookSchemaAwareEditingHandler.md#INFO_SUFIX), [PARA](DocbookSchemaAwareEditingHandler.md#PARA), [TITLE](DocbookSchemaAwareEditingHandler.md#TITLE)
### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md)
 [lastHandlerResult](../api/AuthorSchemaAwareEditingHandlerAdapter.md#lastHandlerResult)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md)
 [ACTION_ID_BACKSPACE](../api/AuthorSchemaAwareEditingHandler.md#ACTION_ID_BACKSPACE), [ACTION_ID_CUT](../api/AuthorSchemaAwareEditingHandler.md#ACTION_ID_CUT), [ACTION_ID_DELETE](../api/AuthorSchemaAwareEditingHandler.md#ACTION_ID_DELETE), [ACTION_ID_DND](../api/AuthorSchemaAwareEditingHandler.md#ACTION_ID_DND), [ACTION_ID_INSERT_FRAGMENT](../api/AuthorSchemaAwareEditingHandler.md#ACTION_ID_INSERT_FRAGMENT), [ACTION_ID_PASTE](../api/AuthorSchemaAwareEditingHandler.md#ACTION_ID_PASTE), [ACTION_ID_TYPING](../api/AuthorSchemaAwareEditingHandler.md#ACTION_ID_TYPING), [CREATE_FRAGMENT_PURPOSE_COPY](../api/AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_COPY), [CREATE_FRAGMENT_PURPOSE_CUT](../api/AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_CUT), [CREATE_FRAGMENT_PURPOSE_DND_COPY](../api/AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_DND_COPY), [CREATE_FRAGMENT_PURPOSE_DND_MOVE](../api/AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_DND_MOVE)
## Constructor Summary
 Constructors
Constructor

Description
 [Docbook5SchemaAwareEditingHandler](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentNamespace)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [changeElementsToMoveUpDown](#changeElementsToMoveUpDown(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](../api/node/AuthorNode.md)> selectedElements)
Determine the elements that should be moved by the Move Up/Down operation.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getInfoElementChildOfSect](#getInfoElementChildOfSect(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sectElementName)
Get the info child element name of to the given sect element name.

### Methods inherited from class ro.sync.ecss.extensions.docbook.[DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md)
 [getAncestorDetectionOptions](DocbookSchemaAwareEditingHandler.md#getAncestorDetectionOptions()), [getPreferredElement](DocbookSchemaAwareEditingHandler.md#getPreferredElement(ro.sync.ecss.extensions.api.AuthorDocumentController,int)), [handlePasteFragment](DocbookSchemaAwareEditingHandler.md#handlePasteFragment(int,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess)), [handleTyping](DocbookSchemaAwareEditingHandler.md#handleTyping(int,char,ro.sync.ecss.extensions.api.AuthorAccess)), [handleTypingFallback](DocbookSchemaAwareEditingHandler.md#handleTypingFallback(int,char,ro.sync.ecss.extensions.api.AuthorAccess)), [isElementWithNameAndNamespace](DocbookSchemaAwareEditingHandler.md#isElementWithNameAndNamespace(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [pushContextElement](DocbookSchemaAwareEditingHandler.md#pushContextElement(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext,java.lang.String))
### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md)
 [canBeReplaced](../api/AuthorSchemaAwareEditingHandlerAdapter.md#canBeReplaced(ro.sync.ecss.extensions.api.node.AuthorNode)), [getLastResult](../api/AuthorSchemaAwareEditingHandlerAdapter.md#getLastResult()), [handleCreateDocumentFragment](../api/AuthorSchemaAwareEditingHandlerAdapter.md#handleCreateDocumentFragment(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess)), [handleDelete](../api/AuthorSchemaAwareEditingHandlerAdapter.md#handleDelete(int,int,ro.sync.ecss.extensions.api.AuthorAccess,boolean)), [handleDeleteElementTags](../api/AuthorSchemaAwareEditingHandlerAdapter.md#handleDeleteElementTags(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)), [handleDeleteNodes](../api/AuthorSchemaAwareEditingHandlerAdapter.md#handleDeleteNodes(ro.sync.ecss.extensions.api.node.AuthorNode%5B%5D,int,ro.sync.ecss.extensions.api.AuthorAccess)), [handleDeleteSelection](../api/AuthorSchemaAwareEditingHandlerAdapter.md#handleDeleteSelection(int,int,int,ro.sync.ecss.extensions.api.AuthorAccess)), [handleJoinElements](../api/AuthorSchemaAwareEditingHandlerAdapter.md#handleJoinElements(ro.sync.ecss.extensions.api.node.AuthorNode,java.util.List,ro.sync.ecss.extensions.api.AuthorAccess))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md)
 [handleCodePointTyping](../api/AuthorSchemaAwareEditingHandler.md#handleCodePointTyping(int,int,ro.sync.ecss.extensions.api.AuthorAccess)), [handleCodePointTypingFallback](../api/AuthorSchemaAwareEditingHandler.md#handleCodePointTypingFallback(int,int,ro.sync.ecss.extensions.api.AuthorAccess))
## Constructor Details

### Docbook5SchemaAwareEditingHandler

public Docbook5SchemaAwareEditingHandler([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentNamespace)
  Parameters: documentNamespace -
## Method Details

### getInfoElementChildOfSect

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getInfoElementChildOfSect([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sectElementName)
 Description copied from class: [DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md#getInfoElementChildOfSect(java.lang.String))
Get the info child element name of to the given sect element name.
  Overrides: [getInfoElementChildOfSect](DocbookSchemaAwareEditingHandler.md#getInfoElementChildOfSect(java.lang.String)) in class [DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md) Parameters: sectElementName - The sect element name. Returns: The info child element name. See Also:
        * [DocbookSchemaAwareEditingHandler.getInfoElementChildOfSect(java.lang.String)](DocbookSchemaAwareEditingHandler.md#getInfoElementChildOfSect(java.lang.String))

### changeElementsToMoveUpDown

public boolean changeElementsToMoveUpDown([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorNode](../api/node/AuthorNode.md)> selectedElements)
 Description copied from class: [AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md#changeElementsToMoveUpDown(java.util.List))
Determine the elements that should be moved by the Move Up/Down operation. For example if the current selected element is a title then the element that should actually be moved is its parent (e.g. section for DocBook).
  Overrides: [changeElementsToMoveUpDown](DocbookSchemaAwareEditingHandler.md#changeElementsToMoveUpDown(java.util.List)) in class [DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md) Parameters: selectedElements - the selected elements in the author page. This list should be altered depending on the framework specific structure. For example if the current selected element is a title then the element that should actually be present in this list is its parent (e.g. section for DocBook). Returns: true if the list of elements to be moved was altered by the framework specific handler. See Also:
        * [AuthorSchemaAwareEditingHandlerAdapter.changeElementsToMoveUpDown(java.util.List)](../api/AuthorSchemaAwareEditingHandlerAdapter.md#changeElementsToMoveUpDown(java.util.List))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
