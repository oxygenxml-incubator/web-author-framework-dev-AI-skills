Package [ro.sync.diff.merge.api](package-summary.md)

# Interface MergedFileState
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface MergedFileState
The state of a merged file contains information about the file location and the merge status (deleted, added, modified). The file location is child of the the directory containing the personal changes (the directory specified in the **personalModifiedFilesDir** parameter of [DiffAndMergeTools.openMergeApplication(java.io.File, java.io.File, java.io.File, java.util.Map)](../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openMergeApplication(java.io.File,java.io.File,java.io.File,java.util.Map))) .

## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [MergedFileState.MergeStatus](MergedFileState.MergeStatus.md)
The merge state

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getFile](#getFile())()
Get the path to the altered file.
  [MergedFileState.MergeStatus](MergedFileState.MergeStatus.md) [getFileModifiedStatus](#getFileModifiedStatus())()
Get the type of change done to the altered file.

## Method Details

### getFile

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getFile()

Get the path to the altered file.
  Returns: The file from the personal changes directory that was altered. (the directory specified in the **personalModifiedFilesDir** parameter of [DiffAndMergeTools.openMergeApplication(java.io.File, java.io.File, java.io.File, java.util.Map)](../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openMergeApplication(java.io.File,java.io.File,java.io.File,java.util.Map))) .
### getFileModifiedStatus

[MergedFileState.MergeStatus](MergedFileState.MergeStatus.md) getFileModifiedStatus()

Get the type of change done to the altered file.
  Returns: The current merge file state.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
