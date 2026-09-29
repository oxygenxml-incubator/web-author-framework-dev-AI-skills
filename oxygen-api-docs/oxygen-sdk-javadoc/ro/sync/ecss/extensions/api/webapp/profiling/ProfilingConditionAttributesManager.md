Package [ro.sync.ecss.extensions.api.webapp.profiling](package-summary.md)

# Interface ProfilingConditionAttributesManager
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ProfilingConditionAttributesManager
Gives access to profiling attributes.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ProfileConditionInfoPO](../../../../conditions/ProfileConditionInfoPO.md)> [getProfilingConditionAttributes](#getProfilingConditionAttributes(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../node/AuthorElement.md) contextElement)
Get defined profiling attribute names and values which can be set for the current context element.

## Method Details

### getProfilingConditionAttributes

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ProfileConditionInfoPO](../../../../conditions/ProfileConditionInfoPO.md)> getProfilingConditionAttributes([AuthorElement](../../node/AuthorElement.md) contextElement)

Get defined profiling attribute names and values which can be set for the current context element. The profiling attribute names and values should be defined either in a subject scheme or in the corresponding options page.
  Parameters: contextElement - The XML element for which profiling attributes are required. In a subject scheme map you can map values based on the element name and attribute name. Returns: the list of defined profiling attribute names and values which can be set for the context element.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
