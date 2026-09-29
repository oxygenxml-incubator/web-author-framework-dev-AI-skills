Package [ro.sync.exml.workspace.api.util.diff](package-summary.md)

# Class DiffMergeResult

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.util.diff.DiffMergeResult
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class DiffMergeResult extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The result of merging new content over an Author document using [CompareUtilAccess.mergeAuthorContent(ro.sync.ecss.extensions.api.AuthorAccess, java.lang.String, java.lang.String, ro.sync.exml.workspace.api.util.diff.TrackChangesMode)](../CompareUtilAccess.md#mergeAuthorContent(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.exml.workspace.api.util.diff.TrackChangesMode)).
  Since: 29  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [DiffMergeResult.ResultType](DiffMergeResult.ResultType.md)
The type of the merge result.

## Constructor Summary
 Constructors
Constructor

Description
 [DiffMergeResult](#%3Cinit%3E(ro.sync.exml.workspace.api.util.diff.DiffMergeResult.ResultType,int,java.lang.String))([DiffMergeResult.ResultType](DiffMergeResult.ResultType.md) resultType, int hunksApplied, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getChunksApplied](#getChunksApplied())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getErrorMessage](#getErrorMessage())()

 [DiffMergeResult.ResultType](DiffMergeResult.ResultType.md) [getResultType](#getResultType())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DiffMergeResult

public DiffMergeResult([DiffMergeResult.ResultType](DiffMergeResult.ResultType.md) resultType, int hunksApplied, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage)

Constructor.
  Parameters: resultType - The type of this result. hunksApplied - The number of difference hunks applied on the live document. errorMessage - The error message, in case the merge did not succeed. null when the merge succeeded.
## Method Details

### getResultType

public [DiffMergeResult.ResultType](DiffMergeResult.ResultType.md) getResultType()
  Returns: The type of this result.
### getChunksApplied

public int getChunksApplied()
  Returns: The number of difference hunks applied on the live document.
### getErrorMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getErrorMessage()
  Returns: The error message, in case the merge did not succeed. null when the merge succeeded.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
