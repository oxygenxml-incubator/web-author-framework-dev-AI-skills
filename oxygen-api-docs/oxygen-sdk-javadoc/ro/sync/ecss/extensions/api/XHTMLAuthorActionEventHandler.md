Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class XHTMLAuthorActionEventHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md)
        * [ro.sync.ecss.extensions.api.DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
            * ro.sync.ecss.extensions.api.XHTMLAuthorActionEventHandler
   All Implemented Interfaces: [AuthorActionEventHandler](AuthorActionEventHandler.md), [Extension](Extension.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class XHTMLAuthorActionEventHandler extends [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
Author action event handler for XHTML. IMPORTANT, THIS CLASS SHOULD HAVE BEEN CREATED IN THE FRAMEWORK SPECIFIC PACKAGE. BUT IT WAS NOT, TOO LATE, WE KEEP IT HERE FOR BACKWARD COMPATIBILITY

## Nested Class Summary

## Nested classes/interfaces inherited from class ro.sync.ecss.extensions.api.[DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
 [DefaultAuthorActionEventHandler.CiElementAndOffset](DefaultAuthorActionEventHandler.CiElementAndOffset.md)
## Nested classes/interfaces inherited from interface ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
 [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md)
## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLAuthorActionEventHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParagraphElement](#getParagraphElement(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Get the preferred XML element content to be inserted.

### Methods inherited from class ro.sync.ecss.extensions.api.[DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)
 [areCompatibleLists](DefaultAuthorActionEventHandler.md#areCompatibleLists(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode)), [canHandleEvent](DefaultAuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)), [deleteNodeChildren](DefaultAuthorActionEventHandler.md#deleteNodeChildren(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorNode)), [getContentCompletionActions](DefaultAuthorActionEventHandler.md#getContentCompletionActions(ro.sync.ecss.extensions.api.AuthorAccess,int)), [getDescription](DefaultAuthorActionEventHandler.md#getDescription()), [getInsertableFormForElement](DefaultAuthorActionEventHandler.md#getInsertableFormForElement(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement,int)), [getPreferredXMLElementContent](DefaultAuthorActionEventHandler.md#getPreferredXMLElementContent(ro.sync.ecss.extensions.api.AuthorAccess)), [handleEvent](DefaultAuthorActionEventHandler.md#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType)), [isList](DefaultAuthorActionEventHandler.md#isList(ro.sync.ecss.extensions.api.node.AuthorNode)), [isMovableListItem](DefaultAuthorActionEventHandler.md#isMovableListItem(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode)), [promote](DefaultAuthorActionEventHandler.md#promote(ro.sync.ecss.extensions.api.AuthorDocumentController,int,java.util.List,boolean)), [promoteSubListItems](DefaultAuthorActionEventHandler.md#promoteSubListItems(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
 [canHandleEvent](AuthorActionEventHandler.md#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventDetails)), [getListItemAncestorToSplit](AuthorActionEventHandler.md#getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
## Constructor Details

### XHTMLAuthorActionEventHandler

public XHTMLAuthorActionEventHandler()

## Method Details

### getParagraphElement

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParagraphElement([AuthorAccess](AuthorAccess.md) authorAccess)
 Description copied from class: [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md#getParagraphElement(ro.sync.ecss.extensions.api.AuthorAccess))
Get the preferred XML element content to be inserted. Can be null.
  Overrides: [getParagraphElement](DefaultAuthorActionEventHandler.md#getParagraphElement(ro.sync.ecss.extensions.api.AuthorAccess)) in class [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md) Parameters: authorAccess - The author access. Returns: the preferred XML element content to be inserted.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
