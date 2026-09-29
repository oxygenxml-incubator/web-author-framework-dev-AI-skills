# Hierarchy For Package ro.sync.ecss.extensions.commons.id
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

                                * ro.sync.ecss.extensions.commons.id.[SAIDElementsCustomizerDialog](SAIDElementsCustomizerDialog.md)

    * ro.sync.ecss.extensions.commons.id.[ConfigureAutoIDElementsOperation](ConfigureAutoIDElementsOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.commons.id.[DefaultUniqueAttributesRecognizer](DefaultUniqueAttributesRecognizer.md) (implements ro.sync.ecss.extensions.api.content.[ClipboardFragmentProcessor](../../api/content/ClipboardFragmentProcessor.md), ro.sync.ecss.extensions.api.[UniqueAttributesRecognizer](../../api/UniqueAttributesRecognizer.md))
    * ro.sync.ecss.extensions.commons.id.[ECIDElementsCustomizer](ECIDElementsCustomizer.md)
    * ro.sync.ecss.extensions.commons.id.[GenerateIDElementsInfo](GenerateIDElementsInfo.md)
    * ro.sync.ecss.extensions.commons.id.[GenerateIDsOperation](GenerateIDsOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.commons.id.[SAIDElementsCustomizer](SAIDElementsCustomizer.md)
    * org.eclipse.jface.window.Window (implements org.eclipse.jface.window.IShellProvider)

        * org.eclipse.jface.dialogs.Dialog

            * org.eclipse.jface.dialogs.TrayDialog

                * ro.sync.ecss.extensions.commons.id.[ECIDElementsCustomizerDialog](ECIDElementsCustomizerDialog.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
