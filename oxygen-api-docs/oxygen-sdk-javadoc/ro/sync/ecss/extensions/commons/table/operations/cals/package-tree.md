# Hierarchy For Package ro.sync.ecss.extensions.commons.table.operations.cals
 Package Hierarchies:
* [All Packages](../../../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](../../../AbstractDocumentTypeHelper.md) (implements ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](../AuthorTableHelper.md))
        * ro.sync.ecss.extensions.commons.table.operations.cals.[CALSDocumentTypeHelper](CALSDocumentTypeHelper.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md))

    * ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../AbstractTableOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.commons.table.operations.[DeleteColumnOperationBase](../DeleteColumnOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[DeleteColumnOperation](DeleteColumnOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md))

        * ro.sync.ecss.extensions.commons.table.operations.[DeleteRowOperationBase](../DeleteRowOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[DeleteRowOperation](DeleteRowOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md))

        * ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../InsertColumnOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[InsertColumnOperation](InsertColumnOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md), ro.sync.ecss.extensions.commons.table.operations.[InsertTableCellsContentConstants](../InsertTableCellsContentConstants.md))

                * ro.sync.ecss.extensions.commons.table.operations.cals.[InsertSingleColumnOperation](InsertSingleColumnOperation.md)

        * ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../InsertRowOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[InsertRowOperation](InsertRowOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md), ro.sync.ecss.extensions.commons.table.operations.[InsertTableCellsContentConstants](../InsertTableCellsContentConstants.md))

                * ro.sync.ecss.extensions.commons.table.operations.cals.[InsertSingleRowOperation](InsertSingleRowOperation.md)

        * ro.sync.ecss.extensions.commons.table.operations.[JoinCellAboveBelowOperationBase](../JoinCellAboveBelowOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[JoinCellAboveBelowOperation](JoinCellAboveBelowOperation.md)

        * ro.sync.ecss.extensions.commons.table.operations.[JoinOperationBase](../JoinOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[JoinOperation](JoinOperation.md)

        * ro.sync.ecss.extensions.commons.table.operations.[JoinRowCellsOperationBase](../JoinRowCellsOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[JoinRowCellsOperation](JoinRowCellsOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md))

        * ro.sync.ecss.extensions.commons.table.operations.[SplitCellAboveBelowOperationBase](../SplitCellAboveBelowOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[SplitCellAboveBelowOperation](SplitCellAboveBelowOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md))

        * ro.sync.ecss.extensions.commons.table.operations.[SplitLeftRightOperationBase](../SplitLeftRightOperationBase.md)
            * ro.sync.ecss.extensions.commons.table.operations.cals.[SplitLeftRightOperation](SplitLeftRightOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md))

        * ro.sync.ecss.extensions.commons.table.operations.[SplitOperationBase](../SplitOperationBase.md)

            * ro.sync.ecss.extensions.commons.table.operations.cals.[SplitOperation](SplitOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md))

    * ro.sync.ecss.extensions.commons.sort.[SortOperation](../../../sort/SortOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.commons.sort.[TableSortOperation](../../../sort/TableSortOperation.md)

            * ro.sync.ecss.extensions.commons.table.operations.cals.[CALSAndHTMLTableSortOperation](CALSAndHTMLTableSortOperation.md)

    * ro.sync.ecss.extensions.api.table.operations.[TableColumnSpecificationInformation](../../../../api/table/operations/TableColumnSpecificationInformation.md) (implements ro.sync.ecss.component.[AuthorContentMetadata](../../../../../component/AuthorContentMetadata.md))

        * ro.sync.ecss.extensions.commons.table.operations.cals.[CALSTableColumnSpecificationInformation](CALSTableColumnSpecificationInformation.md)

## Interface Hierarchy

* ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](CALSConstants.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
