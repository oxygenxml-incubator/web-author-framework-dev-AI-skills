Package [ro.sync.exml.plugin.transform](package-summary.md)

# Class XSLTTransformerPluginExtensionBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.transform.XSLTTransformerPluginExtensionBase
   All Implemented Interfaces: [PluginExtension](../PluginExtension.md), [XSLTTransformerPluginExtension](XSLTTransformerPluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class XSLTTransformerPluginExtensionBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [XSLTTransformerPluginExtension](XSLTTransformerPluginExtension.md)
Base class for transformers.

## Constructor Summary
 Constructors
Constructor

Description
 [XSLTTransformerPluginExtensionBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [TransformerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerFactory.html) [getXSLTTransformerFactory](#getXSLTTransformerFactory(ro.sync.exml.plugin.transform.ConfigurationProperties))([ConfigurationProperties](ConfigurationProperties.md) properties)
Gets the XSLT transformer factory.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.exml.plugin.transform.[XSLTTransformerPluginExtension](XSLTTransformerPluginExtension.md)
 [getDisplayTransformerName](XSLTTransformerPluginExtension.md#getDisplayTransformerName()), [getTransformerName](XSLTTransformerPluginExtension.md#getTransformerName()), [getXSLTTransformerFactory](XSLTTransformerPluginExtension.md#getXSLTTransformerFactory(ro.sync.exml.plugin.transform.XSLMessageListener)), [isXSLT20Transformer](XSLTTransformerPluginExtension.md#isXSLT20Transformer()), [isXSLT30Transformer](XSLTTransformerPluginExtension.md#isXSLT30Transformer()), [suportsAutomaticValidation](XSLTTransformerPluginExtension.md#suportsAutomaticValidation())
## Constructor Details

### XSLTTransformerPluginExtensionBase

public XSLTTransformerPluginExtensionBase()

## Method Details

### getXSLTTransformerFactory

public [TransformerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerFactory.html) getXSLTTransformerFactory([ConfigurationProperties](ConfigurationProperties.md) properties)

Gets the XSLT transformer factory.
  Parameters: properties - Configuration properties. Returns: The factory used for obtaining the transformer. Since: 19.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
