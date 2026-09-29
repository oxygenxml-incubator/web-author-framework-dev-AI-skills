Package [ro.sync.exml.plugin.transform](package-summary.md)

# Interface XQueryTransformerPluginExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   All Known Subinterfaces: [SaxonXQueryTransformerPluginExtension](SaxonXQueryTransformerPluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface XQueryTransformerPluginExtensionextends [PluginExtension](../PluginExtension.md)
A plugin extension that contributes an XQuery transformer.
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
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [getXQueryTransformer](#getXQueryTransformer(javax.xml.transform.Source,javax.xml.transform.URIResolver,boolean))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) source, [URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver, boolean validationOnly)
Get an XQuery transformer.
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
### getXQueryTransformer

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) getXQueryTransformer([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) source, [URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver, boolean validationOnly)throws ro.sync.exml.editor.xmleditor.ErrorListException

Get an XQuery transformer.
  Parameters: source - The XQuery source. uriResolver - The URI resolver. validationOnly - true if the transformer is used only to compile the query, to see if there are any errors. Returns: The transformer if created. Throws: ro.sync.exml.editor.xmleditor.ErrorListException - Exceptions encountered while initializing the transformer.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
