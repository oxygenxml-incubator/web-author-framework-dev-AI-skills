Package [ro.sync.net.protocol](package-summary.md)

# Interface FileBrowsingConnection
    All Known Implementing Classes: [FilterURLConnection](../../ecss/extensions/api/webapp/plugin/FilterURLConnection.md)   @API(src=PUBLIC, type=EXTENDABLE) public interface FileBrowsingConnection
Interface implemented by an URLConnection class that supports file browsing.
  Since: 17.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[FolderEntryDescriptor](FolderEntryDescriptor.md)> [listFolder](#listFolder())()
Retrieves all children of the directory identified by the URL on which this connection is made.

## Method Details

### listFolder

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[FolderEntryDescriptor](FolderEntryDescriptor.md)> listFolder() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [UserActionRequiredException](../../ecss/extensions/api/webapp/plugin/UserActionRequiredException.md)

Retrieves all children of the directory identified by the URL on which this connection is made.
  Returns: For list of descriptors for each folder entry. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the remote server could not return a list of children. [UserActionRequiredException](../../ecss/extensions/api/webapp/plugin/UserActionRequiredException.md) - Whether the browsing requires user interaction, like login.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
