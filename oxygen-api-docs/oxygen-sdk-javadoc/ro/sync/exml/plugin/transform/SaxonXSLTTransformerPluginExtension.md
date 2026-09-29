Package [ro.sync.exml.plugin.transform](package-summary.md)

# Interface SaxonXSLTTransformerPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md), [XSLTTransformerPluginExtension](XSLTTransformerPluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface SaxonXSLTTransformerPluginExtensionextends [XSLTTransformerPluginExtension](XSLTTransformerPluginExtension.md)
A plugin extension that contributes a Saxon XSLT transformer.
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [SaxonEdition](SaxonEdition.md) [getEdition](#getEdition())()
Default value is [SaxonEdition.HE](SaxonEdition.md#HE)

### Methods inherited from interface ro.sync.exml.plugin.transform.[XSLTTransformerPluginExtension](XSLTTransformerPluginExtension.md)
 [getDisplayTransformerName](XSLTTransformerPluginExtension.md#getDisplayTransformerName()), [getTransformerName](XSLTTransformerPluginExtension.md#getTransformerName()), [getXSLTTransformerFactory](XSLTTransformerPluginExtension.md#getXSLTTransformerFactory(ro.sync.exml.plugin.transform.XSLMessageListener)), [isXSLT20Transformer](XSLTTransformerPluginExtension.md#isXSLT20Transformer()), [isXSLT30Transformer](XSLTTransformerPluginExtension.md#isXSLT30Transformer()), [suportsAutomaticValidation](XSLTTransformerPluginExtension.md#suportsAutomaticValidation())
## Method Details

### getEdition

[SaxonEdition](SaxonEdition.md) getEdition()

Default value is [SaxonEdition.HE](SaxonEdition.md#HE)
  Returns: The Saxon edition.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
