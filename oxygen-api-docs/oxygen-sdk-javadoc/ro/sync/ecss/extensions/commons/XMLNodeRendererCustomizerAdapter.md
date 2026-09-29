Package [ro.sync.ecss.extensions.commons](package-summary.md)

# Class XMLNodeRendererCustomizerAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.node.customizer.XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md)
        * ro.sync.ecss.extensions.commons.XMLNodeRendererCustomizerAdapter
   All Implemented Interfaces: [Extension](../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class XMLNodeRendererCustomizerAdapter extends [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md)
Empty implementation for [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md).

## Constructor Summary
 Constructors
Constructor

Description
 [XMLNodeRendererCustomizerAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [BasicRenderingInformation](../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md) [getRenderingInformation](#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext))([NodeRendererCustomizerContext](../../../exml/workspace/api/node/customizer/NodeRendererCustomizerContext.md) context)
Get the rendering information (text to render, path of the icon to display in outline, bread crumb or content completion proposals window) for given context.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XMLNodeRendererCustomizerAdapter

public XMLNodeRendererCustomizerAdapter()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../api/Extension.md#getDescription())

### getRenderingInformation

public [BasicRenderingInformation](../../../exml/workspace/api/node/customizer/BasicRenderingInformation.md) getRenderingInformation([NodeRendererCustomizerContext](../../../exml/workspace/api/node/customizer/NodeRendererCustomizerContext.md) context)
 Description copied from class: [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext))
Get the rendering information (text to render, path of the icon to display in outline, bread crumb or content completion proposals window) for given context.
  Specified by: [getRenderingInformation](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext)) in class [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) Parameters: context - The node context(contains information like node name, namespace and attributes). Returns: The rendering information. If the returned value is null then the default node rendering will be used. See Also:
        * [XMLNodeRendererCustomizer.getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext)](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
