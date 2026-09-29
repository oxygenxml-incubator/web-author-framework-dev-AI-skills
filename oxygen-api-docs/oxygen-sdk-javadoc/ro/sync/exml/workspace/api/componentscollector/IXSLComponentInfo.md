Package [ro.sync.exml.workspace.api.componentscollector](package-summary.md)

# Interface IXSLComponentInfo
    All Superinterfaces: [IComponentInfo](IComponentInfo.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface IXSLComponentInfoextends [IComponentInfo](IComponentInfo.md)
XSL Component information interface.
  Since: 27
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMatch](#getMatch())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMode](#getMode())()

### Methods inherited from interface ro.sync.exml.workspace.api.componentscollector.[IComponentInfo](IComponentInfo.md)
 [getAnnotation](IComponentInfo.md#getAnnotation()), [getEndOffset](IComponentInfo.md#getEndOffset()), [getName](IComponentInfo.md#getName()), [getStartOffset](IComponentInfo.md#getStartOffset()), [getSystemId](IComponentInfo.md#getSystemId()), [getType](IComponentInfo.md#getType())
## Method Details

### getMatch

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMatch()
  Returns: Returns the template's match.
### getMode

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMode()
  Returns: Returns the template's mode.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
