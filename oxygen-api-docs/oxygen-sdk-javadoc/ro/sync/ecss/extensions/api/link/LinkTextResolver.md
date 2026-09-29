Package [ro.sync.ecss.extensions.api.link](package-summary.md)

# Class LinkTextResolver

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.link.LinkTextResolver
   Direct Known Subclasses: [DitaLinkTextResolver](../../dita/link/DitaLinkTextResolver.md), [DocbookLinkTextResolver](../../docbook/link/DocbookLinkTextResolver.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class LinkTextResolver extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Resolves a link and obtains a text representation. This interface is used when CSS function oxy_link-text() is encountered in the CSS on 'content' properties.
  Since: 14.2
## Constructor Summary
 Constructors
Constructor

Description
 [LinkTextResolver](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [activated](#activated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../AuthorAccess.md) authorAccess)
Signals that this resolver has entered in use.
  void [clearReferencesCache](#clearReferencesCache())()
Any cache should be cleared in order to prepare for future evaluations.
  void [deactivated](#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../AuthorAccess.md) authorAccess)
Signals that this resolver has exit from use.
  void [refresh](#refresh())()
Signals a major refresh.
  void [refreshNodeReferences](#refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../node/AuthorNode.md) node)
Marks the references used by the given node as being invalid and requiring refreshing.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../node/AuthorNode.md) node)
Gets a text representation for the reference.
  void [update](#update(java.util.Set))([Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> modifiedURLs)
The given URLs have changed.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### LinkTextResolver

public LinkTextResolver()

## Method Details

### resolveReference

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resolveReference([AuthorNode](../node/AuthorNode.md) node)throws [InvalidLinkException](InvalidLinkException.md)

Gets a text representation for the reference. This text will be used inside author page next to the the link element.
  Parameters: node - Author node. Returns: The link text. Throws: [InvalidLinkException](InvalidLinkException.md) - When it is not possible to resolve the link.
### update

public void update([Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> modifiedURLs)

The given URLs have changed. Update the cache of references if any of the resolved links were loaded from one of these URL.
  Parameters: modifiedURLs - The URLs that are modified.
### refresh

public void refresh()

Signals a major refresh. Any cache should be cleared in order to prepare for future evaluations.

### clearReferencesCache

public void clearReferencesCache()

Any cache should be cleared in order to prepare for future evaluations.

### activated

public void activated([AuthorAccess](../AuthorAccess.md) authorAccess)

Signals that this resolver has entered in use. All kinds of listeners can be added on this call (like [AuthorMouseListener](../AuthorMouseListener.md) or [AuthorListener](../AuthorListener.md)).
  Parameters: authorAccess - The [AuthorAccess](../AuthorAccess.md) of the Author page where the listener was activated.
### deactivated

public void deactivated([AuthorAccess](../AuthorAccess.md) authorAccess)

Signals that this resolver has exit from use. All listeners should be removed on this call.
  Parameters: authorAccess - The [AuthorAccess](../AuthorAccess.md) of the Author page where the listener was activated.
### refreshNodeReferences

public void refreshNodeReferences([AuthorNode](../node/AuthorNode.md) node)

Marks the references used by the given node as being invalid and requiring refreshing. After performing an internal refresh the resolver must get an editor access using [AuthorAccess.getEditorAccess()](../AuthorAccess.md#getEditorAccess()) and call [WSAuthorEditorPageBase.refresh(AuthorNode)](../../../../exml/workspace/api/editor/page/author/WSAuthorEditorPageBase.md#refresh(ro.sync.ecss.extensions.api.node.AuthorNode))so that the editing area updates.
  Parameters: node - The node to be refresh.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
