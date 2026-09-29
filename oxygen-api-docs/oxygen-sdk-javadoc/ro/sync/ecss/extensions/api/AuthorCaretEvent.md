Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorCaretEvent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorCaretEvent
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorCaretEvent extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
AuthorCaretEvent is used to notify interested [AuthorCaretListener](AuthorCaretListener.md) that the position of the caret has changed in the Author editor page.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorCaretEvent](#%3Cinit%3E(int,java.util.List,ro.sync.ecss.extensions.api.node.AuthorNode))(int offset, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> selectionIntervals, [AuthorNode](node/AuthorNode.md) node)
Constructor for the AuthorCaretEvent.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorNode](node/AuthorNode.md) [getNode](#getNode())()

 int [getOffset](#getOffset())()

 int [getSelectionEnd](#getSelectionEnd())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> [getSelectionIntervals](#getSelectionIntervals())()
Get the selection [start offset, end offset] intervals list.
  int [getSelectionStart](#getSelectionStart())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorCaretEvent

public AuthorCaretEvent(int offset, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> selectionIntervals, [AuthorNode](node/AuthorNode.md) node)

Constructor for the AuthorCaretEvent.
  Parameters: offset - The absolute caret position inside the Author page. selectionIntervals - The selection [start offset, end offset] intervals list. If there is no selection the list contains a single entry with [caret offset, caret offset]. node - The node holding the caret offset.
## Method Details

### getOffset

public int getOffset()
  Returns: Returns the absolute caret offset.
### getNode

public [AuthorNode](node/AuthorNode.md) getNode()
  Returns: Returns the node holding the caret position.
### getSelectionStart

public int getSelectionStart()
  Returns: Returns the selection start offset, inclusive. If no selection the selection start is equals with caret offset.
### getSelectionEnd

public int getSelectionEnd()
  Returns: Returns the selection end offset, exclusive. If no selection the selection end is equals with caret offset.
### getSelectionIntervals

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<int[]> getSelectionIntervals()

Get the selection [start offset, end offset] intervals list. If there is no selection the list contains a single [caret offset, caret offset] entry.
  Returns: Returns the list of selection intervals.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
