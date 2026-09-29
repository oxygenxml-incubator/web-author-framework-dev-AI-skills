Package [ro.sync.ecss.extensions.commons.table.spansupport](package-summary.md)

# Class TEITableCellSpanProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.spansupport.TEITableCellSpanProvider
   All Implemented Interfaces: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md), [Extension](../../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class TEITableCellSpanProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md)
Provides cell spanning information about TEI tables.

## Constructor Summary
 Constructors
Constructor

Description
 [TEITableCellSpanProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getColSpan](#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) cellElement)
Compute the number of columns the cell spans across by looking at the 'cols' attribute.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) [getRowSpan](#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) cellElement)
Compute the number of rows the cell spans across by looking at the 'rows' attribute.
  boolean [hasColumnSpecifications](#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
This method tells if the table contains column specifications.
  void [init](#init(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
Nothing to do.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TEITableCellSpanProvider

public TEITableCellSpanProvider()

## Method Details

### getColSpan

public [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getColSpan([AuthorElement](../../../api/node/AuthorElement.md) cellElement)

Compute the number of columns the cell spans across by looking at the 'cols' attribute.
  Specified by: [getColSpan](../../../api/AuthorTableCellSpanProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: cellElement - The node that represents a table cell in CSS. Returns: The number of columns this cell spans across (the minimum returned value must be 1) or null if not specified. See Also:
        * [AuthorTableCellSpanProvider.getColSpan(AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#getColSpan(ro.sync.ecss.extensions.api.node.AuthorElement))

### getRowSpan

public [Integer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Integer.html) getRowSpan([AuthorElement](../../../api/node/AuthorElement.md) cellElement)

Compute the number of rows the cell spans across by looking at the 'rows' attribute.
  Specified by: [getRowSpan](../../../api/AuthorTableCellSpanProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: cellElement - The [AuthorElement](../../../api/node/AuthorElement.md) that represents a table cell in CSS. Returns: The number of rows this cell spans across (the minimum returned value must be 1) or null if not specified. See Also:
        * [AuthorTableCellSpanProvider.getRowSpan(AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#getRowSpan(ro.sync.ecss.extensions.api.node.AuthorElement))

### init

public void init([AuthorElement](../../../api/node/AuthorElement.md) tableElement)

Nothing to do. Cell spanning information in a TEI table is given through the attributes of the cell element.
  Specified by: [init](../../../api/AuthorTableCellSpanProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: tableElement - The [AuthorElement](../../../api/node/AuthorElement.md) representing a table (it has the CSS display property set on 'table'). See Also:
        * [AuthorTableCellSpanProvider.init(AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#init(ro.sync.ecss.extensions.api.node.AuthorElement))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../../api/Extension.md#getDescription()) in interface [Extension](../../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### hasColumnSpecifications

public boolean hasColumnSpecifications([AuthorElement](../../../api/node/AuthorElement.md) tableElement)
 Description copied from interface: [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))
This method tells if the table contains column specifications. For example the CALS table model requires colspec elements to be present.
  Specified by: [hasColumnSpecifications](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)) in interface [AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md) Parameters: tableElement - The [AuthorElement](../../../api/node/AuthorElement.md) that is rendered as a table. Returns: true if some column specification info is present or if the table doesn't require any column specification info. See Also:
        * [AuthorTableCellSpanProvider.hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement)](../../../api/AuthorTableCellSpanProvider.md#hasColumnSpecifications(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
