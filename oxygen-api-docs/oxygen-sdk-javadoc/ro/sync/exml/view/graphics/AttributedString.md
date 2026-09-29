Package [ro.sync.exml.view.graphics](package-summary.md)

# Class AttributedString

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.view.graphics.AttributedString
   @API(type=EXTENDABLE, src=PRIVATE) public class AttributedString extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A string annotated with attributes. For instance an interval can have a red foreground, other one a specific font, etc.. Similar to [AttributedString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/text/AttributedString.html).

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static class  [AttributedString.AttributedInterval](AttributedString.AttributedInterval.md)
A text interval from the string, with a specific attribute.

## Constructor Summary
 Constructors
Constructor

Description
 [AttributedString](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) string)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addAttribute](#addAttribute(ro.sync.exml.view.graphics.TextAttribute,java.lang.Object))([TextAttribute](TextAttribute.md) textAttribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)
Adds an attribute on the entire string.
  void [addAttribute](#addAttribute(ro.sync.exml.view.graphics.TextAttribute,java.lang.Object,int,int))([TextAttribute](TextAttribute.md) attribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value, int beginIndex, int endIndex)
Adds an attribute to a subrange of the string.
  void [addAttributedInterval](#addAttributedInterval(ro.sync.exml.view.graphics.AttributedString.AttributedInterval))([AttributedString.AttributedInterval](AttributedString.AttributedInterval.md) interval)
Adds an attribute to a subrange of the string.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AttributedString.AttributedInterval](AttributedString.AttributedInterval.md)> [getIntervals](#getIntervals())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getString](#getString())()

 int [hashCode](#hashCode())()

 boolean [isDisableDrawSpacesAndTabs](#isDisableDrawSpacesAndTabs())()

 int [length](#length())()

 void [removeAllAttributes](#removeAllAttributes(ro.sync.exml.view.graphics.TextAttribute))([TextAttribute](TextAttribute.md) attrribute)
Remove all intervals having a value for the specified attribute key.
  void [setDisableDrawSpacesAndTabs](#setDisableDrawSpacesAndTabs(boolean))(boolean disableDrawSpacesAndTabs)
Set disable drawing spaces and tabs.
  [AttributedString](AttributedString.md)[] [toMultiLineAttributeStrings](#toMultiLineAttributeStrings())()
Convert this attributed string to an array of attributed strings, one for each line of content.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AttributedString

public AttributedString([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) string)

Constructor.
  Parameters: string - The string
## Method Details

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### addAttribute

public void addAttribute([TextAttribute](TextAttribute.md) attribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value, int beginIndex, int endIndex)

Adds an attribute to a subrange of the string.
  Parameters: attribute - the attribute key value - The value of the attribute. Should not be null. beginIndex - Index of the first character of the range. endIndex - Index of the character following the last character of the range.
### addAttributedInterval

public void addAttributedInterval([AttributedString.AttributedInterval](AttributedString.AttributedInterval.md) interval)

Adds an attribute to a subrange of the string.
  Parameters: interval - the attributed interval.
### getString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getString()
  Returns: Returns the string.
### getIntervals

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AttributedString.AttributedInterval](AttributedString.AttributedInterval.md)> getIntervals()
  Returns: Returns the intervals.
### length

public int length()
  Returns: The length of the inner string.
### addAttribute

public void addAttribute([TextAttribute](TextAttribute.md) textAttribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

Adds an attribute on the entire string.
  Parameters: textAttribute - The text attribute. value - The value of the attribute.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### removeAllAttributes

public void removeAllAttributes([TextAttribute](TextAttribute.md) attrribute)

Remove all intervals having a value for the specified attribute key.
  Parameters: attrribute - The attribute key.
### toMultiLineAttributeStrings

public [AttributedString](AttributedString.md)[] toMultiLineAttributeStrings()

Convert this attributed string to an array of attributed strings, one for each line of content.
  Returns: an array of attributed strings, one for each line of content.
### isDisableDrawSpacesAndTabs

public boolean isDisableDrawSpacesAndTabs()
  Returns: true if drawing spaces and tabs is disabled.
### setDisableDrawSpacesAndTabs

public void setDisableDrawSpacesAndTabs(boolean disableDrawSpacesAndTabs)

Set disable drawing spaces and tabs.
  Parameters: disableDrawSpacesAndTabs - true if drawing spaces and tabs is disabled.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
