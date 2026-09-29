Package [ro.sync.ecss.extensions.dita.map.topicref](package-summary.md)

# Class DITAMapRefResolver

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.DITAConrefsResolverBase](../../../api/DITAConrefsResolverBase.md)
        * [ro.sync.ecss.extensions.dita.conref.DITAConRefResolver](../../conref/DITAConRefResolver.md)
            * ro.sync.ecss.extensions.dita.map.topicref.DITAMapRefResolver
   All Implemented Interfaces: [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md), [CacheableAuthorReferencesResolver](../../../api/CacheableAuthorReferencesResolver.md), [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md), [Extension](../../../api/Extension.md), [ValidatingAuthorReferenceResolver](../../../api/ValidatingAuthorReferenceResolver.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAMapRefResolver extends [DITAConRefResolver](../../conref/DITAConRefResolver.md)implements [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md)
Resolves the hrefs to other maps.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.dita.conref.[DITAConRefResolver](../../conref/DITAConRefResolver.md)
 [keyManagerProvider](../../conref/DITAConRefResolver.md#keyManagerProvider)
### Fields inherited from interface ro.sync.ecss.extensions.api.[DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md)
 [EXPAND_PSEUDO_CLASS](../../../api/DITAMapReferencesResolver.md#EXPAND_PSEUDO_CLASS)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapRefResolver](#%3Cinit%3E())()  Deprecated.
use [DITAMapRefResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead, otherwise key resolution will not work in Web Author.
   [DITAMapRefResolver](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManager))([ContextKeyManager](../../../../dita/ContextKeyManager.md) keyManager)  Deprecated.
use [DITAMapRefResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.
   [DITAMapRefResolver](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider))([ContextKeyManagerProvider](../../../../dita/ContextKeyManagerProvider.md) keyManagerProvider)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [allowsValidatationForEditableReference](#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../../api/node/AuthorNode.md) referenceNodeParent)
Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  void [checkTarget](#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))([AuthorNode](../../../api/node/AuthorNode.md) node, [AuthorDocument](../../../api/node/AuthorDocument.md) targetDocument)
Check if the referenced target can be inserted in the source document
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCacheKey](#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Get an unique cache key for a node which references content which will be expanded.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
Returns the value of the href attribute.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getGrammarCache](#getGrammarCache())()
Get the grammar cache to be reused in another references resolver.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceSystemID](#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](../../../api/node/AuthorNode.md) node, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Get the reference System ID
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceUniqueID](#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
The value of conref attribute is used as the unique identifier.
  boolean [hasEditableReference](#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../../api/node/AuthorNode.md) referenceNodeParent)
Check if the node is editable.
  boolean [hasReferences](#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../../api/node/AuthorNode.md) node)
An element that has href attribute is an element with references.
  boolean [isReferenceChanged](#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Returns true when the attribute name is equal to 'conref'.
  void [replaceReference](#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))([AuthorDocumentProvider](../../../api/node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorReferenceNode](../../../api/node/AuthorReferenceNode.md) referenceNode)
Replace the content of the referenced node from the target document with the modified content inside the reference node.
  [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Resolve the content referred by conref attribute.
  void [setExpandMapReferences](#setExpandMapReferences(boolean))(boolean isExpand)
Decide whether to expand or not the references of DITA maps.
  void [setGrammarCache](#setGrammarCache(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCache)
Set the grammar cache to be reused in another references resolver.
  void [setResolveAllTopicReferences](#setResolveAllTopicReferences(boolean))(boolean resolveAllTopicRefs)
Try to resolve all topic references

### Methods inherited from class ro.sync.ecss.extensions.dita.conref.[DITAConRefResolver](../../conref/DITAConRefResolver.md)
 [getDescription](../../conref/DITAConRefResolver.md#getDescription()), [getTopicPath](../../conref/DITAConRefResolver.md#getTopicPath(java.lang.String)), [setResolveKeyrefsToMetaContentAsConrefs](../../conref/DITAConRefResolver.md#setResolveKeyrefsToMetaContentAsConrefs(boolean))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../api/Extension.md)
 [getDescription](../../../api/Extension.md#getDescription())
## Constructor Details

### DITAMapRefResolver

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public DITAMapRefResolver([ContextKeyManager](../../../../dita/ContextKeyManager.md) keyManager)
 Deprecated.
use [DITAMapRefResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.

Constructor.
  Parameters: keyManager - The context-aware key manager.
### DITAMapRefResolver

public DITAMapRefResolver([ContextKeyManagerProvider](../../../../dita/ContextKeyManagerProvider.md) keyManagerProvider)

Constructor.
  Parameters: keyManagerProvider - The context-aware key manager provider.
### DITAMapRefResolver

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public DITAMapRefResolver()
 Deprecated.
use [DITAMapRefResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead, otherwise key resolution will not work in Web Author.

Constructor.

## Method Details

### hasReferences

public boolean hasReferences([AuthorNode](../../../api/node/AuthorNode.md) node)

An element that has href attribute is an element with references.
  Specified by: [hasReferences](../../../api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Overrides: [hasReferences](../../conref/DITAConRefResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The node to be analyzed. Returns: true if it has references. See Also:
        * [AuthorReferenceResolver.hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))

### getDisplayName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName([AuthorNode](../../../api/node/AuthorNode.md) node)

Returns the value of the href attribute.
  Specified by: [getDisplayName](../../../api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Overrides: [getDisplayName](../../conref/DITAConRefResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The node that contains references. Returns: The display name of the node. See Also:
        * [AuthorReferenceResolver.getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))

### resolveReference

public [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) resolveReference([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)

Resolve the content referred by conref attribute.
  Specified by: [resolveReference](../../../api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Overrides: [resolveReference](../../conref/DITAConRefResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The node which has references. systemID - The system ID of the node with references. authorAccess - The author access implementation. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. entityResolver - The entity resolver that can be used to resolve:
        * Resources that are already opened in editor. For this case the [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) will contain the editor content.
        * Resources resolved through XML catalog.
 Returns: The [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) including the parser and the parser's [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html). IMPORTANT: the SAXSource needs to have an XMLReader set to it. See Also:
        * [AuthorReferenceResolver.resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String, AuthorAccess, EntityResolver)](../../../api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))

### hasEditableReference

public boolean hasEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../../api/node/AuthorNode.md) referenceNodeParent)
 Description copied from interface: [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the node is editable.
  Specified by: [hasEditableReference](../../../api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future referene node Returns: true if the node is editable. See Also:
        * [AuthorReferenceResolver.hasEditableReference(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorNode)](../../../api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))

### allowsValidatationForEditableReference

public boolean allowsValidatationForEditableReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../../api/node/AuthorNode.md) referenceNodeParent)
 Description copied from interface: [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))
Check if the editable node reference can be validated by Oxygen on its own, when modified, based on its own schema information.
  Specified by: [allowsValidatationForEditableReference](../../../api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Parameters: systemID - System ID of the document in which the current node is located. referenceNodeParent - The parent of the future reference node Returns: true if the editable node reference can be validated by Oxygen on its own, based on its own schema information. See Also:
        * [AuthorReferenceResolver.allowsValidatationForEditableReference(java.lang.String, ro.sync.ecss.extensions.api.node.AuthorNode)](../../../api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))

### replaceReference

public void replaceReference([AuthorDocumentProvider](../../../api/node/AuthorDocumentProvider.md) targetProvider, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [AuthorReferenceNode](../../../api/node/AuthorReferenceNode.md) referenceNode)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Description copied from interface: [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))
Replace the content of the referenced node from the target document with the modified content inside the reference node.
  Specified by: [replaceReference](../../../api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Parameters: targetProvider - The provider to the target document. authorAccess - Access to the current document. referenceNode - The reference node to get the modified content from. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the save process fails See Also:
        * [AuthorReferenceResolver.replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider, ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.node.AuthorReferenceNode)](../../../api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))

### getReferenceSystemID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceSystemID([AuthorNode](../../../api/node/AuthorNode.md) node, [AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Get the reference System ID
  Specified by: [getReferenceSystemID](../../../api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Overrides: [getReferenceSystemID](../../conref/DITAConRefResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The reference node. authorAccess - The author access. It provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. Returns: The systemID of the referred content. See Also:
        * [AuthorReferenceResolver.getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode, AuthorAccess)](../../../api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))

### checkTarget

public void checkTarget([AuthorNode](../../../api/node/AuthorNode.md) node, [AuthorDocument](../../../api/node/AuthorDocument.md) targetDocument)throws [ValidatingReferenceResolverException](../../../api/ValidatingReferenceResolverException.md)
 Description copied from interface: [ValidatingAuthorReferenceResolver](../../../api/ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))
Check if the referenced target can be inserted in the source document
  Specified by: [checkTarget](../../../api/ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument)) in interface [ValidatingAuthorReferenceResolver](../../../api/ValidatingAuthorReferenceResolver.md) Overrides: [checkTarget](../../conref/DITAConRefResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The source node for which the target node was resolved. targetDocument - The target document Throws: [ValidatingReferenceResolverException](../../../api/ValidatingReferenceResolverException.md) - If the source does not accept the target expanded in place. See Also:
        * [ValidatingAuthorReferenceResolver.checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.node.AuthorDocument)](../../../api/ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))

### getReferenceUniqueID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceUniqueID([AuthorNode](../../../api/node/AuthorNode.md) node)

The value of conref attribute is used as the unique identifier.
  Specified by: [getReferenceUniqueID](../../../api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Overrides: [getReferenceUniqueID](../../conref/DITAConRefResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The node that has reference. Returns: An unique identifier for the reference node. See Also:
        * [AuthorReferenceResolver.getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)](../../../api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))

### isReferenceChanged

public boolean isReferenceChanged([AuthorNode](../../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Returns true when the attribute name is equal to 'conref'.
  Specified by: [isReferenceChanged](../../../api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)) in interface [AuthorReferenceResolver](../../../api/AuthorReferenceResolver.md) Overrides: [isReferenceChanged](../../conref/DITAConRefResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The [AuthorNode](../../../api/node/AuthorNode.md) with the references. attributeName - The name of the changed attribute. Returns: true if the references must be refreshed. See Also:
        * [AuthorReferenceResolver.isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String)](../../../api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))

### setResolveAllTopicReferences

public void setResolveAllTopicReferences(boolean resolveAllTopicRefs)
 Description copied from interface: [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md#setResolveAllTopicReferences(boolean))
Try to resolve all topic references
  Specified by: [setResolveAllTopicReferences](../../../api/DITAMapReferencesResolver.md#setResolveAllTopicReferences(boolean)) in interface [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md) Parameters: resolveAllTopicRefs - If true, will resolve both map references and topic references. If false, will resolve only map references, defaults to false See Also:
        * [DITAMapReferencesResolver.setResolveAllTopicReferences(boolean)](../../../api/DITAMapReferencesResolver.md#setResolveAllTopicReferences(boolean))

### setExpandMapReferences

public void setExpandMapReferences(boolean isExpand)
 Description copied from interface: [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md#setExpandMapReferences(boolean))
Decide whether to expand or not the references of DITA maps.
  Specified by: [setExpandMapReferences](../../../api/DITAMapReferencesResolver.md#setExpandMapReferences(boolean)) in interface [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md) Parameters: isExpand - true to expand the references. See Also:
        * [DITAMapReferencesResolver.setExpandMapReferences(boolean)](../../../api/DITAMapReferencesResolver.md#setExpandMapReferences(boolean))

### getGrammarCache

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getGrammarCache()
 Description copied from interface: [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md#getGrammarCache())
Get the grammar cache to be reused in another references resolver.
  Specified by: [getGrammarCache](../../../api/DITAMapReferencesResolver.md#getGrammarCache()) in interface [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md) Returns: the grammar cache to be reused in another references resolver. See Also:
        * [DITAMapReferencesResolver.getGrammarCache()](../../../api/DITAMapReferencesResolver.md#getGrammarCache())

### setGrammarCache

public void setGrammarCache([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCache)
 Description copied from interface: [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md#setGrammarCache(java.lang.Object))
Set the grammar cache to be reused in another references resolver.
  Specified by: [setGrammarCache](../../../api/DITAMapReferencesResolver.md#setGrammarCache(java.lang.Object)) in interface [DITAMapReferencesResolver](../../../api/DITAMapReferencesResolver.md) Parameters: grammarCache - The grammar cache to be used. See Also:
        * [DITAMapReferencesResolver.setGrammarCache(java.lang.Object)](../../../api/DITAMapReferencesResolver.md#setGrammarCache(java.lang.Object))

### getCacheKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCacheKey([AuthorNode](../../../api/node/AuthorNode.md) node)
 Description copied from interface: [CacheableAuthorReferencesResolver](../../../api/CacheableAuthorReferencesResolver.md#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode))
Get an unique cache key for a node which references content which will be expanded.
  Specified by: [getCacheKey](../../../api/CacheableAuthorReferencesResolver.md#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [CacheableAuthorReferencesResolver](../../../api/CacheableAuthorReferencesResolver.md) Overrides: [getCacheKey](../../conref/DITAConRefResolver.md#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [DITAConRefResolver](../../conref/DITAConRefResolver.md) Parameters: node - The node. Returns: an unique cache key for a node which references expanded content. Can be null if the node should not be cached. See Also:
        * [DITAConRefResolver.getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode)](../../conref/DITAConRefResolver.md#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
