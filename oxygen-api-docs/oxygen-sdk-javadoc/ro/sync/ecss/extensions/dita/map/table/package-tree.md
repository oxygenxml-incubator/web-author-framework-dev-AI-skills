# Hierarchy For Package ro.sync.ecss.extensions.dita.map.table
 Package Hierarchies:
* [All Packages](../../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](../../../commons/AbstractDocumentTypeHelper.md) (implements ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](../../../commons/table/operations/AuthorTableHelper.md))
        * ro.sync.ecss.extensions.dita.map.table.[DITARelTableDocumentTypeHelper](DITARelTableDocumentTypeHelper.md) (implements ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md))

    * ro.sync.ecss.extensions.commons.table.operations.[AbstractTableOperation](../../../commons/table/operations/AbstractTableOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.commons.table.operations.[DeleteColumnOperationBase](../../../commons/table/operations/DeleteColumnOperationBase.md)
            * ro.sync.ecss.extensions.dita.map.table.[DeleteColumnOperation](DeleteColumnOperation.md) (implements ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md))

        * ro.sync.ecss.extensions.commons.table.operations.[DeleteRowOperationBase](../../../commons/table/operations/DeleteRowOperationBase.md)
            * ro.sync.ecss.extensions.dita.map.table.[DeleteRowOperation](DeleteRowOperation.md) (implements ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md))

        * ro.sync.ecss.extensions.commons.table.operations.[InsertColumnOperationBase](../../../commons/table/operations/InsertColumnOperationBase.md)
            * ro.sync.ecss.extensions.dita.map.table.[InsertColumnOperation](InsertColumnOperation.md) (implements ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md))

                * ro.sync.ecss.extensions.dita.map.table.[InsertSingleColumnOperation](InsertSingleColumnOperation.md)

        * ro.sync.ecss.extensions.commons.table.operations.[InsertRowOperationBase](../../../commons/table/operations/InsertRowOperationBase.md)
            * ro.sync.ecss.extensions.dita.map.table.[InsertRowOperation](InsertRowOperation.md) (implements ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md))

                * ro.sync.ecss.extensions.dita.map.table.[InsertSingleRowOperation](InsertSingleRowOperation.md)

        * ro.sync.ecss.extensions.commons.table.operations.[JoinCellAboveBelowOperationBase](../../../commons/table/operations/JoinCellAboveBelowOperationBase.md)
            * ro.sync.ecss.extensions.dita.map.table.[JoinCellAboveBelowOperation](JoinCellAboveBelowOperation.md)

        * ro.sync.ecss.extensions.commons.table.operations.[JoinRowCellsOperationBase](../../../commons/table/operations/JoinRowCellsOperationBase.md)

            * ro.sync.ecss.extensions.dita.map.table.[JoinRowCellsOperation](JoinRowCellsOperation.md) (implements ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md))

    * java.awt.[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) (implements java.awt.image.[ImageObserver](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ImageObserver.html), java.awt.[MenuContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/MenuContainer.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.awt.[Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html)

            * java.awt.[Window](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Window.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))

                * java.awt.[Dialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dialog.html)

                    * javax.swing.[JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[RootPaneContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/RootPaneContainer.html), javax.swing.[WindowConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/WindowConstants.html))

                        * ro.sync.exml.workspace.api.standalone.ui.[OKCancelDialog](../../../../../exml/workspace/api/standalone/ui/OKCancelDialog.md) (implements ro.sync.ui.application.[HelpPageProvider](../../../../../ui/application/HelpPageProvider.md))

                            * ro.sync.ecss.extensions.commons.ui.[OKCancelDialog](../../../commons/ui/OKCancelDialog.md)

                                * ro.sync.ecss.extensions.commons.table.operations.[SATableCustomizerDialog](../../../commons/table/operations/SATableCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../../../commons/table/operations/TableCustomizerConstants.md))

                                    * ro.sync.ecss.extensions.dita.map.table.[SADITARelTableCustomizerDialog](SADITARelTableCustomizerDialog.md)

    * ro.sync.ecss.extensions.dita.map.table.[InsertTableOperation](InsertTableOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md), ro.sync.ecss.extensions.commons.table.operations.[InsertTableOperationBase](../../../commons/table/operations/InsertTableOperationBase.md))
    * ro.sync.ecss.extensions.dita.map.table.[ReltableCellSpanProvider](ReltableCellSpanProvider.md) (implements ro.sync.ecss.extensions.api.[AuthorTableCellSpanProvider](../../../api/AuthorTableCellSpanProvider.md))
    * ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](../../../commons/table/properties/ShowTablePropertiesBaseOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.dita.map.table.[RelTableShowPropertiesOperation](RelTableShowPropertiesOperation.md)

    * ro.sync.ecss.extensions.commons.table.operations.[TableCustomizer](../../../commons/table/operations/TableCustomizer.md)
        * ro.sync.ecss.extensions.dita.map.table.[ECDITARelTableCustomizer](ECDITARelTableCustomizer.md)
        * ro.sync.ecss.extensions.dita.map.table.[SADITARelTableCustomizer](SADITARelTableCustomizer.md)

    * ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelperBase](../../../commons/table/properties/TablePropertiesHelperBase.md) (implements ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelper](../../../commons/table/properties/TablePropertiesHelper.md))
        * ro.sync.ecss.extensions.dita.map.table.[RelTablePropertiesHelper](RelTablePropertiesHelper.md)

    * org.eclipse.jface.window.Window (implements org.eclipse.jface.window.IShellProvider)

        * org.eclipse.jface.dialogs.Dialog

            * org.eclipse.jface.dialogs.TrayDialog

                * ro.sync.ecss.extensions.commons.table.operations.[ECTableCustomizerDialog](../../../commons/table/operations/ECTableCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.table.operations.[TableCustomizerConstants](../../../commons/table/operations/TableCustomizerConstants.md))

                    * ro.sync.ecss.extensions.dita.map.table.[ECDITARelTableCustomizerDialog](ECDITARelTableCustomizerDialog.md)

## Interface Hierarchy

* ro.sync.ecss.extensions.dita.map.table.[ReltableConstants](ReltableConstants.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
