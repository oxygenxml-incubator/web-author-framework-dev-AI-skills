Package [ro.sync.exml.plugin.transform](package-summary.md)

# Interface XSLTTransformerPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   All Known Subinterfaces: [SaxonXSLTTransformerPluginExtension](SaxonXSLTTransformerPluginExtension.md)   All Known Implementing Classes: [XSLTTransformerPluginExtensionBase](XSLTTransformerPluginExtensionBase.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface XSLTTransformerPluginExtensionextends [PluginExtension](../PluginExtension.md)
A plugin extension that contributes an XSLT transformer.
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayTransformerName](#getDisplayTransformerName())()
Get the display transformer name.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTransformerName](#getTransformerName())()
Get the transformer name.
  [TransformerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerFactory.html) [getXSLTTransformerFactory](#getXSLTTransformerFactory(ro.sync.exml.plugin.transform.XSLMessageListener))([XSLMessageListener](XSLMessageListener.md) messageListener)
Gets the XSLT transformer factory.
  boolean [isXSLT20Transformer](#isXSLT20Transformer())()
Check if it is an XSLT 2.0 transformer.
  boolean [isXSLT30Transformer](#isXSLT30Transformer())()
Check if it is an XSLT 3.0 transformer.
  boolean [suportsAutomaticValidation](#suportsAutomaticValidation())()
Checks if this transformer supports validation.

## Method Details

### getTransformerName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTransformerName()

Get the transformer name.
  Returns: The transformer name.
### getDisplayTransformerName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayTransformerName()

Get the display transformer name.
  Returns: The display transformer name.
### suportsAutomaticValidation

boolean suportsAutomaticValidation()

Checks if this transformer supports validation.
  Returns: true if automatic validation is supported.
### getXSLTTransformerFactory

[TransformerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerFactory.html) getXSLTTransformerFactory([XSLMessageListener](XSLMessageListener.md) messageListener)

Gets the XSLT transformer factory.
  Parameters: messageListener - A listener that will receive events when an xsl:message or xsl:assert is triggered. Returns: The factory used for obtaining the transformer.
### isXSLT20Transformer

boolean isXSLT20Transformer()

Check if it is an XSLT 2.0 transformer.
  Returns: true if it is an XSLT 2.0 transformer.
### isXSLT30Transformer

boolean isXSLT30Transformer()

Check if it is an XSLT 3.0 transformer.
  Returns: true if it is an XSLT 3.0 transformer.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
