Package [ro.sync.ecss.extensions.dita.link](package-summary.md)

# Class DitaLinkTextResolver

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.link.LinkTextResolver](../../api/link/LinkTextResolver.md)
        * ro.sync.ecss.extensions.dita.link.DitaLinkTextResolver
   @API(type=EXTENDABLE, src=PUBLIC) public class DitaLinkTextResolver extends [LinkTextResolver](../../api/link/LinkTextResolver.md)
Can resolve DITA references to another topic made through the href attribute on elements of classes: map/topicref , topic/xref and topic/link . It also resolves key references provided that the ditamap is opened in DITA Map Manager."
  Since: 14.2
## Constructor Summary
 Constructors
Constructor

Description
 [DitaLinkTextResolver](#%3Cinit%3E())()
Constructor.
  [DitaLinkTextResolver](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManager))([ContextKeyManager](../../../dita/ContextKeyManager.md) keyManager)  Deprecated.
use [DitaLinkTextResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.
   [DitaLinkTextResolver](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider))([ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md) keyManagerProvider)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [activated](#activated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Signals that this resolver has entered in use.
  void [clearReferencesCache](#clearReferencesCache())()
Any cache should be cleared in order to prepare for future evaluations.
  void [deactivated](#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Signals that this resolver has exit from use.
  void [refresh](#refresh())()
Signals a major refresh.
  void [refreshNodeReferences](#refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Marks the references used by the given node as being invalid and requiring refreshing.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Get the text of the reference.
  void [update](#update(java.util.Set))([Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> modifiedURLs)
Update the cache of references.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DitaLinkTextResolver

public DitaLinkTextResolver()

Constructor.

### DitaLinkTextResolver

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public DitaLinkTextResolver([ContextKeyManager](../../../dita/ContextKeyManager.md) keyManager)
 Deprecated.
use [DitaLinkTextResolver(ContextKeyManagerProvider)](#%3Cinit%3E(ro.sync.ecss.dita.ContextKeyManagerProvider)) instead.

Constructor.
  Parameters: keyManager - The context-aware key manager.
### DitaLinkTextResolver

public DitaLinkTextResolver([ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md) keyManagerProvider)

Constructor
  Parameters: keyManagerProvider - The context-aware key manager provider.
## Method Details

### resolveReference

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resolveReference([AuthorNode](../../api/node/AuthorNode.md) node)throws [InvalidLinkException](../../api/link/InvalidLinkException.md)

Get the text of the reference.
  Overrides: [resolveReference](../../api/link/LinkTextResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) Parameters: node - Author node. Returns: The link text. Throws: [InvalidLinkException](../../api/link/InvalidLinkException.md) - Various problems while resolving the reference.
### update

public void update([Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> modifiedURLs)

Update the cache of references.
  Overrides: [update](../../api/link/LinkTextResolver.md#update(java.util.Set)) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) Parameters: modifiedURLs - The URLs that are modified.
### refresh

public void refresh()
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#refresh())
Signals a major refresh. Any cache should be cleared in order to prepare for future evaluations.
  Overrides: [refresh](../../api/link/LinkTextResolver.md#refresh()) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) See Also:
        * [LinkTextResolver.refresh()](../../api/link/LinkTextResolver.md#refresh())

### refreshNodeReferences

public void refreshNodeReferences([AuthorNode](../../api/node/AuthorNode.md) node)
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode))
Marks the references used by the given node as being invalid and requiring refreshing. After performing an internal refresh the resolver must get an editor access using [AuthorAccess.getEditorAccess()](../../api/AuthorAccess.md#getEditorAccess()) and call [WSAuthorEditorPageBase.refresh(AuthorNode)](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#refresh(ro.sync.ecss.extensions.api.node.AuthorNode))so that the editing area updates.
  Overrides: [refreshNodeReferences](../../api/link/LinkTextResolver.md#refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) Parameters: node - The node to be refresh. See Also:
        * [LinkTextResolver.refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode)](../../api/link/LinkTextResolver.md#refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode))

### clearReferencesCache

public void clearReferencesCache()
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#clearReferencesCache())
Any cache should be cleared in order to prepare for future evaluations.
  Overrides: [clearReferencesCache](../../api/link/LinkTextResolver.md#clearReferencesCache()) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) See Also:
        * [LinkTextResolver.clearReferencesCache()](../../api/link/LinkTextResolver.md#clearReferencesCache())

### activated

public void activated([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#activated(ro.sync.ecss.extensions.api.AuthorAccess))
Signals that this resolver has entered in use. All kinds of listeners can be added on this call (like [AuthorMouseListener](../../api/AuthorMouseListener.md) or [AuthorListener](../../api/AuthorListener.md)).
  Overrides: [activated](../../api/link/LinkTextResolver.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) Parameters: authorAccess - The [AuthorAccess](../../api/AuthorAccess.md) of the Author page where the listener was activated. See Also:
        * [AuthorExtensionStateListener.activated(ro.sync.ecss.extensions.api.AuthorAccess)](../../api/AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess))

### deactivated

public void deactivated([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))
Signals that this resolver has exit from use. All listeners should be removed on this call.
  Overrides: [deactivated](../../api/link/LinkTextResolver.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess)) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) Parameters: authorAccess - The [AuthorAccess](../../api/AuthorAccess.md) of the Author page where the listener was activated. See Also:
        * [AuthorExtensionStateListener.deactivated(ro.sync.ecss.extensions.api.AuthorAccess)](../../api/AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
