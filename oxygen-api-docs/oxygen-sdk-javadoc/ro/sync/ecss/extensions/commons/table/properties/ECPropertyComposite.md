Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class ECPropertyComposite

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.properties.ECPropertyComposite
   @API(type=INTERNAL, src=PUBLIC) public class ECPropertyComposite extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The composite used to edit a table property.

## Constructor Summary
 Constructors
Constructor

Description
 [ECPropertyComposite](#%3Cinit%3E(org.eclipse.swt.widgets.Composite,ro.sync.ecss.extensions.commons.table.properties.TableProperty,ro.sync.ecss.extensions.api.AuthorResourceBundle,ro.sync.ecss.extensions.commons.table.properties.PropertySelectionController,boolean))(org.eclipse.swt.widgets.Composite parent, [TableProperty](TableProperty.md) tableProperty, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [PropertySelectionController](PropertySelectionController.md) controller, boolean firstChild)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCurrentlySelectedValue](#getCurrentlySelectedValue())()
Obtain the current selected value for this property.
  [TableProperty](TableProperty.md) [getModifiedProperty](#getModifiedProperty())()
Get the new table property.
  [TableProperty](TableProperty.md) [getTableProperty](#getTableProperty())()
The current edited table property.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECPropertyComposite

public ECPropertyComposite(org.eclipse.swt.widgets.Composite parent, [TableProperty](TableProperty.md) tableProperty, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [PropertySelectionController](PropertySelectionController.md) controller, boolean firstChild)

Constructor.
  Parameters: parent - The parent composite. tableProperty - The table property that is edited using the current composite. authorResourceBundle - The author resource bundle. It is used for translation. controller - The property controller. firstChild - true if the current property is the first child in the given parent.
## Method Details

### getModifiedProperty

public [TableProperty](TableProperty.md) getModifiedProperty()

Get the new table property. If the value of the given property is not modified, a null will be return.
  Returns: The modified property or null if the property value was not changed.
### getTableProperty

public [TableProperty](TableProperty.md) getTableProperty()

The current edited table property.
  Returns: Returns the corresponding table property.
### getCurrentlySelectedValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCurrentlySelectedValue()

Obtain the current selected value for this property.
  Returns: The current selected value of the table property.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
