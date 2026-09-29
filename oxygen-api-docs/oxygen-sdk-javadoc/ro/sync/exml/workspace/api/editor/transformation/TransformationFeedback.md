Package [ro.sync.exml.workspace.api.editor.transformation](package-summary.md)

# Class TransformationFeedback

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.transformation.TransformationFeedback
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public abstract class TransformationFeedback extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Receives feedback from a transformation scenario which is running.
  Since: 15
## Constructor Summary
 Constructors
Constructor

Description
 [TransformationFeedback](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract void [transformationFinished](#transformationFinished(boolean))(boolean success)
Called when the transformation has finished.
  abstract void [transformationStopped](#transformationStopped())()
Called when the transformation was cancelled or stopped by the user

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TransformationFeedback

public TransformationFeedback()

## Method Details

### transformationFinished

public abstract void transformationFinished(boolean success)

Called when the transformation has finished.
  Parameters: success - true if the finished transformation was succesfull.
### transformationStopped

public abstract void transformationStopped()

Called when the transformation was cancelled or stopped by the user

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
