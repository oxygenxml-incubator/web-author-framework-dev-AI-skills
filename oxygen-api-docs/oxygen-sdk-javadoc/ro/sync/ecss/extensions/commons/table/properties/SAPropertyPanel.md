Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class SAPropertyPanel

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.properties.SAPropertyPanel
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class SAPropertyPanel extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
This class will add to the given parent container a label with the property render string and a combobox containing all the possible values for the given property. It will return the user choice as a [TableProperty](TableProperty.md) object.

## Constructor Summary
 Constructors
Constructor

Description
 [SAPropertyPanel](#%3Cinit%3E(javax.swing.JPanel,java.awt.GridBagConstraints,ro.sync.ecss.extensions.commons.table.properties.TableProperty,ro.sync.ecss.extensions.api.AuthorResourceBundle,ro.sync.ecss.extensions.commons.table.properties.PropertySelectionController,int,boolean))([JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) parentContainer, [GridBagConstraints](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/GridBagConstraints.html) constr, [TableProperty](TableProperty.md) tableProperty, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [PropertySelectionController](PropertySelectionController.md) controller, int firstChildTopInset, boolean firstChild)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentlySelectedValue](#getCurrentlySelectedValue())()
Obtain the currently selected value;
  [TableProperty](TableProperty.md) [getModifiedProperty](#getModifiedProperty())()
Get the new table property.
  [TableProperty](TableProperty.md) [getTableProperty](#getTableProperty())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SAPropertyPanel

public SAPropertyPanel([JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) parentContainer, [GridBagConstraints](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/GridBagConstraints.html) constr, [TableProperty](TableProperty.md) tableProperty, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [PropertySelectionController](PropertySelectionController.md) controller, int firstChildTopInset, boolean firstChild)

Constructor.
  Parameters: parentContainer - The component that will contain the current property. constr - The [GridBagConstraints](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/GridBagConstraints.html) object. tableProperty - The table property that will be shown by the current panel. authorResourceBundle - The [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) object, which allow to i18n the property render string. controller - The controller used to update the dialog when a value is changed. firstChildTopInset - The top inset for the first child in parent. firstChild - true if the current panel is the first child of the given parent container.
## Method Details

### getModifiedProperty

public [TableProperty](TableProperty.md) getModifiedProperty()

Get the new table property. If the value of the given property is not modified, a null object will be return.
  Returns: The modified property or null if the property value was not changed.
### getCurrentlySelectedValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentlySelectedValue()

Obtain the currently selected value;
  Returns: The currently selected value for this property.
### getTableProperty

public [TableProperty](TableProperty.md) getTableProperty()
  Returns: Returns the table property.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
