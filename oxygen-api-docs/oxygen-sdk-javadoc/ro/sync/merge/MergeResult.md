Package [ro.sync.merge](package-summary.md)

# Class MergeResult

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.merge.MergeResult
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class MergeResult extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Defines the result of a three way merge.
  Since: 18.0
## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [MergeResult.ResultType](MergeResult.ResultType.md)
The way a merge has finalized.

## Constructor Summary
 Constructors
Constructor

Description
 [MergeResult](#%3Cinit%3E())()
No arguments constructor.
  [MergeResult](#%3Cinit%3E(ro.sync.merge.MergeResult.ResultType,java.lang.String))([MergeResult.ResultType](MergeResult.ResultType.md) resultType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mergedString)
Constructor.
  [MergeResult](#%3Cinit%3E(ro.sync.merge.MergeResult.ResultType,java.lang.String,java.lang.Boolean))([MergeResult.ResultType](MergeResult.ResultType.md) resultType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mergedString, [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) mergingOccurred)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMergedString](#getMergedString())()

 [MergeResult.ResultType](MergeResult.ResultType.md) [getResultType](#getResultType())()

 boolean [mergingOccurred](#mergingOccurred())()

 void [setMergedString](#setMergedString(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mergedString)
Sets the value of the merged string.
  void [setResultType](#setResultType(ro.sync.merge.MergeResult.ResultType))([MergeResult.ResultType](MergeResult.ResultType.md) result)
Sets the new value of the result type.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### MergeResult

public MergeResult([MergeResult.ResultType](MergeResult.ResultType.md) resultType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mergedString)

Constructor.
  Parameters: resultType - The type of the merge result. mergedString - The merged string.
### MergeResult

public MergeResult([MergeResult.ResultType](MergeResult.ResultType.md) resultType, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mergedString, [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) mergingOccurred)

Constructor.
  Parameters: resultType - The type of the merge result. mergedString - The merged string. mergingOccurred - Flag telling whether merging occurred or not. If the two left|right files were identical mergingOccurred will be false;
### MergeResult

public MergeResult()

No arguments constructor.

## Method Details

### mergingOccurred

public boolean mergingOccurred()
  Returns: true if merging happened, or false if no merging happened because the given left|right files were identical.
### getMergedString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMergedString()
  Returns: The merged string.
### setMergedString

public void setMergedString([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) mergedString)

Sets the value of the merged string.
  Parameters: mergedString - The new merged string.
### getResultType

public [MergeResult.ResultType](MergeResult.ResultType.md) getResultType()
  Returns: The type of the result.
### setResultType

public void setResultType([MergeResult.ResultType](MergeResult.ResultType.md) result)

Sets the new value of the result type.
  Parameters: result - The new value of the result type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
