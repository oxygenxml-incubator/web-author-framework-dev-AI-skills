Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorListener
    All Superinterfaces: [CompoundEditListener](CompoundEditListener.md)   All Known Implementing Classes: [AuthorListenerAdapter](AuthorListenerAdapter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorListenerextends [CompoundEditListener](CompoundEditListener.md)
Listener notified about Author document changes, document structure changes and document content changes. **DANGER:** You must avoid making live document changes on the received call backs. Please use instead the "ro.sync.ecss.extensions.api.AuthorDocumentController.setDocumentFilter(AuthorDocumentFilter)" API.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
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

### Methods inherited from interface ro.sync.ecss.extensions.api.[CompoundEditListener](CompoundEditListener.md)
 [beforeCompoundEditCancelled](CompoundEditListener.md#beforeCompoundEditCancelled()), [compoundEditCancelled](CompoundEditListener.md#compoundEditCancelled()), [compoundEditEnded](CompoundEditListener.md#compoundEditEnded()), [compoundEditStarted](CompoundEditListener.md#compoundEditStarted())
## Method Details

### beforeContentDelete

void beforeContentDelete([DocumentContentDeletedEvent](DocumentContentDeletedEvent.md) e)

Called before some content is deleted from the document.
  Parameters: e - The [DocumentContentDeletedEvent](DocumentContentDeletedEvent.md).
### beforeAttributeChange

void beforeAttributeChange([AttributeChangedEvent](AttributeChangedEvent.md) e)

Called when an attribute is about to be changed in one of the document's elements.
  Parameters: e - The [AttributeChangedEvent](AttributeChangedEvent.md).
### beforeContentInsert

void beforeContentInsert([DocumentContentInsertedEvent](DocumentContentInsertedEvent.md) e)

Called when content is about to be inserted into a document.
  Parameters: e - The [DocumentContentInsertedEvent](DocumentContentInsertedEvent.md).
### beforeDoctypeChange

void beforeDoctypeChange()

Called before the DOCTYPE section is about to be changed.

### beforeAuthorNodeStructureChange

void beforeAuthorNodeStructureChange([AuthorNode](node/AuthorNode.md) authorNode)

Called when a node structure is about to be changed.
  Parameters: authorNode - The [AuthorNode](node/AuthorNode.md) that contains the modification.
### beforeAuthorNodeNameChange

void beforeAuthorNodeNameChange([AuthorNode](node/AuthorNode.md) authorNode)

Called when a node name is about to be changed.  The authorNode is a reference to the actual node in the [AuthorDocument](node/AuthorDocument.md) so its name will be changed after the name change operation is completed. If the old name of the node will be needed after the call of this method it should be obtained and saved during this method call.
  Parameters: authorNode - The [AuthorNode](node/AuthorNode.md) that will be changed.
### attributeChanged

void attributeChanged([AttributeChangedEvent](AttributeChangedEvent.md) e)

Called when an Author attribute is changed in one of the document's elements.
  Parameters: e - The [AttributeChangedEvent](AttributeChangedEvent.md).
### authorNodeNameChanged

void authorNodeNameChanged([AuthorNode](node/AuthorNode.md) node)

This is called when a node has been renamed.
  Parameters: node - The [AuthorNode](node/AuthorNode.md) that was renamed.
### authorNodeStructureChanged

void authorNodeStructureChanged([AuthorNode](node/AuthorNode.md) node)

The node structure has been changed. An insert or delete operation has been made and affected the children of the node.
  Parameters: node - The [AuthorNode](node/AuthorNode.md) that contains the modification.
### documentChanged

void documentChanged([AuthorDocument](node/AuthorDocument.md) oldDocument, [AuthorDocument](node/AuthorDocument.md) newDocument)

A new document has been set into the author page.
  Parameters: oldDocument - The old Author document newDocument - The new Author document.
### contentDeleted

void contentDeleted([DocumentContentDeletedEvent](DocumentContentDeletedEvent.md) e)

Called when content is deleted from the document.
  Parameters: e - The [DocumentContentDeletedEvent](DocumentContentDeletedEvent.md).
### contentInserted

void contentInserted([DocumentContentInsertedEvent](DocumentContentInsertedEvent.md) e)

Called when content is inserted into the document.
  Parameters: e - The [DocumentContentInsertedEvent](DocumentContentInsertedEvent.md).
### doctypeChanged

void doctypeChanged()

The DOCTYPE section has been changed.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
