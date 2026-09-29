Package [ro.sync.ecss.component.resolvers](package-summary.md)

# Class AuthorReferenceResolverWrapper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.component.resolvers.AuthorReferenceResolverWrapper
   All Implemented Interfaces: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md), [Extension](../../extensions/api/Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorReferenceResolverWrapper extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md)
Adapter used to make wrappers over [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md).
  Since: 18.1
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorReferenceResolverWrapper](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorReferenceResolver))([AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) wrappedResolver)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [allowsValidatationForEditableReference](#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../extensions/api/node/AuthorNode.md) referenceNodeParent)
Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../extensions/api/node/AuthorNode.md) node)
Returns the name of the node that contains the expanded referred content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceSystemID](#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](../../extensions/api/node/AuthorNode.md) node, [AuthorAccess](../../extensions/api/AuthorAccess.md) authorAccess)
Return the systemID of the referred content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceUniqueID](#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../extensions/api/node/AuthorNode.md) node)
Get an unique identifier for the node reference.
  [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) [getWrappedResolver](#getWrappedResolver())()

 boolean [hasEditableReference](#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../extensions/api/node/AuthorNode.md) referenceNodeParent)
Check if the node is editable.
  boolean [hasReferences](#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../extensions/api/node/AuthorNode.md) node)
Verifies if the handler considers the node to have references.
  boolean [isReferenceChanged](#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../../extensions/api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Verifies if the references of the given node must be refreshed when the attribute with the specified name has changed.
  void [replaceReference](#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))([AuthorDocumentProvider](../../extensions/api/node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](../../extensions/api/AuthorAccess.md) authorAccess, [AuthorReferenceNode](../../extensions/api/node/AuthorReferenceNode.md) referenceNode)
Replace the content of the referenced node from the target document with the modified content inside the reference node.
  [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))([AuthorNode](../../extensions/api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../../extensions/api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Resolve the references of the node.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorReferenceResolverWrapper

public AuthorReferenceResolverWrapper([AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) wrappedResolver)

Constructor.
  Parameters: wrappedResolver - The wrapped resolver.
## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../extensions/api/Extension.md#getDescription()) in interface [Extension](../../extensions/api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../extensions/api/Extension.md#getDescription())

### hasReferences

public boolean hasReferences([AuthorNode](../../extensions/api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))
Verifies if the handler considers the node to have references. For example the method should return true for a DITA element that has conref attribute set.
  Specified by: [hasReferences](../../extensions/api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: node - The node to be analyzed. Returns: true if it has references. See Also:
        * [AuthorReferenceResolver.hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)](../../extensions/api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))

### isReferenceChanged

public boolean isReferenceChanged([AuthorNode](../../extensions/api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))
Verifies if the references of the given node must be refreshed when the attribute with the specified name has changed. For example the DITA implementation returns true when the attribute name is equal to 'conref'.
  Specified by: [isReferenceChanged](../../extensions/api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: node - The [AuthorNode](../../extensions/api/node/AuthorNode.md) with the references. attributeName - The name of the changed attribute. Returns: true if the references must be refreshed. See Also:
        * [AuthorReferenceResolver.isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String)](../../extensions/api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))

### resolveReference

public [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) resolveReference([AuthorNode](../../extensions/api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../../extensions/api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))
Resolve the references of the node. The returning [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) will be used for creating the referred content using the parser and the source inside it. IMPORTANT: the SAXSource needs to have an XMLReader set to it. For example the DITA implementation resolves the content referred by the conref attribute.
  Specified by: [resolveReference](../../extensions/api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: node - The node which has references. systemID - The system ID of the node with references. authorAccess - The author access implementation. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. entityResolver - The entity resolver that can be used to resolve:
        * Resources that are already opened in editor. For this case the [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) will contain the editor content.
        * Resources resolved through XML catalog.
 Returns: The [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) including the parser and the parser's [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html). IMPORTANT: the SAXSource needs to have an XMLReader set to it. See Also:
        * [AuthorReferenceResolver.resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String, ro.sync.ecss.extensions.api.AuthorAccess, org.xml.sax.EntityResolver)](../../extensions/api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))

### getDisplayName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName([AuthorNode](../../extensions/api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))
Returns the name of the node that contains the expanded referred content. For example the value of the conref attribute is returned by the DITA implementation.
  Specified by: [getDisplayName](../../extensions/api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: node - The node that contains references. Returns: The display name of the node. See Also:
        * [AuthorReferenceResolver.getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)](../../extensions/api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))

### getReferenceUniqueID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceUniqueID([AuthorNode](../../extensions/api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))
Get an unique identifier for the node reference. The unique identifier is used to avoid resolving the references recursively. For example the DITA implementation uses the value of the conref attribute as the unique identifier.
  Specified by: [getReferenceUniqueID](../../extensions/api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: node - The node that has reference. Returns: An unique identifier for the reference node. See Also:
        * [AuthorReferenceResolver.getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)](../../extensions/api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))

### getReferenceSystemID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceSystemID([AuthorNode](../../extensions/api/node/AuthorNode.md) node, [AuthorAccess](../../extensions/api/AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
Return the systemID of the referred content.
  Specified by: [getReferenceSystemID](../../extensions/api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: node - The reference node. authorAccess - The author access. It provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. Returns: The systemID of the referred content. See Also:
        * [AuthorReferenceResolver.getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.AuthorAccess)](../../extensions/api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))

### getWrappedResolver

public [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) getWrappedResolver()
  Returns: Returns the wrapped resolver.
### hasEditableReference

public boolean hasEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../extensions/api/node/AuthorNode.md) referenceNodeParent)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the node is editable.
  Specified by: [hasEditableReference](../../extensions/api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future referene node Returns: true if the node is editable. See Also:
        * [AuthorReferenceResolver.hasEditableReference(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorNode)](../../extensions/api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))

### allowsValidatationForEditableReference

public boolean allowsValidatationForEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../extensions/api/node/AuthorNode.md) referenceNodeParent)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  Specified by: [allowsValidatationForEditableReference](../../extensions/api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future reference node Returns: true if the editable node reference can be validated by Oxygen on its own, based on its own schema information. See Also:
        * [AuthorReferenceResolver.allowsValidatationForEditableReference(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorNode)](../../extensions/api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))

### replaceReference

public void replaceReference([AuthorDocumentProvider](../../extensions/api/node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](../../extensions/api/AuthorAccess.md) authorAccess, [AuthorReferenceNode](../../extensions/api/node/AuthorReferenceNode.md) referenceNode)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Description copied from interface: [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))
Replace the content of the referenced node from the target document with the modified content inside the reference node.
  Specified by: [replaceReference](../../extensions/api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode)) in interface [AuthorReferenceResolver](../../extensions/api/AuthorReferenceResolver.md) Parameters: targetProvider - The provider to the target document. authorAccess - Access to the current document. referenceNode - The reference node to get the modified content from. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the save process fails See Also:
        * [AuthorReferenceResolver.replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider, ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorReferenceNode)](../../extensions/api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
