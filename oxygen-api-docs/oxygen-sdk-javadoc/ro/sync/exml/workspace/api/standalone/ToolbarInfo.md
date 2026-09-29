Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Class ToolbarInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.ToolbarInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class ToolbarInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Information about a toolbar.
  Since: 11.2
## Constructor Summary
 Constructors
Constructor

Description
 [ToolbarInfo](#%3Cinit%3E(java.lang.String,javax.swing.JComponent%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID, [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html)[] components, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html)[] [getComponents](#getComponents())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getToolbarID](#getToolbarID())()

 boolean [isCustomized](#isCustomized())()
Check if the toolbar info has been customizer.
  void [setComponents](#setComponents(javax.swing.JComponent%5B%5D))([JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html)[] components)
Set the toolbar components
  void [setTitle](#setTitle(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)
Set the toolbar title

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ToolbarInfo

public ToolbarInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarID, [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html)[] components, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)

Constructor
  Parameters: toolbarID - The unique toolbar ID components - The components array title - Title for the toolbar
## Method Details

### getToolbarID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getToolbarID()
  Returns: Returns the toolbarID.
### getComponents

public [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html)[] getComponents()
  Returns: Returns the components.
### getTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()
  Returns: Returns the title.
### setComponents

public void setComponents([JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html)[] components)

Set the toolbar components
  Parameters: components - The components to set.
### setTitle

public void setTitle([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)

Set the toolbar title
  Parameters: title - The title to set.
### isCustomized

public boolean isCustomized()

Check if the toolbar info has been customizer.
  Returns: true if the toolbar info has been customizer.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
