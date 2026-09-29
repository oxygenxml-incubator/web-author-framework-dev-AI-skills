Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorReferenceResolver
    All Superinterfaces: [Extension](Extension.md)   All Known Subinterfaces: [DITAMapReferencesResolver](DITAMapReferencesResolver.md), [ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)   All Known Implementing Classes: [AuthorReferenceResolverWrapper](../../component/resolvers/AuthorReferenceResolverWrapper.md), [DITAConRefResolver](../dita/conref/DITAConRefResolver.md), [DITAConrefsResolverBase](DITAConrefsResolverBase.md), [DITAMapRefResolver](../dita/map/topicref/DITAMapRefResolver.md), [DOTProjectAuthorReferenceResolver](../dita/DOTProjectAuthorReferenceResolver.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorReferenceResolverextends [Extension](Extension.md)
Interface for the custom handlers used to expand content references.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 default boolean [allowsValidatationForEditableReference](#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](node/AuthorNode.md) referenceNodeParent)
Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Returns the name of the node that contains the expanded referred content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceSystemID](#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md) node, [AuthorAccess](AuthorAccess.md) authorAccess)
Return the systemID of the referred content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceUniqueID](#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Get an unique identifier for the node reference.
  default boolean [hasEditableReference](#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](node/AuthorNode.md) referenceNodeParent)
Check if the node is editable.
  boolean [hasReferences](#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) node)
Verifies if the handler considers the node to have references.
  boolean [isReferenceChanged](#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Verifies if the references of the given node must be refreshed when the attribute with the specified name has changed.
  default void [replaceReference](#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))([AuthorDocumentProvider](node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](AuthorAccess.md) authorAccess, [AuthorReferenceNode](node/AuthorReferenceNode.md) referenceNode)
Replace the content of the referenced node from the target document with the modified content inside the reference node.
  [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))([AuthorNode](node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Resolve the references of the node.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### hasReferences

boolean hasReferences([AuthorNode](node/AuthorNode.md) node)

Verifies if the handler considers the node to have references. For example the method should return true for a DITA element that has conref attribute set.
  Parameters: node - The node to be analyzed. Returns: true if it has references.
### isReferenceChanged

boolean isReferenceChanged([AuthorNode](node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Verifies if the references of the given node must be refreshed when the attribute with the specified name has changed. For example the DITA implementation returns true when the attribute name is equal to 'conref'.
  Parameters: node - The [AuthorNode](node/AuthorNode.md) with the references. attributeName - The name of the changed attribute. Returns: true if the references must be refreshed.
### resolveReference

[SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) resolveReference([AuthorNode](node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)throws [ReferenceResolverException](ReferenceResolverException.md)

Resolve the references of the node. The returning [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) will be used for creating the referred content using the parser and the source inside it. IMPORTANT: the SAXSource needs to have an XMLReader set to it. For example the DITA implementation resolves the content referred by the conref attribute.
  Parameters: node - The node which has references. systemID - The system ID of the node with references. authorAccess - The author access implementation. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. entityResolver - The entity resolver that can be used to resolve:
        * Resources that are already opened in editor. For this case the [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) will contain the editor content.
        * Resources resolved through XML catalog.
 Returns: The [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) including the parser and the parser's [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html). IMPORTANT: the SAXSource needs to have an XMLReader set to it. Throws: [ReferenceResolverException](ReferenceResolverException.md) - If something goes wrong when resolving the references.
### getDisplayName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName([AuthorNode](node/AuthorNode.md) node)

Returns the name of the node that contains the expanded referred content. For example the value of the conref attribute is returned by the DITA implementation.
  Parameters: node - The node that contains references. Returns: The display name of the node.
### getReferenceUniqueID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceUniqueID([AuthorNode](node/AuthorNode.md) node)

Get an unique identifier for the node reference. The unique identifier is used to avoid resolving the references recursively. For example the DITA implementation uses the value of the conref attribute as the unique identifier.
  Parameters: node - The node that has reference. Returns: An unique identifier for the reference node.
### getReferenceSystemID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceSystemID([AuthorNode](node/AuthorNode.md) node, [AuthorAccess](AuthorAccess.md) authorAccess)

Return the systemID of the referred content.
  Parameters: node - The reference node. authorAccess - The author access. It provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. Returns: The systemID of the referred content.
### hasEditableReference

default boolean hasEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](node/AuthorNode.md) referenceNodeParent)

Check if the node is editable.
  Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future referene node Returns: true if the node is editable. Since: 23
### allowsValidatationForEditableReference

default boolean allowsValidatationForEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](node/AuthorNode.md) referenceNodeParent)

Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future reference node Returns: true if the editable node reference can be validated by Oxygen on its own, based on its own schema information. Since: 23
### replaceReference

default void replaceReference([AuthorDocumentProvider](node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](AuthorAccess.md) authorAccess, [AuthorReferenceNode](node/AuthorReferenceNode.md) referenceNode)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Replace the content of the referenced node from the target document with the modified content inside the reference node.
  Parameters: targetProvider - The provider to the target document. authorAccess - Access to the current document. referenceNode - The reference node to get the modified content from. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the save process fails Since: 23
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
