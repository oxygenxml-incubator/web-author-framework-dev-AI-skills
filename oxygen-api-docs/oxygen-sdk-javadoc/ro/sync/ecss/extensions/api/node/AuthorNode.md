Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface AuthorNode
    All Known Subinterfaces: [AuthorDocument](AuthorDocument.md), [AuthorElement](AuthorElement.md), [AuthorElementBaseInterface](../AuthorElementBaseInterface.md), [AuthorParentNode](AuthorParentNode.md), [AuthorReferenceNode](AuthorReferenceNode.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorNode
Base interface for all Author nodes. The Author nodes model is similar with the DOM model with the difference that the TEXT nodes do not exists in this model. The text from the document is kept separately into a data structure similar to Content from Swing. The nodes have start and end pointers into the Content, see [getStartOffset()](#getStartOffset())and [getEndOffset()](#getEndOffset()) methods. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range.   The image represents part of the document content and red markers represent special control characters which represent the node ranges.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NODE_NAME_CDATA](#NODE_NAME_CDATA)
Name of CDATA node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NODE_NAME_COMMENT](#NODE_NAME_COMMENT)
Name of COMMENT node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NODE_NAME_DOCUMENT](#NODE_NAME_DOCUMENT)
Name of DOCUMENT node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NODE_NAME_PI](#NODE_NAME_PI)
Name of PI node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NODE_NAME_REFERENCE](#NODE_NAME_REFERENCE)
Name of the reference node.
  static final int [NODE_TYPE_CDATA](#NODE_TYPE_CDATA)
CDATA node type.
  static final int [NODE_TYPE_COMMENT](#NODE_TYPE_COMMENT)
Comment node type.
  static final int [NODE_TYPE_DOCUMENT](#NODE_TYPE_DOCUMENT)
Document node type.
  static final int [NODE_TYPE_ELEMENT](#NODE_TYPE_ELEMENT)
Element node type.
  static final int [NODE_TYPE_PI](#NODE_TYPE_PI)
Processing instruction node type.
  static final int [NODE_TYPE_PSEUDO_DOCTYPE](#NODE_TYPE_PSEUDO_DOCTYPE)
Pseudo DOCTYPE node type.
  static final int [NODE_TYPE_PSEUDO_ELEMENT](#NODE_TYPE_PSEUDO_ELEMENT)
Pseudo element node type.
  static final int [NODE_TYPE_REFERENCE](#NODE_TYPE_REFERENCE)
Reference node type (entity or other reference nodes, e.g.
  static final int [NODE_TYPE_TEXT](#NODE_TYPE_TEXT)
Text node type.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [ContentIterator](ContentIterator.md) [getContentIterator](#getContentIterator())()
Return an iterator over the text content of this node.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName())()
Returns the display name of the node used for visual representation.
  int [getEndOffset](#getEndOffset())()
Returns the offset in the content which marks the end of the node's range.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Returns the node name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNamespace](#getNamespace())()

 [NamespaceContext](NamespaceContext.md) [getNamespaceContext](#getNamespaceContext())()
Obtain access to the mappings from prefix to namespace and from namespace to prefix in the context of the current element.
  [AuthorDocument](AuthorDocument.md) [getOwnerDocument](#getOwnerDocument())()
Returns the document to which this element belongs.
  [AuthorNode](AuthorNode.md) [getParent](#getParent())()

 int [getStartOffset](#getStartOffset())()
Returns the offset in the content which marks the start of the node's range.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTextContent](#getTextContent())()
Returns the nodes text content.
  int [getType](#getType())()
Returns the node type.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getXMLBaseURL](#getXMLBaseURL())()
The returned URL represents the value of base URL in the current nodes context.
  boolean [isDescendentOf](#isDescendentOf(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](AuthorNode.md) ancestor)
See if this node is a descendant of the given node.

## Field Details

### NODE_TYPE_ELEMENT

static final int NODE_TYPE_ELEMENT

Element node type. The value is 0.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_ELEMENT)

### NODE_TYPE_TEXT

static final int NODE_TYPE_TEXT

Text node type. The value is 1.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_TEXT)

### NODE_TYPE_DOCUMENT

static final int NODE_TYPE_DOCUMENT

Document node type. The value is 2.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_DOCUMENT)

### NODE_TYPE_COMMENT

static final int NODE_TYPE_COMMENT

Comment node type. The value is 3.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_COMMENT)

### NODE_TYPE_CDATA

static final int NODE_TYPE_CDATA

CDATA node type. The value is 4.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_CDATA)

### NODE_TYPE_PI

static final int NODE_TYPE_PI

Processing instruction node type. The value is 5.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_PI)

### NODE_TYPE_PSEUDO_ELEMENT

static final int NODE_TYPE_PSEUDO_ELEMENT

Pseudo element node type. The value is 6.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_PSEUDO_ELEMENT)

### NODE_TYPE_REFERENCE

static final int NODE_TYPE_REFERENCE

Reference node type (entity or other reference nodes, e.g. xinclude elements). The value is 7.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_REFERENCE)

### NODE_TYPE_PSEUDO_DOCTYPE

static final int NODE_TYPE_PSEUDO_DOCTYPE

Pseudo DOCTYPE node type. The value is 8.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_TYPE_PSEUDO_DOCTYPE)

### NODE_NAME_CDATA

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NODE_NAME_CDATA

Name of CDATA node. The value is #cdata.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_NAME_CDATA)

### NODE_NAME_COMMENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NODE_NAME_COMMENT

Name of COMMENT node. The value is #comment.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_NAME_COMMENT)

### NODE_NAME_DOCUMENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NODE_NAME_DOCUMENT

Name of DOCUMENT node. The value is #document.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_NAME_DOCUMENT)

### NODE_NAME_PI

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NODE_NAME_PI

Name of PI node. The value is processing-instruction.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_NAME_PI)

### NODE_NAME_REFERENCE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NODE_NAME_REFERENCE

Name of the reference node.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorNode.NODE_NAME_REFERENCE)

## Method Details

### getOwnerDocument

[AuthorDocument](AuthorDocument.md) getOwnerDocument()

Returns the document to which this element belongs.
  Returns: The [AuthorDocument](AuthorDocument.md) to which this element belongs. Returns null if this element is part of a document fragment. For more details see [AuthorDocumentFragment](AuthorDocumentFragment.md).
### isDescendentOf

boolean isDescendentOf([AuthorNode](AuthorNode.md) ancestor)

See if this node is a descendant of the given node.
  Parameters: ancestor - The [AuthorNode](AuthorNode.md) tested to see if it is an ancestor of this node. Returns: true if the given node is an ancestor of this node.
### getType

int getType()

Returns the node type. Can be one of the constants: [NODE_TYPE_CDATA](#NODE_TYPE_CDATA), [NODE_TYPE_COMMENT](#NODE_TYPE_COMMENT), [NODE_TYPE_DOCUMENT](#NODE_TYPE_DOCUMENT), [NODE_TYPE_ELEMENT](#NODE_TYPE_ELEMENT), [NODE_TYPE_PI](#NODE_TYPE_PI), [NODE_TYPE_PSEUDO_DOCTYPE](#NODE_TYPE_PSEUDO_DOCTYPE), [NODE_TYPE_PSEUDO_ELEMENT](#NODE_TYPE_PSEUDO_ELEMENT), [NODE_TYPE_REFERENCE](#NODE_TYPE_REFERENCE).
  Returns: The node type.
### getStartOffset

int getStartOffset()

Returns the offset in the content which marks the start of the node's range. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range.   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Returns: The offset into the content corresponding to the start of the node, 0 based and inclusive.
### getEndOffset

int getEndOffset()

Returns the offset in the content which marks the end of the node's range. The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range.   The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Returns: The offset into the content corresponding to the end of the node, 0 based and inclusive.
### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Returns the node name. Depending on the node type the method returns:
        * [NODE_TYPE_ELEMENT](#NODE_TYPE_ELEMENT) - the qualified name of the element
        * [NODE_TYPE_CDATA](#NODE_TYPE_CDATA) - the constant [NODE_NAME_CDATA](#NODE_NAME_CDATA)
        * [NODE_TYPE_COMMENT](#NODE_TYPE_COMMENT) - the constant [NODE_NAME_COMMENT](#NODE_NAME_COMMENT)
        * [NODE_TYPE_DOCUMENT](#NODE_TYPE_DOCUMENT) - the constant [NODE_NAME_DOCUMENT](#NODE_NAME_DOCUMENT)
        * [NODE_TYPE_REFERENCE](#NODE_TYPE_REFERENCE) - the name of the entity
        * [NODE_TYPE_PI](#NODE_TYPE_PI) - the constant [NODE_NAME_PI](#NODE_NAME_PI)

  Returns: The name of the node.
### getParent

[AuthorNode](AuthorNode.md) getParent()
  Returns: The [AuthorNode](AuthorNode.md) representing the parent of this element, or null if this is the document node.
### getDisplayName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName()

Returns the display name of the node used for visual representation.
  Returns: The display name.
### getXMLBaseURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getXMLBaseURL()

The returned URL represents the value of base URL in the current nodes context. It is resolved taking into account the values of all the 'xml:base' attributes from the ancestors and the document URL if necessary.
If no 'xml:base' attribute is present, the document system ID will be returned. See specification: [http://www.w3.org/TR/xmlbase/](http://www.w3.org/TR/xmlbase/).

  Returns: The XML base URL.
### getTextContent

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTextContent() throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Returns the nodes text content. The returned value is obtained by adding all the descendants text content. The special sentinel characters are removed.
  Returns: The node text content. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If the text content cannot be obtained.
### getContentIterator

[ContentIterator](ContentIterator.md) getContentIterator()

Return an iterator over the text content of this node.

The content may contain special characters which have the value equal to 0. These special characters are the markers for content referenced by descendant nodes.

More about how Author Nodes point to the content:
  Returns: an iterator over the text content of this node. Since: 22
### getNamespace

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNamespace()
  Returns: The node's namespace
### getNamespaceContext

[NamespaceContext](NamespaceContext.md) getNamespaceContext()

Obtain access to the mappings from prefix to namespace and from namespace to prefix in the context of the current element.
  Returns: mappings from prefix to namespace and from namespace to prefix in the context of the current element. Since: 13
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
