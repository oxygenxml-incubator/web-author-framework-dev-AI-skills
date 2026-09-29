# Hierarchy For Package ro.sync.exml.workspace.api.standalone.ui
 Package Hierarchies:
* [All Packages](../../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.awt.[Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) (implements java.awt.image.[ImageObserver](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/ImageObserver.html), java.awt.[MenuContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/MenuContainer.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.awt.[Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html)

            * javax.swing.[JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
                * javax.swing.[AbstractButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/AbstractButton.html) (implements java.awt.[ItemSelectable](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/ItemSelectable.html), javax.swing.[SwingConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/SwingConstants.html))
                    * javax.swing.[JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))
                        * ro.sync.ui.application.ApplicationButton
                            * ro.sync.exml.workspace.api.standalone.ui.[Button](Button.md)
                            * ro.sync.exml.options.ColorButton

                                * ro.sync.exml.workspace.api.standalone.ui.[ColorButton](ColorButton.md)

                        * com.jidesoft.swing.JideButton (implements com.jidesoft.swing.Alignable, com.jidesoft.swing.AlignmentSupport, com.jidesoft.swing.ButtonStyle, com.jidesoft.swing.ComponentStateSupport)

                            * ro.sync.ui.application.ApplicationJideButton
                                * ro.sync.ui.toolbar.ToolBarButton

                                    * ro.sync.exml.workspace.api.standalone.ui.[ToolbarButton](ToolbarButton.md)

                            * com.jidesoft.swing.JideToggleButton (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))

                                * ro.sync.ui.toolbar.ToolbarToggleButton

                                    * ro.sync.exml.workspace.api.standalone.ui.[ToolbarToggleButton](ToolbarToggleButton.md)

                    * javax.swing.[JMenuItem](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenuItem.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[MenuElement](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/MenuElement.html))

                        * javax.swing.[JMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenu.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[MenuElement](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/MenuElement.html))

                            * com.jidesoft.swing.JideMenu (implements com.jidesoft.swing.Alignable)

                                * ro.sync.ui.application.menu.ApplicationMenu (implements ro.sync.ui.application.AutoMnemonicProvider, ro.sync.ui.application.menu.IApplicationMenu, ro.sync.ui.application.menu.IApplicationMenuItem, ro.sync.exml.editor.NeutralActionProvider, ro.sync.ui.application.menu.TaggedMenu)
                                    * ro.sync.exml.workspace.api.standalone.ui.[Menu](Menu.md)

                                * com.jidesoft.swing.JideSplitButton (implements com.jidesoft.swing.ButtonStyle, com.jidesoft.swing.ComponentStateSupport)

                                    * ro.sync.ui.ApplicationSplitButton

                                        * ro.sync.exml.workspace.api.standalone.ui.[SplitMenuButton](SplitMenuButton.md)

                * javax.swing.[JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[SwingConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/SwingConstants.html))
                    * javax.swing.tree.[DefaultTreeCellRenderer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/DefaultTreeCellRenderer.html) (implements javax.swing.tree.[TreeCellRenderer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreeCellRenderer.html))

                        * ro.sync.ui.application.ApplicationTreeCellRenderer (implements ro.sync.ui.application.ActiveTreeAwareCellRenderer, ro.sync.ui.application.ApplicationTreeConstants)

                            * ro.sync.exml.workspace.api.standalone.ui.[TreeCellRenderer](TreeCellRenderer.md)

                * javax.swing.[JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[MenuElement](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/MenuElement.html))
                    * ro.sync.ui.application.ApplicationPopupMenu (implements ro.sync.ui.application.menu.IApplicationMenu, ro.sync.ui.application.menu.TaggedMenu)

                        * ro.sync.exml.workspace.api.standalone.ui.[PopupMenu](PopupMenu.md)

                * javax.swing.[JTable](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTable.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.event.[CellEditorListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/CellEditorListener.html), javax.swing.event.[ListSelectionListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/ListSelectionListener.html), javax.swing.event.[RowSorterListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/RowSorterListener.html), javax.swing.[Scrollable](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Scrollable.html), javax.swing.event.[TableColumnModelListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/TableColumnModelListener.html), javax.swing.event.[TableModelListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/TableModelListener.html))
                    * ro.sync.ui.application.ApplicationTable

                        * ro.sync.exml.workspace.api.standalone.ui.[Table](Table.md)

                * javax.swing.text.[JTextComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/JTextComponent.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[Scrollable](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Scrollable.html))
                    * javax.swing.[JTextField](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextField.html) (implements javax.swing.[SwingConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/SwingConstants.html))

                        * ro.sync.ui.UndoableTextField

                            * ro.sync.ui.ApplicationTextField

                                * ro.sync.exml.workspace.api.standalone.ui.[TextField](TextField.md)

                * javax.swing.[JTree](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTree.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[Scrollable](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Scrollable.html))

                    * ro.sync.ui.application.ApplicationTree (implements ro.sync.ui.DefaultTreeScrollBehaviour)

                        * ro.sync.exml.workspace.api.standalone.ui.[Tree](Tree.md)

            * java.awt.[Window](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Window.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html))

                * java.awt.[Dialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dialog.html)

                    * javax.swing.[JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) (implements javax.accessibility.[Accessible](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/accessibility/Accessible.html), javax.swing.[RootPaneContainer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/RootPaneContainer.html), javax.swing.[WindowConstants](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/WindowConstants.html))

                        * ro.sync.exml.workspace.api.standalone.ui.[OKCancelDialog](OKCancelDialog.md) (implements ro.sync.ui.application.[HelpPageProvider](../../../../../ui/application/HelpPageProvider.md))

    * ro.sync.exml.workspace.api.standalone.ui.[OxygenUIComponentsFactory](OxygenUIComponentsFactory.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
