Package [ro.sync.exml.plugin](package-summary.md)

# Class OptionsPageGroupPluginExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.OptionsPageGroupPluginExtension
   All Implemented Interfaces: [PluginExtension](PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public class OptionsPageGroupPluginExtension extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PluginExtension](PluginExtension.md)
Plugin extension for option pages group.

## Constructor Summary
 Constructors
Constructor

Description
 [OptionsPageGroupPluginExtension](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addOptionPagePluginExtension](#addOptionPagePluginExtension(ro.sync.exml.plugin.option.OptionPagePluginExtension))([OptionPagePluginExtension](option/OptionPagePluginExtension.md) optionPageExtension)
Add a new option page plugin extension in group.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[OptionPagePluginExtension](option/OptionPagePluginExtension.md)> [getOptionPageExtensions](#getOptionPageExtensions())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OptionsPageGroupPluginExtension

public OptionsPageGroupPluginExtension()

## Method Details

### addOptionPagePluginExtension

public void addOptionPagePluginExtension([OptionPagePluginExtension](option/OptionPagePluginExtension.md) optionPageExtension)

Add a new option page plugin extension in group.
  Parameters: optionPageExtension - The option page plugin extension to be added in the group.
### getOptionPageExtensions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[OptionPagePluginExtension](option/OptionPagePluginExtension.md)> getOptionPageExtensions()
  Returns: Returns The list of all option page plugin extensions.Never null, an empty list if no pages are available.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
