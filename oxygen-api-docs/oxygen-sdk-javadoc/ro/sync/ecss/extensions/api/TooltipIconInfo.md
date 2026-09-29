Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class TooltipIconInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.TooltipIconInfo
   @API(type=EXTENDABLE, src=PUBLIC) public class TooltipIconInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The information(tooltip and icon) used to describe the editing of the value for an attribute.
  Since: 21
## Constructor Summary
 Constructors
Constructor

Description
 [TooltipIconInfo](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) iconPath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltip)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getImagePath](#getImagePath())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltip](#getTooltip())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TooltipIconInfo

public TooltipIconInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) iconPath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tooltip)

Constructor
  Parameters: iconPath - The path (an URI) for the custom button icon. tooltip - The custom tooltip for the button.
## Method Details

### getImagePath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getImagePath()
  Returns: The path for the custom button icon.
### getTooltip

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltip()
  Returns: The custom tooltip for the button.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
