Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DOTProjectAuthorReferenceResolver

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.DOTProjectAuthorReferenceResolver
   All Implemented Interfaces: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md), [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DOTProjectAuthorReferenceResolver extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorReferenceResolver](../api/AuthorReferenceResolver.md)
Author Reference Resolver for DITA-OT Project files. It will resolve all  <include href="includedProject.xml">   references.

## Constructor Summary
 Constructors
Constructor

Description
 [DOTProjectAuthorReferenceResolver](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [allowsValidatationForEditableReference](#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../api/node/AuthorNode.md) referenceNodeParent)
Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Returns the name of the node that contains the expanded referred content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceSystemID](#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](../api/node/AuthorNode.md) node, [AuthorAccess](../api/AuthorAccess.md) authorAccess)
Return the systemID of the referred content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceUniqueID](#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Get an unique identifier for the node reference.
  boolean [hasEditableReference](#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../api/node/AuthorNode.md) referenceNodeParent)
Check if the node is editable.
  boolean [hasReferences](#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Only 'include' elements have references.
  boolean [isReferenceChanged](#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
A reference is changed when the value of the href is changed.
  void [replaceReference](#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))([AuthorDocumentProvider](../api/node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorReferenceNode](../api/node/AuthorReferenceNode.md) referenceNode)
Replace the content of the referenced node from the target document with the modified content inside the reference node.
  [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))([AuthorNode](../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Resolve the references of the node.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DOTProjectAuthorReferenceResolver

public DOTProjectAuthorReferenceResolver()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../api/Extension.md#getDescription()) in interface [Extension](../api/Extension.md) Returns: The description of the extension.
### resolveReference

public [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) resolveReference([AuthorNode](../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)throws [ReferenceResolverException](../api/ReferenceResolverException.md)
 Description copied from interface: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))
Resolve the references of the node. The returning [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) will be used for creating the referred content using the parser and the source inside it. IMPORTANT: the SAXSource needs to have an XMLReader set to it. For example the DITA implementation resolves the content referred by the conref attribute.
  Specified by: [resolveReference](../api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: node - The node which has references. systemID - The system ID of the node with references. authorAccess - The author access implementation. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. entityResolver - The entity resolver that can be used to resolve:
        * Resources that are already opened in editor. For this case the [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) will contain the editor content.
        * Resources resolved through XML catalog.
 Returns: The [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) including the parser and the parser's [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html). IMPORTANT: the SAXSource needs to have an XMLReader set to it. Throws: [ReferenceResolverException](../api/ReferenceResolverException.md) - If something goes wrong when resolving the references.
### isReferenceChanged

public boolean isReferenceChanged([AuthorNode](../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

A reference is changed when the value of the href is changed.
  Specified by: [isReferenceChanged](../api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: node - The [AuthorNode](../api/node/AuthorNode.md) with the references. attributeName - The name of the changed attribute. Returns: true if the references must be refreshed.
### hasReferences

public boolean hasReferences([AuthorNode](../api/node/AuthorNode.md) node)

Only 'include' elements have references. The value of the HREF attribute should not be null.
  Specified by: [hasReferences](../api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: node - The node we want to check for references. Returns: true if the node has references.
### getReferenceUniqueID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceUniqueID([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))
Get an unique identifier for the node reference. The unique identifier is used to avoid resolving the references recursively. For example the DITA implementation uses the value of the conref attribute as the unique identifier.
  Specified by: [getReferenceUniqueID](../api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: node - The node that has reference. Returns: An unique identifier for the reference node.
### getReferenceSystemID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceSystemID([AuthorNode](../api/node/AuthorNode.md) node, [AuthorAccess](../api/AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
Return the systemID of the referred content.
  Specified by: [getReferenceSystemID](../api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: node - The reference node. authorAccess - The author access. It provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. Returns: The systemID of the referred content.
### getDisplayName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from interface: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))
Returns the name of the node that contains the expanded referred content. For example the value of the conref attribute is returned by the DITA implementation.
  Specified by: [getDisplayName](../api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: node - The node that contains references. Returns: The display name of the node.
### hasEditableReference

public boolean hasEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../api/node/AuthorNode.md) referenceNodeParent)
 Description copied from interface: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the node is editable.
  Specified by: [hasEditableReference](../api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future referene node Returns: true if the node is editable. See Also:
        * [AuthorReferenceResolver.hasEditableReference(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorNode)](../api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))

### replaceReference

public void replaceReference([AuthorDocumentProvider](../api/node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](../api/AuthorAccess.md) authorAccess, [AuthorReferenceNode](../api/node/AuthorReferenceNode.md) referenceNode)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Description copied from interface: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))
Replace the content of the referenced node from the target document with the modified content inside the reference node.
  Specified by: [replaceReference](../api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: targetProvider - The provider to the target document. authorAccess - Access to the current document. referenceNode - The reference node to get the modified content from. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the save process fails See Also:
        * [AuthorReferenceResolver.replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider, ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorReferenceNode)](../api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))

### allowsValidatationForEditableReference

public boolean allowsValidatationForEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../api/node/AuthorNode.md) referenceNodeParent)
 Description copied from interface: [AuthorReferenceResolver](../api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  Specified by: [allowsValidatationForEditableReference](../api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../api/AuthorReferenceResolver.md) Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future reference node Returns: true if the editable node reference can be validated by Oxygen on its own, based on its own schema information. See Also:
        * [AuthorReferenceResolver.allowsValidatationForEditableReference(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorNode)](../api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
