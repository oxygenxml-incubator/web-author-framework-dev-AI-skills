# Hierarchy For Package ro.sync.ecss.extensions.commons.table.properties
 Package Hierarchies:
* [All Packages](../../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.awt.[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) (implements java.awt.image.[ImageObserver](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ImageObserver.html), java.awt.[MenuContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/MenuContainer.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.awt.[Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html)

            * java.awt.[Window](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Window.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))

                * java.awt.[Dialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dialog.html)

                    * javax.swing.[JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[RootPaneContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/RootPaneContainer.html), javax.swing.[WindowConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/WindowConstants.html))

                        * ro.sync.exml.workspace.api.standalone.ui.[OKCancelDialog](../../../../../exml/workspace/api/standalone/ui/OKCancelDialog.md) (implements ro.sync.ui.application.[HelpPageProvider](../../../../../ui/application/HelpPageProvider.md))

                            * ro.sync.ecss.extensions.commons.ui.[OKCancelDialog](../../ui/OKCancelDialog.md)

                                * ro.sync.ecss.extensions.commons.table.properties.[SATablePropertiesCustomizerDialog](SATablePropertiesCustomizerDialog.md)

    * ro.sync.ecss.extensions.commons.table.properties.[ECPropertyComposite](ECPropertyComposite.md)
    * ro.sync.ecss.extensions.commons.table.properties.[EditedTablePropertiesInfo](EditedTablePropertiesInfo.md)
    * ro.sync.ecss.extensions.commons.table.properties.[SAPropertyPanel](SAPropertyPanel.md)
    * ro.sync.ecss.extensions.commons.table.properties.[ShowTablePropertiesBaseOperation](ShowTablePropertiesBaseOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.commons.table.properties.[CALSAndHTMLShowTablePropertiesBase](CALSAndHTMLShowTablePropertiesBase.md)

            * ro.sync.ecss.extensions.commons.table.properties.[CALSShowTableProperties](CALSShowTableProperties.md)

    * ro.sync.ecss.extensions.commons.table.properties.[TabInfo](TabInfo.md)
    * ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelperBase](TablePropertiesHelperBase.md) (implements ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelper](TablePropertiesHelper.md))
    * ro.sync.ecss.extensions.commons.table.properties.[TableProperty](TableProperty.md)
    * org.eclipse.swt.widgets.Widget
        * org.eclipse.swt.widgets.Control (implements org.eclipse.swt.graphics.Drawable)

            * org.eclipse.swt.widgets.Scrollable

                * org.eclipse.swt.widgets.Composite

                    * ro.sync.ecss.extensions.commons.table.properties.[ECPropertiesComposite](ECPropertiesComposite.md) (implements ro.sync.ecss.extensions.commons.table.properties.[PropertySelectionController](PropertySelectionController.md))

    * org.eclipse.jface.window.Window (implements org.eclipse.jface.window.IShellProvider)

        * org.eclipse.jface.dialogs.Dialog

            * org.eclipse.jface.dialogs.TrayDialog

                * ro.sync.ecss.extensions.commons.table.properties.[ECTablePropertiesCustomizerDialog](ECTablePropertiesCustomizerDialog.md)

## Interface Hierarchy

* ro.sync.ecss.extensions.commons.table.properties.[PropertySelectionController](PropertySelectionController.md)
* ro.sync.ecss.extensions.commons.table.properties.[TableHelper](TableHelper.md)
    * ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelper](TablePropertiesHelper.md) (also extends ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesConstants](TablePropertiesConstants.md))

* ro.sync.ecss.extensions.commons.table.properties.[TableHelperConstants](TableHelperConstants.md)

    * ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesConstants](TablePropertiesConstants.md)

        * ro.sync.ecss.extensions.commons.table.properties.[TablePropertiesHelper](TablePropertiesHelper.md) (also extends ro.sync.ecss.extensions.commons.table.properties.[TableHelper](TableHelper.md))

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.ecss.extensions.commons.table.properties.[EditedTablePropertiesInfo.TAB_TYPE](EditedTablePropertiesInfo.TAB_TYPE.md)
        * ro.sync.ecss.extensions.commons.table.properties.[GuiElements](GuiElements.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
