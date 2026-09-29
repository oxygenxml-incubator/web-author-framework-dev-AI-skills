Package [ro.sync.ecss.extensions.dita.map.topicref](package-summary.md)

# Class TopicrefMoveAction.Builder

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.map.topicref.TopicrefMoveAction.Builder
   Enclosing class: [TopicrefMoveAction](TopicrefMoveAction.md)   public static class TopicrefMoveAction.Builder extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Builder for the TopicrefTransitionOperation. It validates the arguments of the operation

## Constructor Summary
 Constructors
Constructor

Description
 [Builder](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) [authorAccess](#authorAccess(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)
Sets the authorAccess argument.
  [TopicrefMoveAction](TopicrefMoveAction.md) [build](#build())()
Builds a new TopicrefTransitionOperation instance.
  [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) [relativePosition](#relativePosition(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)
Sets the relativePositions argument.
  [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) [sourceLocation](#sourceLocation(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceLocation)
Sets the sourceLocation argument.
  [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) [targetLocation](#targetLocation(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetLocation)
Sets the targetLocation argument.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Builder

public Builder()

## Method Details

### sourceLocation

public [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) sourceLocation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceLocation)

Sets the sourceLocation argument.
  Parameters: sourceLocation - arg. Can be null Returns: this builder
### relativePosition

public [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) relativePosition([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativePosition)

Sets the relativePositions argument.
  Parameters: relativePosition - arg. Cannot be null Returns: this builder
### targetLocation

public [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) targetLocation([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetLocation)

Sets the targetLocation argument.
  Parameters: targetLocation - arg. Cannot be null Returns: this builder
### authorAccess

public [TopicrefMoveAction.Builder](TopicrefMoveAction.Builder.md) authorAccess([AuthorAccess](../../../api/AuthorAccess.md) authorAccess)

Sets the authorAccess argument. Cannot be null
  Parameters: authorAccess -  Returns: this builder
### build

public [TopicrefMoveAction](TopicrefMoveAction.md) build()

Builds a new TopicrefTransitionOperation instance. It validates the arguments
  Returns: the newly created operation
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
