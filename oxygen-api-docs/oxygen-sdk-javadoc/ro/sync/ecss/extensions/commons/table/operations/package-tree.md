# Hierarchy For Package ro.sync.ecss.extensions.commons.table.operations
 Package Hierarchies:
* [All Packages](../../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](AbstractTableOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.commons.table.operations.[DeleteColumnOperationBase](DeleteColumnOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[DeleteRowOperationBase](DeleteRowOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](InsertColumnOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](InsertRowOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[JoinCellAboveBelowOperationBase](JoinCellAboveBelowOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[JoinOperationBase](JoinOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[JoinRowCellsOperationBase](JoinRowCellsOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[SplitCellAboveBelowOperationBase](SplitCellAboveBelowOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[SplitLeftRightOperationBase](SplitLeftRightOperationBase.md)
        * ro.sync.ecss.extensions.commons.table.operations.[SplitOperationBase](SplitOperationBase.md)

    * java.awt.[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) (implements java.awt.image.[ImageObserver](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ImageObserver.html), java.awt.[MenuContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/MenuContainer.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.awt.[Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html)

            * java.awt.[Window](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Window.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))

                * java.awt.[Dialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dialog.html)

                    * javax.swing.[JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[RootPaneContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/RootPaneContainer.html), javax.swing.[WindowConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/WindowConstants.html))

                        * ro.sync.exml.workspace.api.standalone.ui.[OKCancelDialog](../../../../../exml/workspace/api/standalone/ui/OKCancelDialog.md) (implements ro.sync.ui.application.[HelpPageProvider](../../../../../ui/application/HelpPageProvider.md))

                            * ro.sync.ecss.extensions.commons.ui.[OKCancelDialog](../../ui/OKCancelDialog.md)
                                * ro.sync.ecss.extensions.commons.table.operations.[SACustomTableColumnInsertionDialog](SACustomTableColumnInsertionDialog.md)
                                * ro.sync.ecss.extensions.commons.table.operations.[SACustomTableRowInsertionDialog](SACustomTableRowInsertionDialog.md)
                                * ro.sync.ecss.extensions.commons.table.operations.[SATableCustomizerDialog](SATableCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](TableCustomizerConstants.md))

                            * ro.sync.ecss.extensions.commons.table.operations.[SATableSplitCustomizerDialog](SATableSplitCustomizerDialog.md)

    * ro.sync.ecss.extensions.commons.table.operations.[ListContentProvider](ListContentProvider.md) (implements org.eclipse.jface.viewers.IStructuredContentProvider)
    * ro.sync.ecss.extensions.commons.table.operations.[TableColumnInsertionCustomizer](TableColumnInsertionCustomizer.md)
        * ro.sync.ecss.extensions.commons.table.operations.[ECTableColumnInsertionCustomizerInvoker](ECTableColumnInsertionCustomizerInvoker.md)
        * ro.sync.ecss.extensions.commons.table.operations.[SATableColumnInsertionCustomizerInvoker](SATableColumnInsertionCustomizerInvoker.md)

    * ro.sync.ecss.extensions.commons.table.operations.[TableColumnsInfo](TableColumnsInfo.md)
    * ro.sync.ecss.extensions.commons.table.operations.[TableCustomizer](TableCustomizer.md)
    * ro.sync.ecss.extensions.commons.table.operations.[TableInfo](TableInfo.md) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
    * ro.sync.ecss.extensions.commons.table.operations.[TableOperationsUtil](TableOperationsUtil.md)
    * ro.sync.ecss.extensions.commons.table.operations.[TableRowInsertionCustomizer](TableRowInsertionCustomizer.md)
        * ro.sync.ecss.extensions.commons.table.operations.[ECTableRowInsertionCustomizerInvoker](ECTableRowInsertionCustomizerInvoker.md)
        * ro.sync.ecss.extensions.commons.table.operations.[SATableRowInsertionCustomizerInvoker](SATableRowInsertionCustomizerInvoker.md)

    * ro.sync.ecss.extensions.commons.table.operations.[TableRowsInfo](TableRowsInfo.md)
    * org.eclipse.jface.window.Window (implements org.eclipse.jface.window.IShellProvider)

        * org.eclipse.jface.dialogs.Dialog

            * org.eclipse.jface.dialogs.TrayDialog

                * ro.sync.ecss.extensions.commons.table.operations.[ECCustomTableColumnInsertionDialog](ECCustomTableColumnInsertionDialog.md)
                * ro.sync.ecss.extensions.commons.table.operations.[ECCustomTableRowInsertionDialog](ECCustomTableRowInsertionDialog.md)
                * ro.sync.ecss.extensions.commons.table.operations.[ECTableCustomizerDialog](ECTableCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](TableCustomizerConstants.md))
                * ro.sync.ecss.extensions.commons.table.operations.[ECTableSplitCustomizerDialog](ECTableSplitCustomizerDialog.md)

## Interface Hierarchy

* ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](AuthorTableHelper.md)
* ro.sync.ecss.extensions.commons.table.operations.[InsertTableCellsContentConstants](InsertTableCellsContentConstants.md)
* ro.sync.ecss.extensions.commons.table.operations.[InsertTableOperationBase](InsertTableOperationBase.md)
* ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](TableCustomizerConstants.md)

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants.ColumnWidthsType](TableCustomizerConstants.ColumnWidthsType.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
