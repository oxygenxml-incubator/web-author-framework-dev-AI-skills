Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class EditedTablePropertiesInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo
   @API(type=INTERNAL, src=PUBLIC) public class EditedTablePropertiesInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md)
Enumeration that contains the elements for every tab type.

## Constructor Summary
 Constructors
Constructor

Description
 [EditedTablePropertiesInfo](#%3Cinit%3E(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> categories)
Constructor.
  [EditedTablePropertiesInfo](#%3Cinit%3E(java.util.List,ro.sync.ecss.extensions.commons.table.properties.EditedTablePropertiesInfo.TAB_TYPE))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> categories, [EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md) selectedTab)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> [getCategories](#getCategories())()

 [EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md) [getSelectedTab](#getSelectedTab())()
Obtain the tab that is selected when the dialog is shown.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditedTablePropertiesInfo

public EditedTablePropertiesInfo([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> categories)

Constructor. This constructor will consider that table tab should be selected when the "Table Properties" dialog is shown.
  Parameters: categories - The properties that will be edited in the table properties for the given element. The element will be also the tab name in the dialog.
### EditedTablePropertiesInfo

public EditedTablePropertiesInfo([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> categories, [EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md) selectedTab)

Constructor.
  Parameters: categories - The properties that will be edited in the table properties for the given element. The element will be also the tab name in the dialog. selectedTab - The tab that is selected when the dialog is shown.
## Method Details

### getCategories

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TabInfo](TabInfo.md)> getCategories()
  Returns: Returns the table properties mapped to the element name/alias.
### getSelectedTab

public [EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md) getSelectedTab()

Obtain the tab that is selected when the dialog is shown.
  Returns: The tab that is selected when the dialog is shown.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
