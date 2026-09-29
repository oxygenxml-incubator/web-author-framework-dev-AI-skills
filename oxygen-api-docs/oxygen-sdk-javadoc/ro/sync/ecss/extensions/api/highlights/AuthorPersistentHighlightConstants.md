Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface AuthorPersistentHighlightConstants
    All Known Subinterfaces: [AuthorPersistentHighlight](AuthorPersistentHighlight.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorPersistentHighlightConstants
Constants used in the serialization process of the Author Persistent Highlights.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ATTR_NAME_ATTRIBUTE](#ATTR_NAME_ATTRIBUTE)
The name of the attribute holding the name of the changed attribute.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTHOR_NAME_ATTRIBUTE](#AUTHOR_NAME_ATTRIBUTE)
The pseudo attribute name of the PI holding the name of the author who made the modification.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COMMENT_ATTRIBUTE](#COMMENT_ATTRIBUTE)
The pseudo attribute name of the PI holding the comment of the author who made the modification.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COMMENT_ID](#COMMENT_ID)
The pseudo attribute name of the PI holding the id of the comment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COMMENT_PARENT_ID](#COMMENT_PARENT_ID)
The pseudo attribute name of the PI holding the parent id.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CONTENT_ATTRIBUTE](#CONTENT_ATTRIBUTE)
The pseudo attribute name (of the delete PI) holding the deleted content.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DONE_ATTRIBUTE_VALUE](#DONE_ATTRIBUTE_VALUE)
One of the values for [FLAG_ATTRIBUTE](#FLAG_ATTRIBUTE).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EMPTY_MARKER_ATTRIBUTE](#EMPTY_MARKER_ATTRIBUTE)
The name of the attribute that specifies that a marker is not over any content...
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FLAG_ATTRIBUTE](#FLAG_ATTRIBUTE)
The pseudo attribute name of the PI holding the flag of the marker.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MID_ATTRIBUTE](#MID_ATTRIBUTE)
The name of the id attribute which identifies start and end PI markers when they overlap.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MODIFICATION_TIME](#MODIFICATION_TIME)
The pseudo attribute name of the PI holding the modification time.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_ATTRIBUTE](#TYPE_ATTRIBUTE)
The name of the attribute holding the type of the change.

## Field Details

### AUTHOR_NAME_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTHOR_NAME_ATTRIBUTE

The pseudo attribute name of the PI holding the name of the author who made the modification. The value is author.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.AUTHOR_NAME_ATTRIBUTE)

### COMMENT_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COMMENT_ATTRIBUTE

The pseudo attribute name of the PI holding the comment of the author who made the modification. The value is comment.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.COMMENT_ATTRIBUTE)

### MODIFICATION_TIME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MODIFICATION_TIME

The pseudo attribute name of the PI holding the modification time. The value is timestamp.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.MODIFICATION_TIME)

### COMMENT_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COMMENT_ID

The pseudo attribute name of the PI holding the id of the comment. This is first set when a reply is added to the highlight, and will be used as parent id for all its replies. The value is id.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.COMMENT_ID)

### COMMENT_PARENT_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COMMENT_PARENT_ID

The pseudo attribute name of the PI holding the parent id. The parent ID is set on a comment that is a reply to another highlight. Its value is the same as the value of the parent's [COMMENT_ID](#COMMENT_ID) property value. The value is parentID.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.COMMENT_PARENT_ID)

### FLAG_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FLAG_ATTRIBUTE

The pseudo attribute name of the PI holding the flag of the marker. Can have multiple values. One of the values can be ["done"](#DONE_ATTRIBUTE_VALUE)
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.FLAG_ATTRIBUTE)

### DONE_ATTRIBUTE_VALUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DONE_ATTRIBUTE_VALUE

One of the values for [FLAG_ATTRIBUTE](#FLAG_ATTRIBUTE). The value is done.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.DONE_ATTRIBUTE_VALUE)

### CONTENT_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CONTENT_ATTRIBUTE

The pseudo attribute name (of the delete PI) holding the deleted content. The value is content.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.CONTENT_ATTRIBUTE)

### MID_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MID_ATTRIBUTE

The name of the id attribute which identifies start and end PI markers when they overlap.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.MID_ATTRIBUTE)

### EMPTY_MARKER_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EMPTY_MARKER_ATTRIBUTE

The name of the attribute that specifies that a marker is not over any content...
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.EMPTY_MARKER_ATTRIBUTE)

### TYPE_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_ATTRIBUTE

The name of the attribute holding the type of the change.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.TYPE_ATTRIBUTE)

### ATTR_NAME_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ATTR_NAME_ATTRIBUTE

The name of the attribute holding the name of the changed attribute.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlightConstants.ATTR_NAME_ATTRIBUTE)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
