Package [ro.sync.ecss.dita](package-summary.md)

# Enum Class DITAAccess.PasteInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[DITAAccess.PasteInfo](DITAAccess.PasteInfo.md)>
        * ro.sync.ecss.dita.DITAAccess.PasteInfo
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<[DITAAccess.PasteInfo](DITAAccess.PasteInfo.md)>, [Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html)   Enclosing class: [DITAAccess](DITAAccess.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public static enum DITAAccess.PasteInfo extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[DITAAccess.PasteInfo](DITAAccess.PasteInfo.md)>
Paste type of clipboard fragments.

## Nested Class Summary

## Nested classes/interfaces inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [Enum.EnumDesc](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html) extends [Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<[E](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.EnumDesc.html)>>
## Enum Constant Summary
 Enum Constants
Enum Constant

Description
 [PASTE_AS_CONKEYREF](#PASTE_AS_CONKEYREF)
Paste clipboard fragments as content key reference.
  [PASTE_AS_CONREF](#PASTE_AS_CONREF)
Paste clipboard fragments as content reference.
  [PASTE_AS_KEYREF](#PASTE_AS_KEYREF)
Paste clipboard fragments as key reference.
  [PASTE_AS_REFERENCE](#PASTE_AS_REFERENCE)
Paste clipboard fragments as reference.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) [valueOf](#valueOf(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the enum constant of this class with the specified name.
  static [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md)[] [values](#values())()
Returns an array containing the constants of this enum class, in the order they are declared.

### Methods inherited from class java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#clone()), [compareTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#compareTo(E)), [describeConstable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#describeConstable()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#finalize()), [getDeclaringClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#getDeclaringClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#hashCode()), [name](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#name()), [ordinal](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#ordinal()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#toString()), [valueOf](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html#valueOf(java.lang.Class,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Enum Constant Details

### PASTE_AS_CONKEYREF

public static final [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) PASTE_AS_CONKEYREF

Paste clipboard fragments as content key reference.

### PASTE_AS_KEYREF

public static final [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) PASTE_AS_KEYREF

Paste clipboard fragments as key reference.

### PASTE_AS_CONREF

public static final [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) PASTE_AS_CONREF

Paste clipboard fragments as content reference.

### PASTE_AS_REFERENCE

public static final [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) PASTE_AS_REFERENCE

Paste clipboard fragments as reference.

## Method Details

### values

public static [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md)[] values()

Returns an array containing the constants of this enum class, in the order they are declared.
  Returns: an array containing the constants of this enum class, in the order they are declared
### valueOf

public static [DITAAccess.PasteInfo](DITAAccess.PasteInfo.md) valueOf([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the enum constant of this class with the specified name. The string must match *exactly* an identifier used to declare an enum constant in this class. (Extraneous whitespace characters are not permitted.)
  Parameters: name - the name of the enum constant to be returned. Returns: the enum constant with the specified name Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - if this enum class has no constant with the specified name [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
