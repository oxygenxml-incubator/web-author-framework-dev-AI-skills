Package [ro.sync.ecss.extensions.api.table.operations](package-summary.md)

# Class TableColumnSpecificationInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [AuthorContentMetadata](../../../../component/AuthorContentMetadata.md)   Direct Known Subclasses: [CALSTableColumnSpecificationInformation](../../../commons/table/operations/cals/CALSTableColumnSpecificationInformation.md)   @API(type=EXTENDABLE, src=PUBLIC) public class TableColumnSpecificationInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorContentMetadata](../../../../component/AuthorContentMetadata.md)
Contains information about column specification (like column specified width). It can be extended to provide specific table column properties for different types of tables or document types. This information is requested when a column is copied or dragged and it can be used when the column must be inserted in the document (on paste or drop). Please note that when a column is copied the table column specification information will be copied into the clipboard (the AuthorClipboardObject contains a field of [TableColumnSpecificationInformation](TableColumnSpecificationInformation.md) type), so it will be serialized. The column specification is send as an argument to the [AuthorTableOperationsHandler.handleInsertColumn(AuthorTableInsertColumnArguments)](AuthorTableOperationsHandler.md#handleInsertColumn(ro.sync.ecss.extensions.api.table.operations.AuthorTableInsertColumnArguments)) method and it can be used to keep informations like column name or column width unchchanged when the column is moved or copy-pasted.
  Since: 14 See Also:
* [Serialized Form](../../../../../../../serialized-form.md#ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation)

## Constructor Summary
 Constructors
Constructor

Description
 [TableColumnSpecificationInformation](#%3Cinit%3E(ro.sync.ecss.extensions.api.WidthRepresentation))([WidthRepresentation](../../WidthRepresentation.md) widthRepresentation)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [WidthRepresentation](../../WidthRepresentation.md) [getWidthRepresentation](#getWidthRepresentation())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TableColumnSpecificationInformation

public TableColumnSpecificationInformation([WidthRepresentation](../../WidthRepresentation.md) widthRepresentation)

Constructor.
  Parameters: widthRepresentation - The column width representation that specifies the fixed and relative width determined from the column specification.
## Method Details

### getWidthRepresentation

public [WidthRepresentation](../../WidthRepresentation.md) getWidthRepresentation()
  Returns: Returns the column width representation that specifies the fixed and relative width determined from the column specification.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
