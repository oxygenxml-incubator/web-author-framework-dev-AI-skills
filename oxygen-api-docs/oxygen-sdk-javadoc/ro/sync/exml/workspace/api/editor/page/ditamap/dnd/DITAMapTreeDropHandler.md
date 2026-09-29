Package [ro.sync.exml.workspace.api.editor.page.ditamap.dnd](package-summary.md)

# Class DITAMapTreeDropHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.ditamap.dnd.DITAMapTreeDropHandler
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class DITAMapTreeDropHandler extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A handler which can be installed to override handling of drop events in the DITA Map Tree.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapTreeDropHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [acceptDragOverURLs](#acceptDragOverURLs(java.util.List,ro.sync.ecss.extensions.api.node.AuthorNode,boolean))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) resourcesToRefer, [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) contextNode, boolean asChild)
We have a drag over situation with a bunch of resources which have all been previously converted to URLs.
  boolean [consumeDropURLs](#consumeDropURLs(java.util.List,ro.sync.ecss.extensions.api.node.AuthorNode,boolean))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) resourcesToRefer, [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) destination, boolean asChild)
Process drop URLs.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAMapTreeDropHandler

public DITAMapTreeDropHandler()

## Method Details

### acceptDragOverURLs

public boolean acceptDragOverURLs([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) resourcesToRefer, [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) contextNode, boolean asChild)

We have a drag over situation with a bunch of resources which have all been previously converted to URLs. Use this method to accept or reject it.
  Parameters: resourcesToRefer - The resources which will be linked in the map, usually [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) or [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) objects. contextNode - Node over which the mouse is moved. asChild - true if when dropped the list of URLs will be added as children, false if they will be added as siblings (after) the context node. This depends on the position of the mouse relative to the context node bounds. Returns: true if the handler accepts drag over and the default drag over handling should be done, false if it rejects it.
### consumeDropURLs

public boolean consumeDropURLs([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) resourcesToRefer, [AuthorNode](../../../../../../../ecss/extensions/api/node/AuthorNode.md) destination, boolean asChild)

Process drop URLs.
  Parameters: resourcesToRefer - The resources which will be dropped, usually [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) or [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) objects. destination - The node over which the drop was done. asChild - true if when dropped the list of URLs will be added as children, false if they will be added as siblings (after) the destination node. This depends on the position of the mouse relative to the destination node bounds. Returns: true if the handler will make its own processing to insert the references, false if the default processing should be done.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
