Package [ro.sync.exml.workspace.api.editor.page.author.tooltip](package-summary.md)

# Class AuthorTooltipCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.author.tooltip.AuthorTooltipCustomizer
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorTooltipCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Customize the tooltips which appear when hovering in the Author page.
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorTooltipCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract void [customizeTooltip](#customizeTooltip(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.exml.workspace.api.editor.page.author.tooltip.TooltipInformation))([AuthorAccess](../../../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess, [TooltipInformation](TooltipInformation.md) tooltipInformation)
Customize a tooltip description which will be shown when hovering in the Author editing mode.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorTooltipCustomizer

public AuthorTooltipCustomizer()

## Method Details

### customizeTooltip

public abstract void customizeTooltip([AuthorAccess](../../../../../../../ecss/extensions/api/AuthorAccess.md) authorAccess, [TooltipInformation](TooltipInformation.md) tooltipInformation)

Customize a tooltip description which will be shown when hovering in the Author editing mode.
  Parameters: authorAccess - Access to the author API. tooltipInformation - Information about the tooltip which will be displayed. This can also be used to force set a custom tooltip.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
