Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class DITAConrefsResolverBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.DITAConrefsResolverBase
   All Implemented Interfaces: [AuthorReferenceResolver](AuthorReferenceResolver.md), [Extension](Extension.md), [ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)   Direct Known Subclasses: [DITAConRefResolver](../dita/conref/DITAConRefResolver.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class DITAConrefsResolverBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)
Resolve references when showing DITA content in the editor

## Constructor Summary
 Constructors
Constructor

Description
 [DITAConrefsResolverBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract void [setResolveKeyrefsToMetaContentAsConrefs](#setResolveKeyrefsToMetaContentAsConrefs(boolean))(boolean resolveKeyrefsAsConrefs)
Set to true to resolve all keyrefs as conrefs

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorReferenceResolver](AuthorReferenceResolver.md)
 [allowsValidatationForEditableReference](AuthorReferenceResolver.md#allowsValidatationForEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [getDisplayName](AuthorReferenceResolver.md#getDisplayName(ro.sync.ecss.extensions.api.node.AuthorNode)), [getReferenceSystemID](AuthorReferenceResolver.md#getReferenceSystemID(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess)), [getReferenceUniqueID](AuthorReferenceResolver.md#getReferenceUniqueID(ro.sync.ecss.extensions.api.node.AuthorNode)), [hasEditableReference](AuthorReferenceResolver.md#hasEditableReference(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode)), [hasReferences](AuthorReferenceResolver.md#hasReferences(ro.sync.ecss.extensions.api.node.AuthorNode)), [isReferenceChanged](AuthorReferenceResolver.md#isReferenceChanged(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String)), [replaceReference](AuthorReferenceResolver.md#replaceReference(ro.sync.ecss.extensions.api.node.AuthorDocumentProvider,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorReferenceNode)), [resolveReference](AuthorReferenceResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess,org.xml.sax.EntityResolver))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
### Methods inherited from interface ro.sync.ecss.extensions.api.[ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)
 [checkTarget](ValidatingAuthorReferenceResolver.md#checkTarget(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorDocument))
## Constructor Details

### DITAConrefsResolverBase

public DITAConrefsResolverBase()

## Method Details

### setResolveKeyrefsToMetaContentAsConrefs

public abstract void setResolveKeyrefsToMetaContentAsConrefs(boolean resolveKeyrefsAsConrefs)

Set to true to resolve all keyrefs as conrefs
  Parameters: resolveKeyrefsAsConrefs - If true, will resolve keyword keyrefs as conrefs.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
