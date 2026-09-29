Package [ro.sync.ecss.extensions.dita.map.topicref](package-summary.md)

# Class TopicrefMoveAction

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.map.topicref.TopicrefMoveAction
   @API(type=INTERNAL, src=PUBLIC) public class TopicrefMoveAction extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Promotes or demotes a topicref. The type of transition is generic and depends on the insertion position and target XPath location

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static class  [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md)
Builder for the TopicrefTransitionOperation.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) [builder](#builder())()
Returns a new builder for this operation
  void [execute](#execute())()
Executes the transition operation.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### execute

public void execute() throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Executes the transition operation.
  Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) [AuthorOperationException](../../../api/AuthorOperationException.md)
### builder

public static [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) builder()

Returns a new builder for this operation
  Returns: the builder
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
