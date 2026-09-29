Package [ro.sync.exml.workspace.api.node.customizer](package-summary.md)

# Class XMLNodeRendererCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.node.customizer.XMLNodeRendererCustomizer
   All Implemented Interfaces: [Extension](../../../../../ecss/extensions/api/Extension.md)   Direct Known Subclasses: [AntNodeRendererCustomizer](../../../../../ecss/extensions/ant/AntNodeRendererCustomizer.md), [DITAMapNodeRendererCustomizer](../../editor/page/ditamap/DITAMapNodeRendererCustomizer.md), [DITANodeRendererCustomizer](../../../../../ecss/extensions/dita/DITANodeRendererCustomizer.md), [DocbookNodeRendererCustomizer](../../../../../ecss/extensions/docbook/DocbookNodeRendererCustomizer.md), [JSONNodeRendererCustomizer](../../../../../ecss/extensions/json/JSONNodeRendererCustomizer.md), [SchematronNodeRendererCustomizer](../../../../../ecss/extensions/schematron/SchematronNodeRendererCustomizer.md), [TEINodeRendererCustomizer](../../../../../ecss/extensions/tei/TEINodeRendererCustomizer.md), [WSDLNodeRendererCustomizer](../../../../../ecss/extensions/wsdl/WSDLNodeRendererCustomizer.md), [XHTMLNodeRendererCustomizer](../../../../../ecss/extensions/xhtml/XHTMLNodeRendererCustomizer.md), [XMLNodeRendererCustomizerAdapter](../../../../../ecss/extensions/commons/XMLNodeRendererCustomizerAdapter.md), [XSDNodeRendererCustomizer](../../../../../ecss/extensions/xsd/XSDNodeRendererCustomizer.md), [XSLTNodeRendererCustomizer](../../../../../ecss/extensions/xslt/XSLTNodeRendererCustomizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class XMLNodeRendererCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Extension](../../../../../ecss/extensions/api/Extension.md)
Class used to customize the way an XML node is rendered in the UI. A node represents an entry from Author outline, Author bread crumb, Text page outline, content completion proposals window or DITA Map view.
  Since: 13.2
## Constructor Summary
 Constructors
Constructor

Description
 [XMLNodeRendererCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [BasicRenderingInformation](BasicRenderingInformation.md) [getRenderingInformation](#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext))([NodeRendererCustomizerContext](NodeRendererCustomizerContext.md) context)
Get the rendering information (text to render, path of the icon to display in outline, bread crumb or content completion proposals window) for given context.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../../../ecss/extensions/api/Extension.md)
 [getDescription](../../../../../ecss/extensions/api/Extension.md#getDescription())
## Constructor Details

### XMLNodeRendererCustomizer

public XMLNodeRendererCustomizer()

## Method Details

### getRenderingInformation

public abstract [BasicRenderingInformation](BasicRenderingInformation.md) getRenderingInformation([NodeRendererCustomizerContext](NodeRendererCustomizerContext.md) context)

Get the rendering information (text to render, path of the icon to display in outline, bread crumb or content completion proposals window) for given context.
  Parameters: context - The node context(contains information like node name, namespace and attributes). Returns: The rendering information. If the returned value is null then the default node rendering will be used.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
