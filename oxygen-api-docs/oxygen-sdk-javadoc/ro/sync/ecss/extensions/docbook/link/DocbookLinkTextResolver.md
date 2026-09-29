Package [ro.sync.ecss.extensions.docbook.link](package-summary.md)

# Class DocbookLinkTextResolver

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.link.LinkTextResolver](../../api/link/LinkTextResolver.md)
        * ro.sync.ecss.extensions.docbook.link.DocbookLinkTextResolver
   @API(type=EXTENDABLE, src=PUBLIC) public class DocbookLinkTextResolver extends [LinkTextResolver](../../api/link/LinkTextResolver.md)
Resolves local docbook xrefs. The content of the link is given by either the xreflabel attribute or a title(info/title) child of the targeted element.
  Since: 14.2
## Constructor Summary
 Constructors
Constructor

Description
 [DocbookLinkTextResolver](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [activated](#activated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Signals that this resolver has entered in use.
  void [clearReferencesCache](#clearReferencesCache())()
Any cache should be cleared in order to prepare for future evaluations.
  void [deactivated](#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Signals that this resolver has exit from use.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitleValue](#getTitleValue(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) elem)
Checks if the element has a TITLE child or an INFO/TITLE child and returns it's value.
  void [refresh](#refresh())()
Signals a major refresh.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resolveReference](#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../../api/node/AuthorNode.md) node)
Gets a text representation for the reference.

### Methods inherited from class ro.sync.ecss.extensions.api.link.[LinkTextResolver](../../api/link/LinkTextResolver.md)
 [refreshNodeReferences](../../api/link/LinkTextResolver.md#refreshNodeReferences(ro.sync.ecss.extensions.api.node.AuthorNode)), [update](../../api/link/LinkTextResolver.md#update(java.util.Set))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocbookLinkTextResolver

public DocbookLinkTextResolver()

## Method Details

### resolveReference

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resolveReference([AuthorNode](../../api/node/AuthorNode.md) node)throws [InvalidLinkException](../../api/link/InvalidLinkException.md)
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode))
Gets a text representation for the reference. This text will be used inside author page next to the the link element.
  Overrides: [resolveReference](../../api/link/LinkTextResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode)) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) Parameters: node - Author node. Returns: The link text. Throws: [InvalidLinkException](../../api/link/InvalidLinkException.md) - When it is not possible to resolve the link. See Also:
        * [LinkTextResolver.resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode)](../../api/link/LinkTextResolver.md#resolveReference(ro.sync.ecss.extensions.api.node.AuthorNode))

### refresh

public void refresh()
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#refresh())
Signals a major refresh. Any cache should be cleared in order to prepare for future evaluations.
  Overrides: [refresh](../../api/link/LinkTextResolver.md#refresh()) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) See Also:
        * [LinkTextResolver.refresh()](../../api/link/LinkTextResolver.md#refresh())

### clearReferencesCache

public void clearReferencesCache()
 Description copied from class: [LinkTextResolver](../../api/link/LinkTextResolver.md#clearReferencesCache())
Any cache should be cleared in order to prepare for future evaluations.
  Overrides: [clearReferencesCache](../../api/link/LinkTextResolver.md#clearReferencesCache()) in class [LinkTextResolver](../../api/link/LinkTextResolver.md) See Also:
        * [LinkTextResolver.clearReferencesCache()](../../api/link/LinkTextResolver.md#clearReferencesCache())

### getTitleValue

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitleValue([AuthorElement](../../api/node/AuthorElement.md) elem)

Checks if the element has a TITLE child or an INFO/TITLE child and returns it's value.
  Parameters: elem - The current element. Returns: The title value.
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
