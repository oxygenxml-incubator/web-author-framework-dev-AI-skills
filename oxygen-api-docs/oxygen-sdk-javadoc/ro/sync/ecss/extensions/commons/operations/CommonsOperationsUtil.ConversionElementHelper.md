Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class CommonsOperationsUtil.ConversionElementHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil.ConversionElementHelper
   Enclosing class: [CommonsOperationsUtil](CommonsOperationsUtil.md)   public abstract static class CommonsOperationsUtil.ConversionElementHelper extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Interface used to check the elements that will be converted in other elements (table cells or list entries)

## Constructor Summary
 Constructors
Constructor

Description
 [ConversionElementHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract boolean [blockContentMustBeConverted](#blockContentMustBeConverted(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](../../api/node/AuthorNode.md) node, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Check if a block node can be converted in other node (cell or list entry).
  [AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) [createAuthorDocumentFragment](#createAuthorDocumentFragment(ro.sync.ecss.extensions.api.AuthorDocumentController,int,int))([AuthorDocumentController](../../api/AuthorDocumentController.md) controller, int start, int end)
Create the author document fragment to be inserted in a table cell/list item

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ConversionElementHelper

public ConversionElementHelper()

## Method Details

### blockContentMustBeConverted

public abstract boolean blockContentMustBeConverted([AuthorNode](../../api/node/AuthorNode.md) node, [AuthorAccess](../../api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Check if a block node can be converted in other node (cell or list entry). If this method returns false, the block node is treated like an inline node.
  Parameters: node - The node to check authorAccess - The author access Returns: true if the conversion can not be completed for this node Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### createAuthorDocumentFragment

public [AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) createAuthorDocumentFragment([AuthorDocumentController](../../api/AuthorDocumentController.md) controller, int start, int end)throws [AuthorOperationException](../../api/AuthorOperationException.md), [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Create the author document fragment to be inserted in a table cell/list item
  Parameters: controller - The document controller. start - The start offset. end - The end offset. Returns: The fragment. If null, a document fragment from the provided offsets will be created. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the given offset is not in content. [AuthorOperationException](../../api/AuthorOperationException.md) - When the operation could not be completed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
