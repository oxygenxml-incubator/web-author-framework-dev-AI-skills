Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class CriterionPanel

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.sort.CriterionPanel
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class CriterionPanel extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
This class will add to the given parent container a checkbox to enable the criterion, a combobox to select the key, a type combobox and order combobox. It will return the user choice as a [CriterionInformation](CriterionInformation.md) object.

## Constructor Summary
 Constructors
Constructor

Description
 [CriterionPanel](#%3Cinit%3E(java.awt.Container,java.awt.GridBagConstraints,java.util.List,ro.sync.ecss.extensions.commons.sort.CriterionInformation,ro.sync.ecss.extensions.api.AuthorResourceBundle,ro.sync.ecss.extensions.commons.sort.KeysController,java.util.List))([Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html) parent, [GridBagConstraints](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/GridBagConstraints.html) constr, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criterionInformation, [CriterionInformation](CriterionInformation.md) selectedItem, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [KeysController](KeysController.md) keysController, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> allCriteria)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [enableSortcriterion](#enableSortcriterion())()
Selects the checbox associated with the criterion panel, which means that the criterion information from it will be taken into account when sorting.
  [CriterionInformation](CriterionInformation.md) [getInformation](#getInformation())()
Returns the user input as a [CriterionInformation](CriterionInformation.md) object.
  [JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) [getKeyCombo](#getKeyCombo())()
Obtain the combo for the criterion key.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CriterionPanel

public CriterionPanel([Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html) parent, [GridBagConstraints](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/GridBagConstraints.html) constr, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criterionInformation, [CriterionInformation](CriterionInformation.md) selectedItem, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [KeysController](KeysController.md) keysController, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> allCriteria)

Constructor.
  Parameters: parent - The parent [Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html). constr - The [GridBagConstraints](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/GridBagConstraints.html) object. criterionInformation - The list of available criterion which will be added to the keys combobox. selectedItem - The item which will be selected in the keys combobox. authorResourceBundle - The reosurce bundle for i18n. keysController - The keys controller. allCriteria - All criteria information, not only the criteria information shown by the current criterion composite.
## Method Details

### getInformation

public [CriterionInformation](CriterionInformation.md) getInformation()

Returns the user input as a [CriterionInformation](CriterionInformation.md) object.
  Returns: The criterion information selected by the user in the current component.
### enableSortcriterion

public void enableSortcriterion()

Selects the checbox associated with the criterion panel, which means that the criterion information from it will be taken into account when sorting.

### getKeyCombo

public [JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) getKeyCombo()

Obtain the combo for the criterion key.
  Returns: Returns the combo for the criterion key.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
