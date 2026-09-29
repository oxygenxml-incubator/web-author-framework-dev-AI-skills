Package [ro.sync.ecss.extensions.api.structure](package-summary.md)

# Interface AuthorNodeRendererCustomizer
    All Known Implementing Classes: [AuthorBreadCrumbCustomizer](AuthorBreadCrumbCustomizer.md), [AuthorOutlineCustomizer](AuthorOutlineCustomizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorNodeRendererCustomizer
Customize rendering information for an AuthorNode
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizeRenderingInformation](#customizeRenderingInformation(ro.sync.ecss.extensions.api.structure.RenderingInformation))([RenderingInformation](RenderingInformation.md) renderInfo)
Customize the tooltip, text and additional info to be presented in the Outline and Breadcrumb for the given node.

## Method Details

### customizeRenderingInformation

void customizeRenderingInformation([RenderingInformation](RenderingInformation.md) renderInfo)

Customize the tooltip, text and additional info to be presented in the Outline and Breadcrumb for the given node. By default a node is represented in the Outline by its tag name and a additional information obtained from a specific attribute or text. You can set custom values for each rendered field. If you need to change the way the XML elements are displayed, you may consider using a configuration file. For more information, search the oXygen documentation for "cc_config.xml" configuration file. For DITA, this file is in "frameworks/dita/resources/cc_config.xml".
  Parameters: renderInfo - The default information which will get displayed. You can set custom values for each field
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
