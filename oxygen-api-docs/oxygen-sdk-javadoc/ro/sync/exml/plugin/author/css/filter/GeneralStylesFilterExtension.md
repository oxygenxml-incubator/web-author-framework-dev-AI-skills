Package [ro.sync.exml.plugin.author.css.filter](package-summary.md)

# Class GeneralStylesFilterExtension

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.author.css.filter.GeneralStylesFilterExtension
   All Implemented Interfaces: [Extension](../../../../../ecss/extensions/api/Extension.md), [StylesFilter](../../../../../ecss/extensions/api/StylesFilter.md), [PluginExtension](../../../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class GeneralStylesFilterExtension extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [PluginExtension](../../../PluginExtension.md), [StylesFilter](../../../../../ecss/extensions/api/StylesFilter.md)
CSS properties filter plugin extension. This extension will be used whether or not a document type association exists.
  Since: 14.2
## Constructor Summary
 Constructors
Constructor

Description
 [GeneralStylesFilterExtension](#%3Cinit%3E())()

## Method Summary

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../../../ecss/extensions/api/Extension.md)
 [getDescription](../../../../../ecss/extensions/api/Extension.md#getDescription())
### Methods inherited from interface ro.sync.ecss.extensions.api.[StylesFilter](../../../../../ecss/extensions/api/StylesFilter.md)
 [filter](../../../../../ecss/extensions/api/StylesFilter.md#filter(ro.sync.ecss.css.Styles,ro.sync.ecss.extensions.api.node.AuthorNode))
## Constructor Details

### GeneralStylesFilterExtension

public GeneralStylesFilterExtension()

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
