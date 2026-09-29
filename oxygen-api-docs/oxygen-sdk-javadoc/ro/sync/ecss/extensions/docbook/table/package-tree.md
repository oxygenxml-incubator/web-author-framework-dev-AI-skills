# Hierarchy For Package ro.sync.ecss.extensions.docbook.table
 Package Hierarchies:
* [All Packages](../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../commons/table/operations/AbstractTableOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.docbook.table.[InsertTableOperation](InsertTableOperation.md) (implements ro.sync.ecss.extensions.commons.table.operations.[InsertTableCellsContentConstants](../../commons/table/operations/InsertTableCellsContentConstants.md), ro.sync.ecss.extensions.commons.table.operations.[InsertTableOperationBase](../../commons/table/operations/InsertTableOperationBase.md))

    * ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](../../api/AuthorTableColumnWidthProviderBase.md) (implements ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProvider](../../api/AuthorTableColumnWidthProvider.md))
        * ro.sync.ecss.extensions.commons.table.support.[CALSTableCellInfoProvider](../../commons/table/support/CALSTableCellInfoProvider.md) (implements ro.sync.ecss.extensions.api.[AuthorTableCellSepProvider](../../api/AuthorTableCellSepProvider.md), ro.sync.ecss.extensions.api.[AuthorTableCellSpanProvider](../../api/AuthorTableCellSpanProvider.md), ro.sync.ecss.extensions.commons.table.operations.cals.[CALSConstants](../../commons/table/operations/cals/CALSConstants.md))

            * ro.sync.ecss.extensions.docbook.table.[DocbookTableCellSepInfoProvider](DocbookTableCellSepInfoProvider.md)

    * java.awt.[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) (implements java.awt.image.[ImageObserver](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ImageObserver.html), java.awt.[MenuContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/MenuContainer.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.awt.[Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html)

            * java.awt.[Window](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Window.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))

                * java.awt.[Dialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dialog.html)

                    * javax.swing.[JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[RootPaneContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/RootPaneContainer.html), javax.swing.[WindowConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/WindowConstants.html))

                        * ro.sync.exml.workspace.api.standalone.ui.[OKCancelDialog](../../../../exml/workspace/api/standalone/ui/OKCancelDialog.md) (implements ro.sync.ui.application.[HelpPageProvider](../../../../ui/application/HelpPageProvider.md))

                            * ro.sync.ecss.extensions.commons.ui.[OKCancelDialog](../../commons/ui/OKCancelDialog.md)

                                * ro.sync.ecss.extensions.commons.table.operations.[SATableCustomizerDialog](../../commons/table/operations/SATableCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../../commons/table/operations/TableCustomizerConstants.md))

                                    * ro.sync.ecss.extensions.docbook.table.[SADocbookTableCustomizerDialog](SADocbookTableCustomizerDialog.md)

                                        * ro.sync.ecss.extensions.docbook.table.[SADocbook4TableCustomizerDialog](SADocbook4TableCustomizerDialog.md)
                                        * ro.sync.ecss.extensions.docbook.table.[SADocbook5TableCustomizerDialog](SADocbook5TableCustomizerDialog.md)

    * ro.sync.ecss.extensions.commons.sort.[SortOperation](../../commons/sort/SortOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.commons.sort.[TableSortOperation](../../commons/sort/TableSortOperation.md)

            * ro.sync.ecss.extensions.commons.table.operations.cals.[CALSAndHTMLTableSortOperation](../../commons/table/operations/cals/CALSAndHTMLTableSortOperation.md)

                * ro.sync.ecss.extensions.docbook.table.[DocbookCALSTableSortOperation](DocbookCALSTableSortOperation.md)

    * ro.sync.ecss.extensions.commons.table.operations.[TableCustomizer](../../commons/table/operations/TableCustomizer.md)
        * ro.sync.ecss.extensions.docbook.table.[ECDocbookInnerTableCustomizer](ECDocbookInnerTableCustomizer.md)
        * ro.sync.ecss.extensions.docbook.table.[ECDocbookTableCustomizer](ECDocbookTableCustomizer.md)
        * ro.sync.ecss.extensions.docbook.table.[SADocbookInnerTableCustomizer](SADocbookInnerTableCustomizer.md)
        * ro.sync.ecss.extensions.docbook.table.[SADocbookTableCustomizer](SADocbookTableCustomizer.md)

    * org.eclipse.jface.window.Window (implements org.eclipse.jface.window.IShellProvider)

        * org.eclipse.jface.dialogs.Dialog

            * org.eclipse.jface.dialogs.TrayDialog

                * ro.sync.ecss.extensions.commons.table.operations.[ECTableCustomizerDialog](../../commons/table/operations/ECTableCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../../commons/table/operations/TableCustomizerConstants.md))

                    * ro.sync.ecss.extensions.docbook.table.[ECDocbookTableCustomizerDialog](ECDocbookTableCustomizerDialog.md)

## Interface Hierarchy

* ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../../commons/table/operations/TableCustomizerConstants.md)

    * ro.sync.ecss.extensions.docbook.table.[DocbookTableCustomizerConstants](DocbookTableCustomizerConstants.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
