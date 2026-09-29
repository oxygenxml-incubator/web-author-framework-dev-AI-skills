Package [ro.sync.ecss.extensions.api.webapp.cc](package-summary.md)

# Class CCItemProxy

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy
   All Implemented Interfaces: [AuthorCCItemTypes](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class CCItemProxy extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorCCItemTypes](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md)
An item proposed by the content completion manager, and which can be selected by the user. The item has a type, a name and a path for an icon to be displayed to the user that makes the selection.
  Since: 15.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [NORMAL_SORT_PRIORITY](#NORMAL_SORT_PRIORITY)
The priority for normal elements.
  static final int [SPLIT_ITEM_PRIORITY](#SPLIT_ITEM_PRIORITY)
The priority for "Split" / "New" type of entries.

### Fields inherited from interface ro.sync.ecss.contentcompletion.ccitems.[AuthorCCItemTypes](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md)
 [CDATA_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#CDATA_CC_ITEM), [COMMENT_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#COMMENT_CC_ITEM), [CUSTOM_ACTION_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#CUSTOM_ACTION_CC_ITEM), [CUSTOM_ELEMENT_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#CUSTOM_ELEMENT_CC_ITEM), [ELEMENT_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#ELEMENT_CC_ITEM), [ELEMENT_VALUE_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#ELEMENT_VALUE_CC_ITEM), [LINE_BREAK_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#LINE_BREAK_CC_ITEM), [PI_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#PI_CC_ITEM), [SPLIT_CC_ITEM](../../../../contentcompletion/ccitems/AuthorCCItemTypes.md#SPLIT_CC_ITEM)
## Constructor Summary
 Constructors
Constructor

Description
 [CCItemProxy](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getActionId](#getActionId())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAlias](#getAlias())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayName](#getDisplayName())()

 [CCItemProxy](CCItemProxy.md) [getElementProxy](#getElementProxy())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getIconPath](#getIconPath())()

 int [getSortPriority](#getSortPriority())()
This method returns the sort priority of a content completion item.
  int [getType](#getType())()

 boolean [isUseActionName](#isUseActionName())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### NORMAL_SORT_PRIORITY

public static final int NORMAL_SORT_PRIORITY

The priority for normal elements.
  Since: 21.1 See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy.NORMAL_SORT_PRIORITY)

### SPLIT_ITEM_PRIORITY

public static final int SPLIT_ITEM_PRIORITY

The priority for "Split" / "New" type of entries.
  Since: 21.1 See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy.SPLIT_ITEM_PRIORITY)

## Constructor Details

### CCItemProxy

public CCItemProxy()

## Method Details

### getDisplayName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayName()
  Returns: The display name of the content completion item.
### getIconPath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getIconPath()
  Returns: The icon path of the content completion item.
### getType

public int getType()
  Returns: The type of the content completion item.
### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description for a given item.
### getActionId

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getActionId()
  Returns: The action id, if this item is a replacement action item.
### getAlias

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAlias()
  Returns: The alias to be used as rendering string, if this item is a replacement action item.
### isUseActionName

public boolean isUseActionName()
  Returns: true to use the action name, if this item is a replacement action item.
### getSortPriority

public int getSortPriority()

This method returns the sort priority of a content completion item. By default it is [NORMAL_SORT_PRIORITY](#NORMAL_SORT_PRIORITY) for all items except for "Split"-type entries which have a priority of [SPLIT_ITEM_PRIORITY](#SPLIT_ITEM_PRIORITY).
  Returns: Returns the sort priority. The larger the priority the upper in the list the element is promoted. Since: 21.1
### getElementProxy

public [CCItemProxy](CCItemProxy.md) getElementProxy()
  Returns: Returns the proxy of the replaced element, if this item is a replacement action item.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
