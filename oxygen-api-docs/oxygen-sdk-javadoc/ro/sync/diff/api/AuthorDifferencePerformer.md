Package [ro.sync.diff.api](package-summary.md)

# Interface AuthorDifferencePerformer
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDifferencePerformer
The [AuthorDifferencePerformer](AuthorDifferencePerformer.md) is used to compare two Author documents using a set of options. The result of the diff is a list with the differences between the resources.
  Since: 22
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Difference](Difference.md)> [performDiff](#performDiff(ro.sync.diff.api.DiffProgressListener))([DiffProgressListener](DiffProgressListener.md) diffProgressListener)
Performs the diff operation between the resources represented by the two AuthorAccess.
  void [setBaseDocument](#setBaseDocument(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../ecss/extensions/api/AuthorAccess.md) baseAuthorAccess)
Set the base Author document, used to perform a three-way comparison.
  void [setDocumentsToCompare](#setDocumentsToCompare(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../ecss/extensions/api/AuthorAccess.md) leftAuthorAccess, [AuthorAccess](../../ecss/extensions/api/AuthorAccess.md) rightAuthorAccess)
Set the documents to be compared.
  void [setOptions](#setOptions(ro.sync.diff.api.DiffOptions))([DiffOptions](DiffOptions.md) diffOptions)
Set the options used by the diff performer to perform the comparison.
  void [stop](#stop())()
Signal to the diff performer that it must stop.

## Method Details

### setBaseDocument

void setBaseDocument([AuthorAccess](../../ecss/extensions/api/AuthorAccess.md) baseAuthorAccess)

Set the base Author document, used to perform a three-way comparison. It can be null.
  Parameters: baseAuthorAccess - The access to the base Author document.
### setDocumentsToCompare

void setDocumentsToCompare([AuthorAccess](../../ecss/extensions/api/AuthorAccess.md) leftAuthorAccess, [AuthorAccess](../../ecss/extensions/api/AuthorAccess.md) rightAuthorAccess)

Set the documents to be compared.
  Parameters: leftAuthorAccess - The access to the left Author document. rightAuthorAccess - The access to the right Author document.
### setOptions

void setOptions([DiffOptions](DiffOptions.md) diffOptions)

Set the options used by the diff performer to perform the comparison. It can be null meaning a default set of options will be used.
  Parameters: diffOptions - The options.
### performDiff

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Difference](Difference.md)> performDiff([DiffProgressListener](DiffProgressListener.md) diffProgressListener)throws [DiffException](DiffException.md), [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Performs the diff operation between the resources represented by the two AuthorAccess.
  Parameters: diffProgressListener - The [DiffProgressListener](DiffProgressListener.md) notified about the progress of the diff. It can be null when the diff progress doesn't need to be monitored. Returns: The list with the differences. If the resources are identical or the diff fails the list will be empty.  The returned differences are represented by [Difference](Difference.md) objects that contain the start and end offsets in the Author content for each Author document. The Author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset() The following image represents the architecture of an Author document fragment that is a part of the Author document content. The red markers represent special control characters which represent the node ranges:    If the hierarchical diff is activated ([DiffOptions.isEnableHierarchicalDiff()](DiffOptions.md#isEnableHierarchicalDiff()) returns true) then the returned list contains [DifferenceParent](DifferenceParent.md) elements. Throws: [DiffException](DiffException.md) - If the diff operation fails or it is stopped before it finishes. [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### stop

void stop()

Signal to the diff performer that it must stop.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
