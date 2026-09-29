Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorConstants
    All Known Subinterfaces: [AuthorAccess](AuthorAccess.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorConstants
Interface containing the constants used in Author API.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARG_VALUE_FALSE](#ARG_VALUE_FALSE)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARG_VALUE_TRUE](#ARG_VALUE_TRUE)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MOVE_DOWN](#MOVE_DOWN)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MOVE_UP](#MOVE_UP)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_AFTER](#POSITION_AFTER)
The insertion location is after the selected node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_BEFORE](#POSITION_BEFORE)
The insertion location is before the selected node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_INSIDE](#POSITION_INSIDE)  Deprecated.
Use the constant POSITION_INSIDE_FIRST instead.
   static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_INSIDE_AT_THE_BEGINNING](#POSITION_INSIDE_AT_THE_BEGINNING)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_INSIDE_AT_THE_END](#POSITION_INSIDE_AT_THE_END)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_INSIDE_FIRST](#POSITION_INSIDE_FIRST)
The insertion location is inside the selected node as the first child.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [POSITION_INSIDE_LAST](#POSITION_INSIDE_LAST)
The insertion location is inside the selected node as the last child.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SELECT_CONTENT](#SELECT_CONTENT)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SELECT_ELEMENT](#SELECT_ELEMENT)
Constant used for operation argument value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SELECT_NONE](#SELECT_NONE)
Constant used for operation argument value.

## Field Details

### POSITION_BEFORE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_BEFORE

The insertion location is before the selected node.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.POSITION_BEFORE)

### POSITION_AFTER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_AFTER

The insertion location is after the selected node.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.POSITION_AFTER)

### POSITION_INSIDE

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_INSIDE
 Deprecated.
Use the constant POSITION_INSIDE_FIRST instead.

The insertion location is inside the selected node as the first child.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.POSITION_INSIDE)

### POSITION_INSIDE_FIRST

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_INSIDE_FIRST

The insertion location is inside the selected node as the first child.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.POSITION_INSIDE_FIRST)

### POSITION_INSIDE_LAST

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_INSIDE_LAST

The insertion location is inside the selected node as the last child.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.POSITION_INSIDE_LAST)

### ARG_VALUE_TRUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARG_VALUE_TRUE

Constant used for operation argument value.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.ARG_VALUE_TRUE)

### ARG_VALUE_FALSE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARG_VALUE_FALSE

Constant used for operation argument value.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.ARG_VALUE_FALSE)

### SELECT_NONE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SELECT_NONE

Constant used for operation argument value. It means that no selection should be performed.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.SELECT_NONE)

### SELECT_ELEMENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SELECT_ELEMENT

Constant used for operation argument value. It means that the current element should be selected.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.SELECT_ELEMENT)

### SELECT_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SELECT_CONTENT

Constant used for operation argument value. It means that the content of the current element should be selected.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.SELECT_CONTENT)

### POSITION_INSIDE_AT_THE_BEGINNING

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_INSIDE_AT_THE_BEGINNING

Constant used for operation argument value. It means that the caret should be positioned inside the element, right after the start tag.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.POSITION_INSIDE_AT_THE_BEGINNING)

### POSITION_INSIDE_AT_THE_END

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) POSITION_INSIDE_AT_THE_END

Constant used for operation argument value. It means that the caret should be positioned inside the element, right before the end tag.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.POSITION_INSIDE_AT_THE_END)

### MOVE_UP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MOVE_UP

Constant used for operation argument value. It means that the block at caret or blocks selected will move up.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.MOVE_UP)

### MOVE_DOWN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MOVE_DOWN

Constant used for operation argument value. It means that the block at caret or blocks selected will move down.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorConstants.MOVE_DOWN)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
