Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface ValidatingAuthorReferenceResolver
    All Superinterfaces: [AuthorReferenceResolver](AuthorReferenceResolver.md), [Extension](Extension.md)   All Known Subinterfaces: [DITAMapReferencesResolver](DITAMapReferencesResolver.md)   All Known Implementing Classes: [DITAConRefResolver](../dita/conref/DITAConRefResolver.md), [DITAConrefsResolverBase](DITAConrefsResolverBase.md), [DITAMapRefResolver](../dita/map/topicref/DITAMapRefResolver.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ValidatingAuthorReferenceResolverextends [AuthorReferenceResolver](AuthorReferenceResolver.md)
This resolver also validates the target

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [checkTarget](#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))([AuthorNode](node/AuthorNode.md) node, [AuthorDocument](node/AuthorDocument.md) targetDocument)
Check if the referenced target can be inserted in the source document

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorReferenceResolver](AuthorReferenceResolver.md)
 [allowsValidatationForEditableReference](AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [getDisplayName](AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)), [getReferenceSystemID](AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)), [getReferenceUniqueID](AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)), [hasEditableReference](AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [hasReferences](AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)), [isReferenceChanged](AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [replaceReference](AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode)), [resolveReference](AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### checkTarget

void checkTarget([AuthorNode](node/AuthorNode.md) node, [AuthorDocument](node/AuthorDocument.md) targetDocument)throws [ValidatingReferenceResolverException](ValidatingReferenceResolverException.md)

Check if the referenced target can be inserted in the source document
  Parameters: node - The source node for which the target node was resolved. targetDocument - The target document Throws: [ValidatingReferenceResolverException](ValidatingReferenceResolverException.md) - If the source does not accept the target expanded in place.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
