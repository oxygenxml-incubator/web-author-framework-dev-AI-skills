Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class CriterionInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.sort.CriterionInformation
   @API(type=INTERNAL, src=PUBLIC) public class CriterionInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds information about a single sorting criterion.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [CriterionInformation.ORDER](CriterionInformation.ORDER.md)
Order enumeration.
  static enum  [CriterionInformation.TYPE](CriterionInformation.TYPE.md)
Type enumeration.

## Constructor Summary
 Constructors
Constructor

Description
 [CriterionInformation](#%3Cinit%3E(int,java.lang.String))(int keyIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayName)
Constructor.
  [CriterionInformation](#%3Cinit%3E(int,java.lang.String,java.lang.String,java.lang.String))(int keyIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) order, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayName)
Constructor.
  [CriterionInformation](#%3Cinit%3E(int,java.lang.String,java.lang.String,java.lang.String,boolean))(int keyIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) order, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayName, boolean isInitiallyEnabled)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName())()

 int [getKeyIndex](#getKeyIndex())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOrder](#getOrder())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getType](#getType())()

 boolean [isInitiallySelected](#isInitiallySelected())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CriterionInformation

public CriterionInformation(int keyIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) order, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayName)

Constructor.
  Parameters: keyIndex - The index in its parent of the element that corresponds to the sorting key. type - The sorting type. One of [CriterionInformation.TYPE.TEXT](CriterionInformation.TYPE.md#TEXT), [CriterionInformation.TYPE.NUMERIC](CriterionInformation.TYPE.md#NUMERIC) or [CriterionInformation.TYPE.DATE](CriterionInformation.TYPE.md#DATE). order - The sorting order. One of [CriterionInformation.ORDER.ASCENDING](CriterionInformation.ORDER.md#ASCENDING) or [CriterionInformation.ORDER.DESCENDING](CriterionInformation.ORDER.md#DESCENDING). displayName - The key display name. For a table column it can be the text from the corresponding table header cell.
### CriterionInformation

public CriterionInformation(int keyIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) type, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) order, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayName, boolean isInitiallyEnabled)

Constructor.
  Parameters: keyIndex - The index in its parent of the element that corresponds to the sorting key. type - The sorting type. One of [CriterionInformation.TYPE.TEXT](CriterionInformation.TYPE.md#TEXT), [CriterionInformation.TYPE.NUMERIC](CriterionInformation.TYPE.md#NUMERIC) or [CriterionInformation.TYPE.DATE](CriterionInformation.TYPE.md#DATE). order - The sorting order. One of [CriterionInformation.ORDER.ASCENDING](CriterionInformation.ORDER.md#ASCENDING) or [CriterionInformation.ORDER.DESCENDING](CriterionInformation.ORDER.md#DESCENDING). displayName - The key display name. For a table column it can be the text from the corresponding table header cell. isInitiallyEnabled - true if this criterion should be initially enabled.
### CriterionInformation

public CriterionInformation(int keyIndex, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayName)

Constructor.
  Parameters: keyIndex - The index in its parent of the element that corresponds to the sorting key. displayName - The key display name. For a table column it can be the text from the corresponding table header cell.
## Method Details

### getDisplayName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName()
  Returns: Returns the display name of the criterion key.
### getKeyIndex

public int getKeyIndex()
  Returns: Returns the key index for the sorting criterion. This represents the index in its parent of the element associated with the key. For a table this represents the index of the cell in its parent row.
### getType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getType()
  Returns: Returns the sorting type. One of [CriterionInformation.TYPE.TEXT](CriterionInformation.TYPE.md#TEXT), [CriterionInformation.TYPE.NUMERIC](CriterionInformation.TYPE.md#NUMERIC) or [CriterionInformation.TYPE.DATE](CriterionInformation.TYPE.md#DATE)
### getOrder

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOrder()
  Returns: Returns the sorting order. One of [CriterionInformation.ORDER.ASCENDING](CriterionInformation.ORDER.md#ASCENDING) or [CriterionInformation.ORDER.DESCENDING](CriterionInformation.ORDER.md#DESCENDING).
### isInitiallySelected

public boolean isInitiallySelected()
  Returns: true if the criterion is initially enabled.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
