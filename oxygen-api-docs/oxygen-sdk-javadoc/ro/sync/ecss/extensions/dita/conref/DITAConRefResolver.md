Package [ro.sync.ecss.extensions.dita.conref](package-summary.md)

# Class DITAConRefResolver

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.DITAConrefsResolverBase](../../api/DITAConrefsResolverBase.md)
        * ro.sync.ecss.extensions.dita.conref.DITAConRefResolver
   All Implemented Interfaces: [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md), [CacheableAuthorReferencesResolver](../../api/CacheableAuthorReferencesResolver.md), [Extension](../../api/Extension.md), [ValidatingAuthorReferenceResolver](../../api/ValidatingAuthorReferenceResolver.md)   Direct Known Subclasses: [DITAMapRefResolver](../map/topicref/DITAMapRefResolver.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAConRefResolver extends [DITAConrefsResolverBase](../../api/DITAConrefsResolverBase.md)implements [CacheableAuthorReferencesResolver](../../api/CacheableAuthorReferencesResolver.md)
Resolver for content referred using conref attribute.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected final [ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md) [keyManagerProvider](#keyManagerProvider)
The context-aware key manager provider used to resolve keyrefs.

## Constructor Summary
 Constructors
Constructor

Description
 [DITAConRefResolver](#%3Cinit%3E())()
Constructor.
  [DITAConRefResolver](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManager))([ContextKeyManager](../../../dita/ContextKeyManager.md) keyManager)  Deprecated.
use [DITAConRefResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.
   [DITAConRefResolver](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider))([ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md) keyManagerProvider)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [checkTarget](#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))([AuthorNode](../../api/node/AuthorNode.md) node, [AuthorDocument](../../api/node/AuthorDocument.md) targetDocument)
Check if the referenced target can be inserted in the source document
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCacheKey](#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Get an unique cache key for a node which references content which will be expanded.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Returns the value of the conref attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceSystemID](#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](../../api/node/AuthorNode.md) node, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Return the systemID of the referred content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceUniqueID](#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
The value of conref attribute is used as the unique identifier.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTopicPath](#getTopicPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Gets the topic IDs as an array of strings.
  boolean [hasReferences](#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
An element that has conref attribute is an element with references.
  boolean [isReferenceChanged](#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Returns true when the attribute name is equal to 'conref'.
  [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))([AuthorNode](../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../../api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Resolve the content referred by conref attribute.
  void [setResolveKeyrefsToMetaContentAsConrefs](#setResolveKeyrefsToMetaContentAsConrefs(boolean))(boolean resolveKeyrefsAsConrefs)
Set to true to resolve all keyrefs as conrefs

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorReferenceResolver](../../api/AuthorReferenceResolver.md)
 [allowsValidatationForEditableReference](../../api/AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [hasEditableReference](../../api/AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [replaceReference](../../api/AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode))
## Field Details

### keyManagerProvider

protected final [ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md) keyManagerProvider

The context-aware key manager provider used to resolve keyrefs.

## Constructor Details

### DITAConRefResolver

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public DITAConRefResolver([ContextKeyManager](../../../dita/ContextKeyManager.md) keyManager)
 Deprecated.
use [DITAConRefResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.

Constructor.
  Parameters: keyManager - The context-aware key manager.
### DITAConRefResolver

public DITAConRefResolver()

Constructor.

### DITAConRefResolver

public DITAConRefResolver([ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md) keyManagerProvider)

Constructor.
  Parameters: keyManagerProvider - The context-aware key manager provider.
## Method Details

### hasReferences

public boolean hasReferences([AuthorNode](../../api/node/AuthorNode.md) node)

An element that has conref attribute is an element with references.
  Specified by: [hasReferences](../../api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) Parameters: node - The node to be analyzed. Returns: true if it has references. See Also:
        * [AuthorReferenceResolver.hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)](../../api/AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode))

### getDisplayName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName([AuthorNode](../../api/node/AuthorNode.md) node)

Returns the value of the conref attribute.
  Specified by: [getDisplayName](../../api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) Parameters: node - The node that contains references. Returns: The display name of the node. See Also:
        * [AuthorReferenceResolver.getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)](../../api/AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode))

### resolveReference

public [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) resolveReference([AuthorNode](../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorAccess](../../api/AuthorAccess.md) authorAccess, [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)throws [ReferenceResolverException](../../api/ReferenceResolverException.md)

Resolve the content referred by conref attribute.
  Specified by: [resolveReference](../../api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver)) in interface [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) Parameters: node - The node which has references. systemID - The system ID of the node with references. authorAccess - The author access implementation. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. entityResolver - The entity resolver that can be used to resolve:
        * Resources that are already opened in editor. For this case the [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) will contain the editor content.
        * Resources resolved through XML catalog.
 Returns: The [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) including the parser and the parser's [InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html). IMPORTANT: the SAXSource needs to have an XMLReader set to it. Throws: [ReferenceResolverException](../../api/ReferenceResolverException.md) - If something goes wrong when resolving the references. See Also:
        * [AuthorReferenceResolver.resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String, AuthorAccess, EntityResolver)](../../api/AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))

### getTopicPath

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTopicPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Gets the topic IDs as an array of strings.
  Parameters: value - The conref attribute value. Returns: The path of IDs as an array of strings.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### getReferenceUniqueID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceUniqueID([AuthorNode](../../api/node/AuthorNode.md) node)

The value of conref attribute is used as the unique identifier.
  Specified by: [getReferenceUniqueID](../../api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) Parameters: node - The node that has reference. Returns: An unique identifier for the reference node. See Also:
        * [AuthorReferenceResolver.getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)](../../api/AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode))

### isReferenceChanged

public boolean isReferenceChanged([AuthorNode](../../api/node/AuthorNode.md) node, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Returns true when the attribute name is equal to 'conref'.
  Specified by: [isReferenceChanged](../../api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)) in interface [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) Parameters: node - The [AuthorNode](../../api/node/AuthorNode.md) with the references. attributeName - The name of the changed attribute. Returns: true if the references must be refreshed. See Also:
        * [AuthorReferenceResolver.isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode, java.lang.String)](../../api/AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))

### getReferenceSystemID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceSystemID([AuthorNode](../../api/node/AuthorNode.md) node, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))
Return the systemID of the referred content.
  Specified by: [getReferenceSystemID](../../api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorReferenceResolver](../../api/AuthorReferenceResolver.md) Parameters: node - The reference node. authorAccess - The author access. It provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. Returns: The systemID of the referred content. See Also:
        * [AuthorReferenceResolver.getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode, AuthorAccess)](../../api/AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))

### checkTarget

public void checkTarget([AuthorNode](../../api/node/AuthorNode.md) node, [AuthorDocument](../../api/node/AuthorDocument.md) targetDocument)throws [ValidatingReferenceResolverException](../../api/ValidatingReferenceResolverException.md)
 Description copied from interface: [ValidatingAuthorReferenceResolver](../../api/ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))
Check if the referenced target can be inserted in the source document
  Specified by: [checkTarget](../../api/ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument)) in interface [ValidatingAuthorReferenceResolver](../../api/ValidatingAuthorReferenceResolver.md) Parameters: node - The source node for which the target node was resolved. targetDocument - The target document Throws: [ValidatingReferenceResolverException](../../api/ValidatingReferenceResolverException.md) - If the source does not accept the target expanded in place. See Also:
        * [ValidatingAuthorReferenceResolver.checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode, ro.sync.ecss.extensions.api.node.AuthorDocument)](../../api/ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))

### setResolveKeyrefsToMetaContentAsConrefs

public void setResolveKeyrefsToMetaContentAsConrefs(boolean resolveKeyrefsAsConrefs)
 Description copied from class: [DITAConrefsResolverBase](../../api/DITAConrefsResolverBase.md#setResolveKeyrefsToMetaContentAsConrefs(boolean))
Set to true to resolve all keyrefs as conrefs
  Specified by: [setResolveKeyrefsToMetaContentAsConrefs](../../api/DITAConrefsResolverBase.md#setResolveKeyrefsToMetaContentAsConrefs(boolean)) in class [DITAConrefsResolverBase](../../api/DITAConrefsResolverBase.md) Parameters: resolveKeyrefsAsConrefs - If true, will resolve keyword keyrefs as conrefs. See Also:
        * [DITAConrefsResolverBase.setResolveKeyrefsToMetaContentAsConrefs(boolean)](../../api/DITAConrefsResolverBase.md#setResolveKeyrefsToMetaContentAsConrefs(boolean))

### getCacheKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCacheKey([AuthorNode](../../api/node/AuthorNode.md) node)
 Description copied from interface: [CacheableAuthorReferencesResolver](../../api/CacheableAuthorReferencesResolver.md#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode))
Get an unique cache key for a node which references content which will be expanded.
  Specified by: [getCacheKey](../../api/CacheableAuthorReferencesResolver.md#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [CacheableAuthorReferencesResolver](../../api/CacheableAuthorReferencesResolver.md) Parameters: node - The node. Returns: an unique cache key for a node which references expanded content. Can be null if the node should not be cached. See Also:
        * [CacheableAuthorReferencesResolver.getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode)](../../api/CacheableAuthorReferencesResolver.md#getCacheKey(ro.sync.ecss.extensions.api.node.AuthorNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
