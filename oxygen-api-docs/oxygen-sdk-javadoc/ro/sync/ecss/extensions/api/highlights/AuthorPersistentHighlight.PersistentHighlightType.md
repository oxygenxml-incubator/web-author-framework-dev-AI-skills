Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Enum Class AuthorPersistentHighlight.PersistentHighlightType

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md)>
        * ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight.PersistentHighlightType
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   Enclosing interface: [AuthorPersistentHighlight](AuthorPersistentHighlight.md)   public static enum AuthorPersistentHighlight.PersistentHighlightType extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md)>
The Author Persistent Highlight type.   [CUSTOM_HIGHLIGHT](#CUSTOM_HIGHLIGHT) represents the Custom defined highlights that can be managed by using the [AuthorPersistentHighlighter](AuthorPersistentHighlighter.md). The name of the processing instruction markers corresponding to this type of highlight are oxy_custom_start and oxy_custom_end  [COMMENT](#COMMENT) represents the Comment highlightswhich get serialized using the oxy_comment_start and oxy_comment_end processing instruction names.  [CHANGE_INSERT](#CHANGE_INSERT) represents the Insert highlight from Change Tracking, with the oxy_insert_startand oxy_insert_end corresponding processing instruction names.  [CHANGE_DELETE](#CHANGE_DELETE) represents the Delete highlight from Change Tracking, which get serialized by using the oxy_delete processing instruction name.

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [CHANGE_ATTRIBUTE_DELETED](#CHANGE_ATTRIBUTE_DELETED)
Attribute change delete.
  [CHANGE_ATTRIBUTE_INSERTED](#CHANGE_ATTRIBUTE_INSERTED)
Attribute change insert.
  [CHANGE_ATTRIBUTE_MODIFIED](#CHANGE_ATTRIBUTE_MODIFIED)
Attribute change modified.
  [CHANGE_DELETE](#CHANGE_DELETE)
Delete change highlight
  [CHANGE_INSERT](#CHANGE_INSERT)
Insert change highlight
  [COMMENT](#COMMENT)
Comment persistent highlight
  [CUSTOM_HIGHLIGHT](#CUSTOM_HIGHLIGHT)
Custom persistent highlight

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### COMMENT

public static final [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) COMMENT

Comment persistent highlight

### CUSTOM_HIGHLIGHT

public static final [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) CUSTOM_HIGHLIGHT

Custom persistent highlight

### CHANGE_INSERT

public static final [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) CHANGE_INSERT

Insert change highlight

### CHANGE_DELETE

public static final [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) CHANGE_DELETE

Delete change highlight

### CHANGE_ATTRIBUTE_INSERTED

public static final [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) CHANGE_ATTRIBUTE_INSERTED

Attribute change insert.

### CHANGE_ATTRIBUTE_MODIFIED

public static final [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) CHANGE_ATTRIBUTE_MODIFIED

Attribute change modified.

### CHANGE_ATTRIBUTE_DELETED

public static final [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) CHANGE_ATTRIBUTE_DELETED

Attribute change delete.

## Method Details

### values

public static [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [AuthorPersistentHighlight.PersistentHighlightType](AuthorPersistentHighlight.PersistentHighlightType.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
