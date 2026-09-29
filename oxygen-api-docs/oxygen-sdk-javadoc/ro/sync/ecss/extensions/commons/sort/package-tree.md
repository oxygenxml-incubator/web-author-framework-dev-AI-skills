# Hierarchy For Package ro.sync.ecss.extensions.commons.sort
 Package Hierarchies:
* [All Packages](../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.awt.[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) (implements java.awt.image.[ImageObserver](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ImageObserver.html), java.awt.[MenuContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/MenuContainer.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.awt.[Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html)

            * java.awt.[Window](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Window.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))

                * java.awt.[Dialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dialog.html)

                    * javax.swing.[JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[RootPaneContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/RootPaneContainer.html), javax.swing.[WindowConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/WindowConstants.html))

                        * ro.sync.exml.workspace.api.standalone.ui.[OKCancelDialog](../../../../exml/workspace/api/standalone/ui/OKCancelDialog.md) (implements ro.sync.ui.application.[HelpPageProvider](../../../../ui/application/HelpPageProvider.md))

                            * ro.sync.ecss.extensions.commons.ui.[OKCancelDialog](../ui/OKCancelDialog.md)

                                * ro.sync.ecss.extensions.commons.sort.[SASortCustomizerDialog](SASortCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.sort.[KeysController](KeysController.md), ro.sync.ecss.extensions.commons.sort.[SortCustomizer](SortCustomizer.md))

    * ro.sync.ecss.extensions.commons.sort.[CriterionComposite](CriterionComposite.md)
    * ro.sync.ecss.extensions.commons.sort.[CriterionInformation](CriterionInformation.md)
    * ro.sync.ecss.extensions.commons.sort.[CriterionPanel](CriterionPanel.md)
    * ro.sync.ecss.extensions.commons.sort.[SortCriteriaInformation](SortCriteriaInformation.md)
    * ro.sync.ecss.extensions.commons.sort.[SortOperation](SortOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.commons.sort.[DITAListSortOperation](DITAListSortOperation.md)
        * ro.sync.ecss.extensions.commons.sort.[DocbookListSortOperation](DocbookListSortOperation.md)
        * ro.sync.ecss.extensions.commons.sort.[TableSortOperation](TableSortOperation.md)
            * ro.sync.ecss.extensions.commons.sort.[SimpleTableSortOperation](SimpleTableSortOperation.md)

        * ro.sync.ecss.extensions.commons.sort.[TEIListSortOperation](TEIListSortOperation.md)
        * ro.sync.ecss.extensions.commons.sort.[XHTMLListSortOperation](XHTMLListSortOperation.md)

    * ro.sync.ecss.extensions.commons.sort.[SortUtil](SortUtil.md)
    * ro.sync.ecss.extensions.commons.sort.[TableSortUtil](TableSortUtil.md)
    * org.eclipse.jface.window.Window (implements org.eclipse.jface.window.IShellProvider)

        * org.eclipse.jface.dialogs.Dialog

            * org.eclipse.jface.dialogs.TrayDialog

                * ro.sync.ecss.extensions.commons.sort.[ECSortCustomizerDialog](ECSortCustomizerDialog.md) (implements ro.sync.ecss.extensions.commons.sort.[KeysController](KeysController.md), ro.sync.ecss.extensions.commons.sort.[SortCustomizer](SortCustomizer.md))

## Interface Hierarchy

* ro.sync.ecss.extensions.commons.sort.[KeysController](KeysController.md)
* ro.sync.ecss.extensions.commons.sort.[SortCustomizer](SortCustomizer.md)

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.ecss.extensions.commons.sort.[CriterionInformation.ORDER](CriterionInformation.ORDER.md)
        * ro.sync.ecss.extensions.commons.sort.[CriterionInformation.TYPE](CriterionInformation.TYPE.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
