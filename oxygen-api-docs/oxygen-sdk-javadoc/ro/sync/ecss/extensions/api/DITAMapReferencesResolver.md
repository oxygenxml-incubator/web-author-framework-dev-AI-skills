Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface DITAMapReferencesResolver
    All Superinterfaces: [AuthorReferenceResolver](AuthorReferenceResolver.md), [Extension](Extension.md), [ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)   All Known Implementing Classes: [DITAMapRefResolver](../dita/map/topicref/DITAMapRefResolver.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface DITAMapReferencesResolverextends [ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)
Resolve references when showing a DITA Map in the editor

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EXPAND_PSEUDO_CLASS](#EXPAND_PSEUDO_CLASS)
Reference elements (like topicref, mapref, etc) will be expanded if: have this pseudo class this pseudo class is set on root See also [setResolveAllTopicReferences(boolean)](#setResolveAllTopicReferences(boolean)).

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 default [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getGrammarCache](#getGrammarCache())()
Get the grammar cache to be reused in another references resolver.
  default void [setExpandMapReferences](#setExpandMapReferences(boolean))(boolean isExpandMapRefs)
Decide whether to expand or not the references of DITA maps.
  default void [setGrammarCache](#setGrammarCache(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCache)
Set the grammar cache to be reused in another references resolver.
  void [setResolveAllTopicReferences](#setResolveAllTopicReferences(boolean))(boolean resolveAllTopicRefs)
Try to resolve all topic references

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorReferenceResolver](AuthorReferenceResolver.md)
 [allowsValidatationForEditableReference](AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [getDisplayName](AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)), [getReferenceSystemID](AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)), [getReferenceUniqueID](AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)), [hasEditableReference](AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [hasReferences](AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)), [isReferenceChanged](AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [replaceReference](AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode)), [resolveReference](AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
### Methods inherited from interface ro.sync.ecss.extensions.api.[ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)
 [checkTarget](ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))
## Field Details

### EXPAND_PSEUDO_CLASS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EXPAND_PSEUDO_CLASS

Reference elements (like topicref, mapref, etc) will be expanded if:
        *  have this pseudo class
        *  this pseudo class is set on root
See also [setResolveAllTopicReferences(boolean)](#setResolveAllTopicReferences(boolean)).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.DITAMapReferencesResolver.EXPAND_PSEUDO_CLASS)

## Method Details

### setResolveAllTopicReferences

void setResolveAllTopicReferences(boolean resolveAllTopicRefs)

Try to resolve all topic references
  Parameters: resolveAllTopicRefs - If true, will resolve both map references and topic references. If false, will resolve only map references, defaults to false
### setExpandMapReferences

default void setExpandMapReferences(boolean isExpandMapRefs)

Decide whether to expand or not the references of DITA maps.
  Parameters: isExpandMapRefs - true to expand the references.
### getGrammarCache

default [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getGrammarCache()

Get the grammar cache to be reused in another references resolver.
  Returns: the grammar cache to be reused in another references resolver. Since: 23
### setGrammarCache

default void setGrammarCache([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCache)

Set the grammar cache to be reused in another references resolver.
  Parameters: grammarCache - The grammar cache to be used. Since: 23
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
