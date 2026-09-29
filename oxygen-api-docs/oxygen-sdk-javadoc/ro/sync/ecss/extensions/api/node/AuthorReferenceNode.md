Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface AuthorReferenceNode
    All Superinterfaces: [AuthorNode](AuthorNode.md), [AuthorParentNode](AuthorParentNode.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorReferenceNodeextends [AuthorParentNode](AuthorParentNode.md)
Interface for reference nodes that have a content expanded when displayed in the Author mode.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTR_NAME_ALLOWS_VALIDATION](#ATTR_NAME_ALLOWS_VALIDATION)
Allows Validation attribute name
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTR_NAME_CHANGE_TRACK_COUNT](#ATTR_NAME_CHANGE_TRACK_COUNT)
Number of track changes
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTR_NAME_COMMENTS_COUNTS](#ATTR_NAME_COMMENTS_COUNTS)
Number of comments
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTR_NAME_EDITABLE](#ATTR_NAME_EDITABLE)
Editable attribute name
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTR_NAME_TEXT_BEFORE_ROOT](#ATTR_NAME_TEXT_BEFORE_ROOT)
Text before root.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [HREF](#HREF)
Href.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXYGEN_NAMESPACE](#OXYGEN_NAMESPACE)
The Oxygen namespace.
  static final int [REFERENCE_TYPE_ENTITY](#REFERENCE_TYPE_ENTITY)
Entities reference nodes type.
  static final int [REFERENCE_TYPE_SYNTHETIC](#REFERENCE_TYPE_SYNTHETIC)
Synthetic reference nodes type (e.g.

### Fields inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [NODE_NAME_CDATA](AuthorNode.md#NODE_NAME_CDATA), [NODE_NAME_COMMENT](AuthorNode.md#NODE_NAME_COMMENT), [NODE_NAME_DOCUMENT](AuthorNode.md#NODE_NAME_DOCUMENT), [NODE_NAME_PI](AuthorNode.md#NODE_NAME_PI), [NODE_NAME_REFERENCE](AuthorNode.md#NODE_NAME_REFERENCE), [NODE_TYPE_CDATA](AuthorNode.md#NODE_TYPE_CDATA), [NODE_TYPE_COMMENT](AuthorNode.md#NODE_TYPE_COMMENT), [NODE_TYPE_DOCUMENT](AuthorNode.md#NODE_TYPE_DOCUMENT), [NODE_TYPE_ELEMENT](AuthorNode.md#NODE_TYPE_ELEMENT), [NODE_TYPE_PI](AuthorNode.md#NODE_TYPE_PI), [NODE_TYPE_PSEUDO_DOCTYPE](AuthorNode.md#NODE_TYPE_PSEUDO_DOCTYPE), [NODE_TYPE_PSEUDO_ELEMENT](AuthorNode.md#NODE_TYPE_PSEUDO_ELEMENT), [NODE_TYPE_REFERENCE](AuthorNode.md#NODE_TYPE_REFERENCE), [NODE_TYPE_TEXT](AuthorNode.md#NODE_TYPE_TEXT)
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getReferenceType](#getReferenceType())()
Returns the type of the reference.

### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorNode](AuthorNode.md)
 [getContentIterator](AuthorNode.md#getContentIterator()), [getDisplayName](AuthorNode.md#getDisplayName()), [getEndOffset](AuthorNode.md#getEndOffset()), [getName](AuthorNode.md#getName()), [getNamespace](AuthorNode.md#getNamespace()), [getNamespaceContext](AuthorNode.md#getNamespaceContext()), [getOwnerDocument](AuthorNode.md#getOwnerDocument()), [getParent](AuthorNode.md#getParent()), [getStartOffset](AuthorNode.md#getStartOffset()), [getTextContent](AuthorNode.md#getTextContent()), [getType](AuthorNode.md#getType()), [getXMLBaseURL](AuthorNode.md#getXMLBaseURL()), [isDescendentOf](AuthorNode.md#isDescendentOf(ro.sync.ecss.extensions.api.node.AuthorNode))
### Methods inherited from interface ro.sync.ecss.extensions.api.node.[AuthorParentNode](AuthorParentNode.md)
 [getContentNodes](AuthorParentNode.md#getContentNodes()), [getParentElement](AuthorParentNode.md#getParentElement())
## Field Details

### REFERENCE_TYPE_ENTITY

static final int REFERENCE_TYPE_ENTITY

Entities reference nodes type. The value is 0.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.REFERENCE_TYPE_ENTITY)

### REFERENCE_TYPE_SYNTHETIC

static final int REFERENCE_TYPE_SYNTHETIC

Synthetic reference nodes type (e.g. XInclude elements). The value is 1.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.REFERENCE_TYPE_SYNTHETIC)

### HREF

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) HREF

Href.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.HREF)

### ATTR_NAME_CHANGE_TRACK_COUNT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTR_NAME_CHANGE_TRACK_COUNT

Number of track changes
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.ATTR_NAME_CHANGE_TRACK_COUNT)

### ATTR_NAME_COMMENTS_COUNTS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTR_NAME_COMMENTS_COUNTS

Number of comments
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.ATTR_NAME_COMMENTS_COUNTS)

### ATTR_NAME_EDITABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTR_NAME_EDITABLE

Editable attribute name
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.ATTR_NAME_EDITABLE)

### ATTR_NAME_ALLOWS_VALIDATION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTR_NAME_ALLOWS_VALIDATION

Allows Validation attribute name
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.ATTR_NAME_ALLOWS_VALIDATION)

### ATTR_NAME_TEXT_BEFORE_ROOT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTR_NAME_TEXT_BEFORE_ROOT

Text before root. Includes the root element.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.ATTR_NAME_TEXT_BEFORE_ROOT)

### OXYGEN_NAMESPACE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXYGEN_NAMESPACE

The Oxygen namespace.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.node.AuthorReferenceNode.OXYGEN_NAMESPACE)

## Method Details

### getReferenceType

int getReferenceType()

Returns the type of the reference. Used to differentiate between XML entities and other reference (e.g. XInclude elements).
  Returns: The type of the reference. One of the two constants: [REFERENCE_TYPE_ENTITY](#REFERENCE_TYPE_ENTITY), [REFERENCE_TYPE_SYNTHETIC](#REFERENCE_TYPE_SYNTHETIC).
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
