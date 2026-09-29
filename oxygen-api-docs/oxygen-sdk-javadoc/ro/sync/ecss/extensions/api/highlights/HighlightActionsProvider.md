Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Class HighlightActionsProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.highlights.HighlightActionsProvider
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class HighlightActionsProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provider for the actions available for a highlight.
  Since: 17.1
## Constructor Summary
 Constructors
Constructor

Description
 [HighlightActionsProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) [getActions](#getActions(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../AuthorAccess.md) authorAccess)
Get the available actions for a highlight.
  abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getCollapsedWidgetIcon](#getCollapsedWidgetIcon())()
Get the icon for the collapsed widget.
  abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getExpandedWidgetIcon](#getExpandedWidgetIcon())()
Get the icon for the expanded widget.
  [HighlightActionsRenderingStyle](HighlightActionsRenderingStyle.md) [getRenderingStyle](#getRenderingStyle())()
Get the rendering style of the actions.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getWidgetTooltipMessage](#getWidgetTooltipMessage())()
Get the tolltip message displayed when hovering over the widget.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### HighlightActionsProvider

public HighlightActionsProvider()

## Method Details

### getActions

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) getActions([AuthorAccess](../AuthorAccess.md) authorAccess)

Get the available actions for a highlight.
  Parameters: authorAccess - The author access. Returns: the list of actions.
### getCollapsedWidgetIcon

public abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getCollapsedWidgetIcon()

Get the icon for the collapsed widget. The collapsed widget is shown when hovering over a highlight.
  Returns: the icon for the collapsed widget.
### getExpandedWidgetIcon

public abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getExpandedWidgetIcon()

Get the icon for the expanded widget. The expanded widget is shown when hovering over the collapsed widget. The collapsed widget is shown when hovering over a highlight.
  Returns: the icon for the expanded widget.
### getRenderingStyle

public [HighlightActionsRenderingStyle](HighlightActionsRenderingStyle.md) getRenderingStyle()

Get the rendering style of the actions.
  Returns: the rendering style of the actions.
### getWidgetTooltipMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getWidgetTooltipMessage()

Get the tolltip message displayed when hovering over the widget.
  Returns: The tooltip message displayed on the widget.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
