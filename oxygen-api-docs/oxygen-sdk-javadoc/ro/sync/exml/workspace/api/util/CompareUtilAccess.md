Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface CompareUtilAccess
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface CompareUtilAccess
Compare utilities.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorDifferencePerformer](../../../../diff/api/AuthorDifferencePerformer.md) [createAuthorDiffPerformer](#createAuthorDiffPerformer())()
Create an Author difference performer.
  [DifferencePerformer](../../../../diff/api/DifferencePerformer.md) [createDiffPerformer](#createDiffPerformer())()
Create difference performer.
  [DiffMergeResult](diff/DiffMergeResult.md) [mergeAuthorContent](#mergeAuthorContent(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String,ro.sync.exml.workspace.api.util.diff.TrackChangesMode))([AuthorAccess](../../../../ecss/extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newContent, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) trackChangesUser, [TrackChangesMode](diff/TrackChangesMode.md) trackChangesMode)
Applies newContent onto the Author document behind authorAccess as a sequence of incremental modifications (delete/insert fragment) computed by diffing, instead of replacing the entire document.
  [MergeResult](../../../../merge/MergeResult.md) [threeWayAutoMerge](#threeWayAutoMerge(java.lang.String,java.lang.String,java.lang.String,ro.sync.merge.MergeConflictResolutionMethods))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ancestor, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) left, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) right, [MergeConflictResolutionMethods](../../../../merge/MergeConflictResolutionMethods.md) conflictResolutionMethod)
Merges two strings representing XML files using a three way merging algorithm which needs an ancestor file.

## Method Details

### threeWayAutoMerge

[MergeResult](../../../../merge/MergeResult.md) threeWayAutoMerge([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ancestor, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) left, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) right, [MergeConflictResolutionMethods](../../../../merge/MergeConflictResolutionMethods.md) conflictResolutionMethod)

Merges two strings representing XML files using a three way merging algorithm which needs an ancestor file.
  Parameters: ancestor - The original file string which has been modified into left and right. left - The left version of the file string, the one with "our" changes. right - The right version of the file string, the one with "others" changes. conflictResolutionMethod - The conflict resolution method to use. Returns: A merged file string where conflicts are resolved by using the left version of the file or null if the merge encountered an error. Since: 17.1
### createDiffPerformer

[DifferencePerformer](../../../../diff/api/DifferencePerformer.md) createDiffPerformer() throws [DiffException](../../../../diff/api/DiffException.md)

Create difference performer.
  Returns: a difference performer that can be used to compare two resources using different algorithms and options. Throws: [DiffException](../../../../diff/api/DiffException.md) - When it fails to create the diff performer. Since: 19.1
### createAuthorDiffPerformer

[AuthorDifferencePerformer](../../../../diff/api/AuthorDifferencePerformer.md) createAuthorDiffPerformer() throws [DiffException](../../../../diff/api/DiffException.md)

Create an Author difference performer.
  Returns: a difference performer that can be used to compare two Author documents using different algorithms and options. Throws: [DiffException](../../../../diff/api/DiffException.md) - When it fails to create the difference performer. Since: 22
### mergeAuthorContent

[DiffMergeResult](diff/DiffMergeResult.md) mergeAuthorContent([AuthorAccess](../../../../ecss/extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newContent, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) trackChangesUser, [TrackChangesMode](diff/TrackChangesMode.md) trackChangesMode)

Applies newContent onto the Author document behind authorAccess as a sequence of incremental modifications (delete/insert fragment) computed by diffing, instead of replacing the entire document. The modifications go through the document's AuthorDocumentController, inside a single compound edit, so any listener attached to the Author document model (for example a Content Fusion concurrent editing room) observes them like normal edits. The current content is read fresh from authorAccess at call time - no separate baseline needed. If applying any of the differences fails, all modifications made so far are rolled back, so the document is either fully updated or left unchanged. Every outcome, including a failure, is reported through the returned [DiffMergeResult](diff/DiffMergeResult.md) - this method does not throw. The merge is declined when the document is read-only. Callers that imposed the read-only state themselves, through WSEditorPage.setReadOnly, must lift it around this call. The whole operation runs on the calling thread, so it must be called on the thread owning the document: the AWT thread in the standalone application, the thread holding the document lock in Web Author.
  Parameters: authorAccess - Access to the Author document to be modified. The location of this document is also used to resolve the relative paths and the DTD references of newContent. newContent - The new content to apply on the document. trackChangesUser - The name recorded on the tracked changes, when the merge is tracked. When null, the reviewer name of the document is used. trackChangesMode - Whether the merge is recorded as tracked changes. When null, [TrackChangesMode.AUTO](diff/TrackChangesMode.md#AUTO) is used. Returns: The merge result, never null. Since: 28.1.0.4  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
