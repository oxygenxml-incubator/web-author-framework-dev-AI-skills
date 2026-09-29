Package [ro.sync.diff.api](package-summary.md)

# Interface AuthorDiffChangeTrackingMerger
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDiffChangeTrackingMerger
Extracts the differences reported when comparing two XML documents ('Two-Way' Author comparison mode) as a document with change tracking, which can be used to review the differences and merge the two documents. Access to the resulting document is provided through a [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) for its content.
  Since: 26.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [getMergeResultsReader](#getMergeResultsReader(java.net.URL,java.io.Reader,java.net.URL,java.io.Reader,ro.sync.diff.api.DiffOptions))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseDocSysID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) baseDocReader, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) docToMergeWithSysID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docToMergeWithReader, [DiffOptions](DiffOptions.md) diffOptions)
Gets the results of the comparison between two XML documents ('Two-Way' Author comparison mode) as a [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) for the contents of the resulted document with change tracking, which can be used to review the differences and merge the two documents. **Important note:**  If the documents to be compared already contain tracked changes, all such changes are automatically accepted before the comparison and the generation of the resulting document.
  void [setNameOfAuthorOfChangeTrackingMarkers](#setNameOfAuthorOfChangeTrackingMarkers(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) authorName)
Sets the name of the author of the change tracking markers created in the merged document.

## Method Details

### getMergeResultsReader

[Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) getMergeResultsReader([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseDocSysID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) baseDocReader, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) docToMergeWithSysID, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) docToMergeWithReader, [DiffOptions](DiffOptions.md) diffOptions)throws [DiffException](DiffException.md)

Gets the results of the comparison between two XML documents ('Two-Way' Author comparison mode) as a [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) for the contents of the resulted document with change tracking, which can be used to review the differences and merge the two documents. **Important note:**  If the documents to be compared already contain tracked changes, all such changes are automatically accepted before the comparison and the generation of the resulting document.
  Parameters: baseDocSysID - The system ID of the base document.  Can be null, but only in case of **baseDocReader** provided. baseDocReader - The [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) for the base document.  If null and **baseDocSysID** provided, the reader will be created internally.  If both **baseDocReader** and **baseDocSysID** are null, a [DiffException](DiffException.md) is thrown. docToMergeWithSysID - The system ID of the document to merge with.  Can be null, but only in case of **docToMergeWithReader** provided. docToMergeWithReader - The [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) for the document to merge with.  If null and **docToMergeWithSysID** provided, the reader will be created internally.  If both **docToMergeWithReader** and **docToMergeWithSysID** are null, a [DiffException](DiffException.md) is thrown. diffOptions - The [DiffOptions](DiffOptions.md) used to decide which comparing algorithm and which comparing options to use.   Can be null in which case the comparison algorithm is chosen automatically and the default comparison options are used. Returns: A [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) for the contents of the resulted document with change tracking which can be used to review the differences and merge the two documents provided for comparison. Throws: [DiffException](DiffException.md) - If something went wrong while generating the resulting document.
### setNameOfAuthorOfChangeTrackingMarkers

void setNameOfAuthorOfChangeTrackingMarkers([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) authorName)

Sets the name of the author of the change tracking markers created in the merged document. This name will be post-fixed with the " [Auto Merger]" construct, in order to make a clear association between the author and an imposed/fixed color used for highlighting track changes when loading the merged document in Oxygen.
  Parameters: authorName - The name of the author of the change tracking markers created in the merged document. Can be null, in which case the default name "Auto Merger" is used.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
