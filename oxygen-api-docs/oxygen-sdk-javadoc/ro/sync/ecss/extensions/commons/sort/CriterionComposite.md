Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class CriterionComposite

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.sort.CriterionComposite
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class CriterionComposite extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
This class will add to the given parent container a checkbox to enable the criterion, a combobox to select the key, a type combobox and order combobox. It will return the user choice as a [CriterionInformation](CriterionInformation.md) object.

## Constructor Summary
 Constructors
Constructor

Description
 [CriterionComposite](#%3Cinit%3E(org.eclipse.swt.widgets.Composite,ro.sync.ecss.extensions.api.AuthorResourceBundle,java.util.List,ro.sync.ecss.extensions.commons.sort.CriterionInformation,boolean,ro.sync.ecss.extensions.commons.sort.KeysController,java.util.List))(org.eclipse.swt.widgets.Composite parent, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criterionInformation, [CriterionInformation](CriterionInformation.md) selectedItem, boolean isFirstCriterion, [KeysController](KeysController.md) keysController, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> allCriteria)
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
  org.eclipse.swt.widgets.Combo [getKeyCombo](#getKeyCombo())()
Obtain access to the keys combobox.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CriterionComposite

public CriterionComposite(org.eclipse.swt.widgets.Composite parent, [AuthorResourceBundle](../../api/AuthorResourceBundle.md) authorResourceBundle, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criterionInformation, [CriterionInformation](CriterionInformation.md) selectedItem, boolean isFirstCriterion, [KeysController](KeysController.md) keysController, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> allCriteria)

Constructor.
  Parameters: parent - The parent composite. authorResourceBundle - The Author resource bundle criterionInformation - The list of available criterion which will be added to the keys combobox. selectedItem - The item which will be selected in the keys combobox. isFirstCriterion - true if the titles for every component of the current composite should be displayed. keysController - The keys combo controller. allCriteria - All criteria information, not only the criteria information shown by the current criterion composite.
## Method Details

### getKeyCombo

public org.eclipse.swt.widgets.Combo getKeyCombo()

Obtain access to the keys combobox.
  Returns: Returns the keys combobox.
### getInformation

public [CriterionInformation](CriterionInformation.md) getInformation()

Returns the user input as a [CriterionInformation](CriterionInformation.md) object.
  Returns: The criterion information selected by the user in the current component.
### enableSortcriterion

public void enableSortcriterion()

Selects the checbox associated with the criterion panel, which means that the criterion information from it will be taken into account when sorting.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
