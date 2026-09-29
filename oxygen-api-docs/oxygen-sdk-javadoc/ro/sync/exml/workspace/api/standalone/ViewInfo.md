Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Class ViewInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.ViewInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class ViewInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Information about a view.
  Since: 11.2
## Constructor Summary
 Constructors
Constructor

Description
 [ViewInfo](#%3Cinit%3E(java.lang.String,javax.swing.JComponent,java.lang.String,javax.swing.Icon))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID, [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) component, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) icon)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) [getComponent](#getComponent())()
Get the current component this view will display
  [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) [getIcon](#getIcon())()
Get the current view icon
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()
Get the view title
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getViewID](#getViewID())()
Gets the ID of the view.
  boolean [isCustomized](#isCustomized())()
Check if the view information has been customized.
  void [setComponent](#setComponent(javax.swing.JComponent))([JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) component)
Set a new component to be displayed in the view
  void [setIcon](#setIcon(javax.swing.Icon))([Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) icon)
Set the current view icon
  void [setTitle](#setTitle(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)
Set a new view title.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ViewInfo

public ViewInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) viewID, [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) component, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) icon)

Constructor
  Parameters: viewID - The unique view ID component - The component which will be placed inside title - Title for the view icon - The view's icon
## Method Details

### getViewID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getViewID()

Gets the ID of the view.
  Returns: The ID of the view.
### getComponent

public [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) getComponent()

Get the current component this view will display
  Returns: Returns the component.
### getTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()

Get the view title
  Returns: Returns the title.
### setComponent

public void setComponent([JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) component)

Set a new component to be displayed in the view
  Parameters: component - The component to set.
### setTitle

public void setTitle([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)

Set a new view title.
  Parameters: title - The title to set.
### getIcon

public [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) getIcon()

Get the current view icon
  Returns: Returns the icon.
### setIcon

public void setIcon([Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) icon)

Set the current view icon
  Parameters: icon - The icon to set.
### isCustomized

public boolean isCustomized()

Check if the view information has been customized.
  Returns: true if the view information has been customized.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
