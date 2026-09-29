Package [ro.sync.ecss.extensions.api.access](package-summary.md)

# Interface UnsavedContentReferenceManager
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface UnsavedContentReferenceManager
Manager that can be used to find (and save) the resources that have been modified during the editing of a document that contained the expanded references to these resources.
  Since: 23
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[UnsavedReferenceNodeDescriptor](UnsavedReferenceNodeDescriptor.md)> [getUnsavedReferencedNodeDescriptors](#getUnsavedReferencedNodeDescriptors())()
Get the descriptors of nodes that correspond to all unsaved references.
  [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [getUnsavedReferenceInputStream](#getUnsavedReferenceInputStream(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceUrl)
Get the input stream of the specified reference (whose modifications are not saved).
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> [getUnsavedReferencesList](#getUnsavedReferencesList())()
Get the URLs of all the references for which the changes were not saved.
  boolean [isDocumentUnsaved](#isDocumentUnsaved())()

 void [markDocumentAsSaved](#markDocumentAsSaved())()
Mark the document as saved.
  void [markReferenceAsSaved](#markReferenceAsSaved(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceUrl)
Mark the specified reference as saved.

## Method Details

### getUnsavedReferencesList

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> getUnsavedReferencesList()

Get the URLs of all the references for which the changes were not saved.
  Returns: The unsaved references URLs. Can be an empty list if there are no such references.
### getUnsavedReferencedNodeDescriptors

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[UnsavedReferenceNodeDescriptor](UnsavedReferenceNodeDescriptor.md)> getUnsavedReferencedNodeDescriptors()

Get the descriptors of nodes that correspond to all unsaved references.
  Returns: The descriptors of nodes corresponding to all unsaved references. Can be an empty list if there are no such references.
### getUnsavedReferenceInputStream

[InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) getUnsavedReferenceInputStream([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceUrl)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Get the input stream of the specified reference (whose modifications are not saved). This input stream offers the entire content of the reference, with all the unsaved modifications applied.
  Parameters: referenceUrl - The reference URL. Returns: The input stream. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Can be thrown due to incorrect system id, unsupported encodings, files saving permission, etc
### markReferenceAsSaved

void markReferenceAsSaved([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceUrl)

Mark the specified reference as saved. Signal to the application that the reference should now be considered as saved.
  Parameters: referenceUrl - The reference URL.
### isDocumentUnsaved

boolean isDocumentUnsaved()
  Returns: true if the document has unsaved changes that are not inside references.
### markDocumentAsSaved

void markDocumentAsSaved()

Mark the document as saved. Signal to the application that the document should now be considered as saved.
  Since: 23.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
