Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorListenerAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorListenerAdapter
   All Implemented Interfaces: [AuthorListener](AuthorListener.md), [CompoundEditListener](CompoundEditListener.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorListenerAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorListener](AuthorListener.md)
Convenience implementation of the [AuthorListener](AuthorListener.md).  **DANGER:** You must avoid making live document changes on the received call backs. Please use instead the "ro.sync.ecss.extensions.api.AuthorDocumentController.setDocumentFilter(AuthorDocumentFilter)" API.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorListenerAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [attributeChanged](#attributeChanged(ro.sync.ecss.extensions.api.AttributeChangedEvent))([AttributeChangedEvent](AttributeChangedEvent.md) e)
Called when an Author attribute is changed in one of the document's elements.
  void [authorNodeNameChanged](#authorNodeNameChanged(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
This is called when a node has been renamed.
  void [authorNodeStructureChanged](#authorNodeStructureChanged(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
The node structure has been changed.
  void [beforeAttributeChange](#beforeAttributeChange(ro.sync.ecss.extensions.api.AttributeChangedEvent))([AttributeChangedEvent](AttributeChangedEvent.md) e)
Called when an attribute is about to be changed in one of the document's elements.
  void [beforeAuthorNodeNameChange](#beforeAuthorNodeNameChange(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) authorNode)
Called when a node name is about to be changed.
  void [beforeAuthorNodeStructureChange](#beforeAuthorNodeStructureChange(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) authorNode)
Called when a node structure is about to be changed.
  void [beforeContentDelete](#beforeContentDelete(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent))([DocumentContentDeletedEvent](DocumentContentDeletedEvent.md) e)
Called before some content is deleted from the document.
  void [beforeContentInsert](#beforeContentInsert(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent))([DocumentContentInsertedEvent](DocumentContentInsertedEvent.md) e)
Called when content is about to be inserted into a document.
  void [beforeDoctypeChange](#beforeDoctypeChange())()
Called before the DOCTYPE section is about to be changed.
  void [contentDeleted](#contentDeleted(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent))([DocumentContentDeletedEvent](DocumentContentDeletedEvent.md) e)
Called when content is deleted from the document.
  void [contentInserted](#contentInserted(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent))([DocumentContentInsertedEvent](DocumentContentInsertedEvent.md) e)
Called when content is inserted into the document.
  void [doctypeChanged](#doctypeChanged())()
The DOCTYPE section has been changed.
  void [documentChanged](#documentChanged(ro.sync.ecss.extensions.api.node.AuthorDocument,ro.sync.ecss.extensions.api.node.AuthorDocument))([AuthorDocument](node/AuthorDocument.md) oldDocument, [AuthorDocument](node/AuthorDocument.md) newDocument)
A new document has been set into the author page.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[CompoundEditListener](CompoundEditListener.md)
 [beforeCompoundEditCancelled](CompoundEditListener.md#beforeCompoundEditCancelled()), [compoundEditCancelled](CompoundEditListener.md#compoundEditCancelled()), [compoundEditEnded](CompoundEditListener.md#compoundEditEnded()), [compoundEditStarted](CompoundEditListener.md#compoundEditStarted())
## Constructor Details

### AuthorListenerAdapter

public AuthorListenerAdapter()

## Method Details

### attributeChanged

public void attributeChanged([AttributeChangedEvent](AttributeChangedEvent.md) e)
 Description copied from interface: [AuthorListener](AuthorListener.md#attributeChanged(ro.sync.ecss.extensions.api.AttributeChangedEvent))
Called when an Author attribute is changed in one of the document's elements.
  Specified by: [attributeChanged](AuthorListener.md#attributeChanged(ro.sync.ecss.extensions.api.AttributeChangedEvent)) in interface [AuthorListener](AuthorListener.md) Parameters: e - The [AttributeChangedEvent](AttributeChangedEvent.md). See Also:
        * [AuthorListener.attributeChanged(ro.sync.ecss.extensions.api.AttributeChangedEvent)](AuthorListener.md#attributeChanged(ro.sync.ecss.extensions.api.AttributeChangedEvent))

### authorNodeNameChanged

public void authorNodeNameChanged([AuthorNode](node/AuthorNode.md) node)
 Description copied from interface: [AuthorListener](AuthorListener.md#authorNodeNameChanged(ro.sync.ecss.extensions.api.node.AuthorNode))
This is called when a node has been renamed.
  Specified by: [authorNodeNameChanged](AuthorListener.md#authorNodeNameChanged(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorListener](AuthorListener.md) Parameters: node - The [AuthorNode](node/AuthorNode.md) that was renamed. See Also:
        * [AuthorListener.authorNodeNameChanged(ro.sync.ecss.extensions.api.node.AuthorNode)](AuthorListener.md#authorNodeNameChanged(ro.sync.ecss.extensions.api.node.AuthorNode))

### authorNodeStructureChanged

public void authorNodeStructureChanged([AuthorNode](node/AuthorNode.md) node)
 Description copied from interface: [AuthorListener](AuthorListener.md#authorNodeStructureChanged(ro.sync.ecss.extensions.api.node.AuthorNode))
The node structure has been changed. An insert or delete operation has been made and affected the children of the node.
  Specified by: [authorNodeStructureChanged](AuthorListener.md#authorNodeStructureChanged(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorListener](AuthorListener.md) Parameters: node - The [AuthorNode](node/AuthorNode.md) that contains the modification. See Also:
        * [AuthorListener.authorNodeStructureChanged(ro.sync.ecss.extensions.api.node.AuthorNode)](AuthorListener.md#authorNodeStructureChanged(ro.sync.ecss.extensions.api.node.AuthorNode))

### beforeAttributeChange

public void beforeAttributeChange([AttributeChangedEvent](AttributeChangedEvent.md) e)
 Description copied from interface: [AuthorListener](AuthorListener.md#beforeAttributeChange(ro.sync.ecss.extensions.api.AttributeChangedEvent))
Called when an attribute is about to be changed in one of the document's elements.
  Specified by: [beforeAttributeChange](AuthorListener.md#beforeAttributeChange(ro.sync.ecss.extensions.api.AttributeChangedEvent)) in interface [AuthorListener](AuthorListener.md) Parameters: e - The [AttributeChangedEvent](AttributeChangedEvent.md). See Also:
        * [AuthorListener.beforeAttributeChange(AttributeChangedEvent)](AuthorListener.md#beforeAttributeChange(ro.sync.ecss.extensions.api.AttributeChangedEvent))

### beforeAuthorNodeStructureChange

public void beforeAuthorNodeStructureChange([AuthorNode](node/AuthorNode.md) authorNode)
 Description copied from interface: [AuthorListener](AuthorListener.md#beforeAuthorNodeStructureChange(ro.sync.ecss.extensions.api.node.AuthorNode))
Called when a node structure is about to be changed.
  Specified by: [beforeAuthorNodeStructureChange](AuthorListener.md#beforeAuthorNodeStructureChange(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorListener](AuthorListener.md) Parameters: authorNode - The [AuthorNode](node/AuthorNode.md) that contains the modification. See Also:
        * [AuthorListener.beforeAuthorNodeStructureChange(ro.sync.ecss.extensions.api.node.AuthorNode)](AuthorListener.md#beforeAuthorNodeStructureChange(ro.sync.ecss.extensions.api.node.AuthorNode))

### beforeAuthorNodeNameChange

public void beforeAuthorNodeNameChange([AuthorNode](node/AuthorNode.md) authorNode)
 Description copied from interface: [AuthorListener](AuthorListener.md#beforeAuthorNodeNameChange(ro.sync.ecss.extensions.api.node.AuthorNode))
Called when a node name is about to be changed.  The authorNode is a reference to the actual node in the [AuthorDocument](node/AuthorDocument.md) so its name will be changed after the name change operation is completed. If the old name of the node will be needed after the call of this method it should be obtained and saved during this method call.
  Specified by: [beforeAuthorNodeNameChange](AuthorListener.md#beforeAuthorNodeNameChange(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorListener](AuthorListener.md) Parameters: authorNode - The [AuthorNode](node/AuthorNode.md) that will be changed. See Also:
        * [AuthorListener.beforeAuthorNodeNameChange(ro.sync.ecss.extensions.api.node.AuthorNode)](AuthorListener.md#beforeAuthorNodeNameChange(ro.sync.ecss.extensions.api.node.AuthorNode))

### beforeContentDelete

public void beforeContentDelete([DocumentContentDeletedEvent](DocumentContentDeletedEvent.md) e)
 Description copied from interface: [AuthorListener](AuthorListener.md#beforeContentDelete(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent))
Called before some content is deleted from the document.
  Specified by: [beforeContentDelete](AuthorListener.md#beforeContentDelete(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent)) in interface [AuthorListener](AuthorListener.md) Parameters: e - The [DocumentContentDeletedEvent](DocumentContentDeletedEvent.md). See Also:
        * [AuthorListener.beforeContentDelete(DocumentContentDeletedEvent)](AuthorListener.md#beforeContentDelete(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent))

### beforeContentInsert

public void beforeContentInsert([DocumentContentInsertedEvent](DocumentContentInsertedEvent.md) e)
 Description copied from interface: [AuthorListener](AuthorListener.md#beforeContentInsert(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent))
Called when content is about to be inserted into a document.
  Specified by: [beforeContentInsert](AuthorListener.md#beforeContentInsert(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent)) in interface [AuthorListener](AuthorListener.md) Parameters: e - The [DocumentContentInsertedEvent](DocumentContentInsertedEvent.md). See Also:
        * [AuthorListener.beforeContentInsert(DocumentContentInsertedEvent)](AuthorListener.md#beforeContentInsert(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent))

### beforeDoctypeChange

public void beforeDoctypeChange()
 Description copied from interface: [AuthorListener](AuthorListener.md#beforeDoctypeChange())
Called before the DOCTYPE section is about to be changed.
  Specified by: [beforeDoctypeChange](AuthorListener.md#beforeDoctypeChange()) in interface [AuthorListener](AuthorListener.md) See Also:
        * [AuthorListener.beforeDoctypeChange()](AuthorListener.md#beforeDoctypeChange())

### contentDeleted

public void contentDeleted([DocumentContentDeletedEvent](DocumentContentDeletedEvent.md) e)
 Description copied from interface: [AuthorListener](AuthorListener.md#contentDeleted(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent))
Called when content is deleted from the document.
  Specified by: [contentDeleted](AuthorListener.md#contentDeleted(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent)) in interface [AuthorListener](AuthorListener.md) Parameters: e - The [DocumentContentDeletedEvent](DocumentContentDeletedEvent.md). See Also:
        * [AuthorListener.contentDeleted(DocumentContentDeletedEvent)](AuthorListener.md#contentDeleted(ro.sync.ecss.extensions.api.DocumentContentDeletedEvent))

### contentInserted

public void contentInserted([DocumentContentInsertedEvent](DocumentContentInsertedEvent.md) e)
 Description copied from interface: [AuthorListener](AuthorListener.md#contentInserted(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent))
Called when content is inserted into the document.
  Specified by: [contentInserted](AuthorListener.md#contentInserted(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent)) in interface [AuthorListener](AuthorListener.md) Parameters: e - The [DocumentContentInsertedEvent](DocumentContentInsertedEvent.md). See Also:
        * [AuthorListener.contentInserted(DocumentContentInsertedEvent)](AuthorListener.md#contentInserted(ro.sync.ecss.extensions.api.DocumentContentInsertedEvent))

### doctypeChanged

public void doctypeChanged()
 Description copied from interface: [AuthorListener](AuthorListener.md#doctypeChanged())
The DOCTYPE section has been changed.
  Specified by: [doctypeChanged](AuthorListener.md#doctypeChanged()) in interface [AuthorListener](AuthorListener.md) See Also:
        * [AuthorListener.doctypeChanged()](AuthorListener.md#doctypeChanged())

### documentChanged

public void documentChanged([AuthorDocument](node/AuthorDocument.md) oldDocument, [AuthorDocument](node/AuthorDocument.md) newDocument)
 Description copied from interface: [AuthorListener](AuthorListener.md#documentChanged(ro.sync.ecss.extensions.api.node.AuthorDocument,ro.sync.ecss.extensions.api.node.AuthorDocument))
A new document has been set into the author page.
  Specified by: [documentChanged](AuthorListener.md#documentChanged(ro.sync.ecss.extensions.api.node.AuthorDocument,ro.sync.ecss.extensions.api.node.AuthorDocument)) in interface [AuthorListener](AuthorListener.md) Parameters: oldDocument - The old Author document newDocument - The new Author document. See Also:
        * [AuthorListener.documentChanged(ro.sync.ecss.extensions.api.node.AuthorDocument, ro.sync.ecss.extensions.api.node.AuthorDocument)](AuthorListener.md#documentChanged(ro.sync.ecss.extensions.api.node.AuthorDocument,ro.sync.ecss.extensions.api.node.AuthorDocument))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
