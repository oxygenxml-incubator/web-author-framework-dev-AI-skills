Package [ro.sync.exml.workspace.api.editor.page.ditamap](package-summary.md)

# Class DITAMapNodeRendererCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.node.customizer.XMLNodeRendererCustomizer](../../../node/customizer/XMLNodeRendererCustomizer.md)
        * ro.sync.exml.workspace.api.editor.page.ditamap.DITAMapNodeRendererCustomizer
   All Implemented Interfaces: [Extension](../../../../../../ecss/extensions/api/Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class DITAMapNodeRendererCustomizer extends [XMLNodeRendererCustomizer](../../../node/customizer/XMLNodeRendererCustomizer.md)
Node renderer customizer specific for the DITA Maps Manager.
  Since: 18.1
## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapNodeRendererCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [customizeComputedTopicrefTitle](#customizeComputedTopicrefTitle(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) topicref, [AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) targetTopicOrMap, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultComputedTitle)
Customize the default computed topicref title.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [customizeRenderedTopicrefTitle](#customizeRenderedTopicrefTitle(ro.sync.ecss.extensions.api.node.AuthorNode,java.lang.String))([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) topicref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultRenderedTitle)
Customize the default rendered topicref title.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [BasicRenderingInformation](../../../node/customizer/BasicRenderingInformation.md) [getRenderingInformation](#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext))([NodeRendererCustomizerContext](../../../node/customizer/NodeRendererCustomizerContext.md) context)
Override this to provide extra rendering information.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAMapNodeRendererCustomizer

public DITAMapNodeRendererCustomizer()

## Method Details

### customizeComputedTopicrefTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) customizeComputedTopicrefTitle([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) topicref, [AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) targetTopicOrMap, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultComputedTitle)

Customize the default computed topicref title. After the API returns the modified title, the title will be cached for the current referenced topic. So this method is called usually once for every individual referenced topic. This kind of method is useful for example if you want to get some significant attributes (maybe profiling attributes) from the topic's root element and display them in the title.
  Parameters: topicref - The topicref node present in the DITA Maps Manager targetTopicOrMap - Oxygen already parsed the document referenced via topicref, computed a title and this parameter gives you access to the root element of the parsed topic. defaultComputedTitle - The default title computed by Oxygen Returns: The customized topic title.
### customizeRenderedTopicrefTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) customizeRenderedTopicrefTitle([AuthorNode](../../../../../../ecss/extensions/api/node/AuthorNode.md) topicref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultRenderedTitle)

Customize the default rendered topicref title. This method is called very often, each time the tree or part of the tree is rendered. It is also called separately if there are multiple topicrefs pointing to the same topic. This kind of method is useful for example if you want to number topicrefs displayed in the DITA Maps Manager view based on depth.
  Parameters: topicref - The topicref node present in the DITA Maps Manager defaultRenderedTitle - The default title which will be rendered by Oxygen Returns: The customized topic title. Since: 21
### getRenderingInformation

public [BasicRenderingInformation](../../../node/customizer/BasicRenderingInformation.md) getRenderingInformation([NodeRendererCustomizerContext](../../../node/customizer/NodeRendererCustomizerContext.md) context)

Override this to provide extra rendering information. The context is an instance of [DITAMapNodeRendererCustomizerContext](DITAMapNodeRendererCustomizerContext.md) which has more information about topicrefs.
  Specified by: [getRenderingInformation](../../../node/customizer/XMLNodeRendererCustomizer.md#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext)) in class [XMLNodeRendererCustomizer](../../../node/customizer/XMLNodeRendererCustomizer.md) Parameters: context - The node context(contains information like node name, namespace and attributes). Returns: The rendering information. If the returned value is null then the default node rendering will be used. See Also:
        * [XMLNodeRendererCustomizer.getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext)](../../../node/customizer/XMLNodeRendererCustomizer.md#getRenderingInformation(ro.sync.exml.workspace.api.node.customizer.NodeRendererCustomizerContext))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../../../../ecss/extensions/api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
