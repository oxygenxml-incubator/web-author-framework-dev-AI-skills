Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface AuthorDocumentProvider
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDocumentProvider
Use this API to access an "in memory" representation of an author document over a resource and customize the document in a non visual way using the [AuthorDocumentController](../AuthorDocumentController.md) and [AuthorDocument](AuthorDocument.md) API.
  Since: 22.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorDocumentController](../AuthorDocumentController.md) [getAuthorDocumentController](#getAuthorDocumentController())()
Access the author document controller.
  [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [getContentInputStream](#getContentInputStream())()
Create an input stream over the nodes structure.
  [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [getContentReader](#getContentReader())()
Create a reader over the nodes structure.
  int[] [getLineColumnMapping](#getLineColumnMapping(int))(int offset)
Map an offset in the Author model to XML line/column.
  [Styles](../../../css/Styles.md) [getStyles](#getStyles(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](AuthorNode.md) node)
Get the CSS styles which are used to render a particular Author node.
  void [save](#save())()
Saves the content to the original load location.

## Method Details

### getAuthorDocumentController

[AuthorDocumentController](../AuthorDocumentController.md) getAuthorDocumentController()

Access the author document controller. You can use it to make changes to the structure of nodes, run XPath expressions to identify nodes and much more.
  Returns: The [AuthorDocumentController](../AuthorDocumentController.md).
### getContentReader

[Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) getContentReader()

Create a reader over the nodes structure.
  Returns: The reader over the created author document.
### getContentInputStream

[InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) getContentInputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Create an input stream over the nodes structure.
  Returns: The input stream over the created author document. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) Since: 23
### save

void save() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Saves the content to the original load location.
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If saving error occurs.
### getStyles

[Styles](../../../css/Styles.md) getStyles([AuthorNode](AuthorNode.md) node)

Get the CSS styles which are used to render a particular Author node. This method **MUST** only be used to query styles.
  Parameters: node - The node for which we want to obtain the styles. Returns: the styles associated with the node or null. Since: 24
### getLineColumnMapping

int[] getLineColumnMapping(int offset)

Map an offset in the Author model to XML line/column.
  Parameters: offset - The offset Returns: The line column mapping or null if it could not be computed. The line is 1 based. Since: 27.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
