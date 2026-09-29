Package [ro.sync.exml.plugin.transform](package-summary.md)

# Interface SaxonXQueryTransformerPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md), [XQueryTransformerPluginExtension](XQueryTransformerPluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface SaxonXQueryTransformerPluginExtensionextends [XQueryTransformerPluginExtension](XQueryTransformerPluginExtension.md)
A plugin extension that contributes a Saxon XQuery transformer.
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [SaxonEdition](SaxonEdition.md) [getEdition](#getEdition())()
Default value is [SaxonEdition.HE](SaxonEdition.md#HE)
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [getXQueryTransformer](#getXQueryTransformer(javax.xml.transform.Source,ro.sync.exml.editor.xmleditor.transform.advanced.XQuerySaxonHEAdvancedOptions,javax.xml.transform.URIResolver,boolean))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) source, ro.sync.exml.editor.xmleditor.transform.advanced.XQuerySaxonHEAdvancedOptions advOptions, [URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver, boolean validationOnly)
Get an XQuery transformer.

### Methods inherited from interface ro.sync.exml.plugin.transform.[XQueryTransformerPluginExtension](XQueryTransformerPluginExtension.md)
 [getDisplayTransformerName](XQueryTransformerPluginExtension.md#getDisplayTransformerName()), [getTransformerName](XQueryTransformerPluginExtension.md#getTransformerName()), [getXQueryTransformer](XQueryTransformerPluginExtension.md#getXQueryTransformer(javax.xml.transform.Source,javax.xml.transform.URIResolver,boolean)), [suportsAutomaticValidation](XQueryTransformerPluginExtension.md#suportsAutomaticValidation())
## Method Details

### getXQueryTransformer

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) getXQueryTransformer([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) source, ro.sync.exml.editor.xmleditor.transform.advanced.XQuerySaxonHEAdvancedOptions advOptions, [URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver, boolean validationOnly)throws ro.sync.exml.editor.xmleditor.ErrorListException

Get an XQuery transformer.
  Parameters: source - The XQuery source. advOptions - Advanced options. Can be XQuerySaxonHEAdvancedOptions, XQuerySaxonPEAdvancedOptionsor XQuerySaxonEEAdvancedOptions. uriResolver - The URI resolver. validationOnly - true if the transformer is used only to compile the query, to see if there are any errors. Returns: The transformer if created. Throws: ro.sync.exml.editor.xmleditor.ErrorListException
### getEdition

[SaxonEdition](SaxonEdition.md) getEdition()

Default value is [SaxonEdition.HE](SaxonEdition.md#HE)
  Returns: The Saxon edition.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
