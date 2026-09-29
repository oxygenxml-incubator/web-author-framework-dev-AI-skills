Package [ro.sync.ecss.extensions.api](package-summary.md)

# Enum Class SelectionInterpretationMode

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[SelectionInterpretationMode](SelectionInterpretationMode.md)>
        * ro.sync.ecss.extensions.api.SelectionInterpretationMode
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[SelectionInterpretationMode](SelectionInterpretationMode.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public enum SelectionInterpretationMode extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[SelectionInterpretationMode](SelectionInterpretationMode.md)>
Impose how the selection is interpreted by the application.  The [TABLE_COLUMN](#TABLE_COLUMN) interpretation mode is already set by default by the application when a table column is selected. In this case, when the column is pasted, it is also interpreted as a table column by the application built-in document types. To obtain this behavior for any selection, the [TABLE_COLUMN](#TABLE_COLUMN) interpretation mode must be imposed from [AuthorSelectionModel.setSelectionInterpretationMode(SelectionInterpretationMode)](AuthorSelectionModel.md#setSelectionInterpretationMode(ro.sync.ecss.extensions.api.SelectionInterpretationMode))method. For instance, when two paragraphs are copied, the clipboard object contains a list with two Author document fragments (one for each paragraph). If the selection interpretation mode is imposed to [TABLE_COLUMN](#TABLE_COLUMN), when pasting the fragments a table column is created, each paragraph being the content of a column cell.  For a custom document type, when a content with an imposed [TABLE_COLUMN](#TABLE_COLUMN) interpretation mode is pasted the AuthorTableOperationsHandler#handlePasteColumn(AuthorTablePasteColumnArguments) method is called. If there is no implementation for this extension, the default paste behavior is invoked. See [ExtensionsBundle.getAuthorTableOperationsHandler()](ExtensionsBundle.md#getAuthorTableOperationsHandler()) for handling the paste column operation.
  Since: 14
## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [TABLE](#TABLE)
Table selection interpretation.
  [TABLE_CELLS](#TABLE_CELLS)
Table cells selection interpretation (one or more table cells are selected).
  [TABLE_COLUMN](#TABLE_COLUMN)
Table column selection interpretation.
  [TABLE_ROW](#TABLE_ROW)
Table rows selection interpretation (one or more table rows are selected).

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [SelectionInterpretationMode](SelectionInterpretationMode.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [SelectionInterpretationMode](SelectionInterpretationMode.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### TABLE_COLUMN

public static final [SelectionInterpretationMode](SelectionInterpretationMode.md) TABLE_COLUMN

Table column selection interpretation.

### TABLE_ROW

public static final [SelectionInterpretationMode](SelectionInterpretationMode.md) TABLE_ROW

Table rows selection interpretation (one or more table rows are selected).

### TABLE_CELLS

public static final [SelectionInterpretationMode](SelectionInterpretationMode.md) TABLE_CELLS

Table cells selection interpretation (one or more table cells are selected).

### TABLE

public static final [SelectionInterpretationMode](SelectionInterpretationMode.md) TABLE

Table selection interpretation.

## Method Details

### values

public static [SelectionInterpretationMode](SelectionInterpretationMode.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [SelectionInterpretationMode](SelectionInterpretationMode.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
