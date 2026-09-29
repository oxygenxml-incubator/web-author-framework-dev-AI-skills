Package [ro.sync.ecss.extensions.api.content](package-summary.md)

# Interface OffsetInformation
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface OffsetInformation
Information about the node which contains the offset. If the offset is on a marker character the returned result will also contain the node which contains the range indicated by the marker.    The author content contains the entire XML document text and special marker characters. Each author node points in the content to the start and end marker characters which are used to delimit it's range. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset() The image represents part of the document content and red markers represent special control characters which represent the node ranges.
  Since: 12.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [IN_CONTENT](#IN_CONTENT)
The offset is in character content.
  static final int [ON_END_MARKER](#ON_END_MARKER)
The offset is on the marker representing the end range of a node.
  static final int [ON_START_MARKER](#ON_START_MARKER)
The offset is on the marker representing the start range of a node.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorNode](../node/AuthorNode.md) [getNodeForMarkerOffset](#getNodeForMarkerOffset())()
If the offset is on a marker character this method returns the node which contains the marker.
  [AuthorNode](../node/AuthorNode.md) [getNodeForOffset](#getNodeForOffset())()
Returns the parent node for the given offset.
  int [getPositionType](#getPositionType())()
Get the type of position the offset has.

## Field Details

### IN_CONTENT

static final int IN_CONTENT

The offset is in character content.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.content.OffsetInformation.IN_CONTENT)

### ON_START_MARKER

static final int ON_START_MARKER

The offset is on the marker representing the start range of a node.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.content.OffsetInformation.ON_START_MARKER)

### ON_END_MARKER

static final int ON_END_MARKER

The offset is on the marker representing the end range of a node.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.content.OffsetInformation.ON_END_MARKER)

## Method Details

### getNodeForMarkerOffset

[AuthorNode](../node/AuthorNode.md) getNodeForMarkerOffset()

If the offset is on a marker character this method returns the node which contains the marker. Example on the situations when this method returns a node:
     Returns: If the offset is on a marker character this method returns the node which contains the marker.
### getNodeForOffset

[AuthorNode](../node/AuthorNode.md) getNodeForOffset()

Returns the parent node for the given offset. Never null.
  Returns: the parent node for the given offset. Never null.
### getPositionType

int getPositionType()

Get the type of position the offset has. It returns one of the constants: [IN_CONTENT](#IN_CONTENT) or [ON_START_MARKER](#ON_START_MARKER) or [ON_END_MARKER](#ON_END_MARKER)
  Returns: the type of position for the offset.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
