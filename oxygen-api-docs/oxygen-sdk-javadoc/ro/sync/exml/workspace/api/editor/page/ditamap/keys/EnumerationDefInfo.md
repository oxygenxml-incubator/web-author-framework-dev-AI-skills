Package [ro.sync.exml.workspace.api.editor.page.ditamap.keys](package-summary.md)

# Class EnumerationDefInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.ditamap.keys.EnumerationDefInfo
   @API(type=EXTENDABLE, src=PUBLIC) public class EnumerationDefInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
An enumeration def info. <enumerationdef> <elementdef name="p"/> <attributedef name="product"/> <subjectdef keyref="test"/> </enumerationdef>

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MULTI_VALUE_OUTPUTCLASS_TOKEN](#MULTI_VALUE_OUTPUTCLASS_TOKEN)
If this token is found in the outputclass attribute, then the enumerationdef only allows multiple values.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SINGLE_VALUE_OUTPUTCLASS_TOKEN](#SINGLE_VALUE_OUTPUTCLASS_TOKEN)
If this token is found in the outputclass attribute, then the enumerationdef only allows single values.

## Constructor Summary
 Constructors
Constructor

Description
 [EnumerationDefInfo](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementName)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addReferencedKey](#addReferencedKey(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef)
Add a referenced key.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeName](#getAttributeName())()
Get the attribute name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getElementName](#getElementName())()
Get the element name.
  [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> [getKeyScopes](#getKeyScopes())()

 [LinkedHashSet](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashSet.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getReferencedKeys](#getReferencedKeys())()
Get the set of referenced keys, can be null.
  int [hashCode](#hashCode())()

 [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) [isSingleValue](#isSingleValue())()

 void [setKeyScopes](#setKeyScopes(java.util.Stack))([Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> keyScopes)

 void [setSingleValue](#setSingleValue(java.lang.Boolean))([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) singleValue)
Set single value.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### SINGLE_VALUE_OUTPUTCLASS_TOKEN

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SINGLE_VALUE_OUTPUTCLASS_TOKEN

If this token is found in the outputclass attribute, then the enumerationdef only allows single values.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.EnumerationDefInfo.SINGLE_VALUE_OUTPUTCLASS_TOKEN)

### MULTI_VALUE_OUTPUTCLASS_TOKEN

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MULTI_VALUE_OUTPUTCLASS_TOKEN

If this token is found in the outputclass attribute, then the enumerationdef only allows multiple values.
  See Also:
        * [Constant Field Values](../../../../../../../../../constant-values.md#ro.sync.exml.workspace.api.editor.page.ditamap.keys.EnumerationDefInfo.MULTI_VALUE_OUTPUTCLASS_TOKEN)

## Constructor Details

### EnumerationDefInfo

public EnumerationDefInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementName)

Constructor.
  Parameters: attributeName - The attribute name. elementName - The element name. Can be null.
## Method Details

### getAttributeName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeName()

Get the attribute name.
  Returns: Returns the attribute name.
### getElementName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getElementName()

Get the element name.
  Returns: Returns the element name.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### getReferencedKeys

public [LinkedHashSet](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashSet.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getReferencedKeys()

Get the set of referenced keys, can be null.
  Returns: Returns the referenced key names.
### addReferencedKey

public void addReferencedKey([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyRef)

Add a referenced key.
  Parameters: keyRef - The keyref.
### setKeyScopes

public void setKeyScopes([Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> keyScopes)
  Parameters: keyScopes - The keyScopes to set.
### getKeyScopes

public [Stack](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Stack.html)<[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> getKeyScopes()
  Returns: Returns the keyScopes.
### isSingleValue

public [Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) isSingleValue()
  Returns: Returns null if we do not have this information, true if should allow single value, false if it should allow multiple values.
### setSingleValue

public void setSingleValue([Boolean](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Boolean.html) singleValue)

Set single value.
  Parameters: singleValue - null if we do not have this information, true if should allow single value, false if it should allow multiple values.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
