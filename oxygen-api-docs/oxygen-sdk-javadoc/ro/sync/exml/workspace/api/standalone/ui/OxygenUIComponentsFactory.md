Package [ro.sync.exml.workspace.api.standalone.ui](package-summary.md)

# Class OxygenUIComponentsFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.ui.OxygenUIComponentsFactory
   @API(type=EXTENDABLE, src=PUBLIC) public final class OxygenUIComponentsFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Create UI components that look and feel like the ones in oXygen.
  Since: 21.1
## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static void [changeContentType](#changeContentType(javax.swing.JTextArea,java.lang.String))([JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) textArea, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Changes the content type of a text area created with Oxygen API [createTextArea(String)](#createTextArea(java.lang.String))
  static [JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) [createButton](#createButton(javax.swing.Action))([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)
Create a button.
  static [JCheckBoxMenuItem](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JCheckBoxMenuItem.html) [createCheckBoxMenuItem](#createCheckBoxMenuItem(javax.swing.Action))([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)
Create a checkbox menu item over given action.
  static [ColorButton](ColorButton.md) [createColorChooserButton](#createColorChooserButton(java.awt.Color))([Color](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html) currentColor)
Create a button that presents a color chooser.
  static [JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) [createComboBox](#createComboBox(javax.swing.ComboBoxModel))([ComboBoxModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/ComboBoxModel.html) model)
Create a new Oxygen style combo box.
  static [JEditorPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JEditorPane.html) [createHTMLEditorPane](#createHTMLEditorPane(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, boolean useStandardTextFont)
Creates a JEditorPane to edit HTML content.
  static [InputUrlComponentProvider](urlpanel/InputUrlComponentProvider.md) [createInputURLPanelProvider](#createInputURLPanelProvider(java.lang.String%5B%5D,java.lang.String,java.lang.String%5B%5D,boolean,java.lang.String,ro.sync.exml.workspace.api.standalone.ui.urlpanel.LocalFileBrowseType))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] extensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filesDescription, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] initialContent, boolean showEditorVariables, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) persistenceKey, [LocalFileBrowseType](urlpanel/LocalFileBrowseType.md) browseType)
Create the input url component provider, used to create an URL chooser similar to the ones in the application which can be embedded inside a third party panel.
  static [JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) [createLinkLabel](#createLinkLabel(java.lang.String,java.awt.event.ActionListener))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, [ActionListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionListener.html) listener)
Create a clickable label which looks like a link.
  static [Menu](Menu.md) [createMenu](#createMenu(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) menuName)
Create a javax.swing.JMenu extension that has the look and feel consistent with the menus from oXygen.
  static [JMenuItem](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenuItem.html) [createMenuItem](#createMenuItem(javax.swing.Action))([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)
Create a menu item over given action.
  static [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) [createMultilineLabel](#createMultilineLabel(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, boolean boldText)
Create a new multiline label.
  static [OKCancelDialog](OKCancelDialog.md) [createOkCancelDialog](#createOkCancelDialog(java.awt.Frame,java.lang.String,boolean))([Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, boolean modal)
Create a dialog with OK and Cancel buttons.
  static [PopupMenu](PopupMenu.md) [createPopupMenu](#createPopupMenu())()
Create a javax.swing.JPopupMenu extension that has the look and feel consistent with the pop-up menus from oXygen.
  static [JRadioButtonMenuItem](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JRadioButtonMenuItem.html) [createRadioMenuItem](#createRadioMenuItem(javax.swing.Action))([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)
Create a radio button menu item over given action.
  static [JScrollPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JScrollPane.html) [createScrollPane](#createScrollPane(java.awt.Component,int,int))([Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) view, int vsbPolicy, int hsbPolicy)
Creates a ScrollPane that displays a view component in a viewport whose view position can be controlled with a pair of scrollbars.
  static [SplitMenuButton](SplitMenuButton.md) [createSplitMenuButton](#createSplitMenuButton(java.lang.String,javax.swing.Icon,boolean,boolean,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultText, [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) defaultIcon, boolean updateText, boolean updateIcon, boolean alwaysShowMenu, boolean setSelectedActionAsDefault)
Create a split menu button.
  static [Table](Table.md) [createTable](#createTable(javax.swing.table.TableModel))([TableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/TableModel.html) tableModel)
Create a javax.swing.JTable extension that has the look and feel consistent with the tables from oXygen.
  static [JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) [createTextArea](#createTextArea(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Create a javax.swing.JTextArea extension with undo/redo support.
  static [JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) [createTextArea](#createTextArea(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, boolean highlightCurrentLine)
Create a javax.swing.JTextArea extension extension with undo/redo support.
  static [JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) [createTextArea](#createTextArea(java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, boolean highlightCurrentLine, boolean indentOnEnter)
Create a javax.swing.JTextArea extension extension with undo/redo support.
  static [TextField](TextField.md) [createTextField](#createTextField())()
Create a javax.swing.JTextField extension with undo/redo support.
  static [JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) [createToolbarButton](#createToolbarButton(javax.swing.Action,boolean))([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action, boolean showText)
Create a toolbar button.
  static [JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) [createToolbarToggleButton](#createToolbarToggleButton(javax.swing.Action,boolean))([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action, boolean showText)
Create a toolbar toggle button.
  static [Tree](Tree.md) [createTree](#createTree(javax.swing.tree.TreeModel))([TreeModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreeModel.html) model)
Create a javax.swing.JTree extension that has a look and feel consistent with the trees used in oXygen.
  static [JToolTip](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolTip.html) [installMultilineTooltip](#installMultilineTooltip(javax.swing.JComponent))([JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) component)
Installs a new multiline tooltip on a component.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### createButton

public static [JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) createButton([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)

Create a button.
  Parameters: action - The action associated with the button. Returns: the button.
### createColorChooserButton

public static [ColorButton](ColorButton.md) createColorChooserButton([Color](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Color.html) currentColor)

Create a button that presents a color chooser.
  Parameters: currentColor - The color to set as current/selected. Returns: The button.
### createMenu

public static [Menu](Menu.md) createMenu([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) menuName)

Create a javax.swing.JMenu extension that has the look and feel consistent with the menus from oXygen.
  Parameters: menuName - The menu's name. Returns: the menu.
### createOkCancelDialog

public static [OKCancelDialog](OKCancelDialog.md) createOkCancelDialog([Frame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Frame.html) parentFrame, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, boolean modal)

Create a dialog with OK and Cancel buttons.
  Parameters: parentFrame - The parent frame. Can be null, in which case it will be auto-detected. title - The dialog title. modal - true if modal. Returns: the dialog.
### createPopupMenu

public static [PopupMenu](PopupMenu.md) createPopupMenu()

Create a javax.swing.JPopupMenu extension that has the look and feel consistent with the pop-up menus from oXygen.
  Returns: the pop-up menu.
### createSplitMenuButton

public static [SplitMenuButton](SplitMenuButton.md) createSplitMenuButton([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultText, [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) defaultIcon, boolean updateText, boolean updateIcon, boolean alwaysShowMenu, boolean setSelectedActionAsDefault)

Create a split menu button. This a component representing a combination of a button and a menu. There is a line in the component that splits it into the two aforementioned sub-components. The part before the line is a button, and can be clicked in order to trigger an action. The part after the line is a menu.
  Parameters: defaultText - The default text, used when there is no action set explicitly. Can be null. defaultIcon - The default icon, used when there is no action set explicitly. Can be null. updateText - true to update the text of the button when selecting an action. updateIcon - true to update the icon of the button when selecting an action. alwaysShowMenu - true if pressing the button should always display the associated menu. setSelectedActionAsDefault - true to promote the selected action, setting it as the current/default action of the button. Returns: the button.
### createTable

public static [Table](Table.md) createTable([TableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/TableModel.html) tableModel)

Create a javax.swing.JTable extension that has the look and feel consistent with the tables from oXygen.
  Parameters: tableModel - The table's model. Returns: the table.
### createTextField

public static [TextField](TextField.md) createTextField()

Create a javax.swing.JTextField extension with undo/redo support. It also has an "edit" contextual menu (Cut, Copy, Paste, etc.).
  Returns: the text field.
### createToolbarButton

public static [JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) createToolbarButton([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action, boolean showText)

Create a toolbar button.
  Parameters: action - The action to execute. showText - true to show the text set for the action. Returns: the button.
### createToolbarToggleButton

public static [JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) createToolbarToggleButton([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action, boolean showText)

Create a toolbar toggle button.
  Parameters: action - The action to execute. showText - true to show the text set for the action. Returns: the button.
### createTree

public static [Tree](Tree.md) createTree([TreeModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreeModel.html) model)

Create a javax.swing.JTree extension that has a look and feel consistent with the trees used in oXygen. It uses a [TreeCellRenderer](TreeCellRenderer.md) by default.
  Parameters: model - The model of the tree. Returns: the tree.
### createMenuItem

public static [JMenuItem](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenuItem.html) createMenuItem([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)

Create a menu item over given action.
  Parameters: action - The action to execute. Returns: the menu item.
### installMultilineTooltip

public static [JToolTip](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolTip.html) installMultilineTooltip([JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) component)

Installs a new multiline tooltip on a component. In order to install the multiline tooltip you have to override the javax.swing.JComponent.createToolTip() method of the component and return the result of the current method.
  Parameters: component - The component to install the tooltip on. Returns: The new tooltip component. Since: 22
### createMultilineLabel

public static [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) createMultilineLabel([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, boolean boldText)

Create a new multiline label.
  Parameters: text - The content of the multiline component. boldText - true if the content must be bold, false otherwise. Returns: A label which will present the given content on multiple lines. Since: 22.1
### createComboBox

public static [JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) createComboBox([ComboBoxModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/ComboBoxModel.html) model)

Create a new Oxygen style combo box.
  Parameters: model - The model of the combo box. Returns: An Oxygen style combo box. Since: 23
### createInputURLPanelProvider

public static [InputUrlComponentProvider](urlpanel/InputUrlComponentProvider.md) createInputURLPanelProvider([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] extensions, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) filesDescription, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] initialContent, boolean showEditorVariables, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) persistenceKey, [LocalFileBrowseType](urlpanel/LocalFileBrowseType.md) browseType)

Create the input url component provider, used to create an URL chooser similar to the ones in the application which can be embedded inside a third party panel.
  Parameters: extensions - Files having this extension will be shown in the file system browser. filesDescription - The file description associated with the extension. initialContent - The initial content of the combo box from the url chooser. showEditorVariables - true for showing the Editor Variables chooser button. false otherwise. persistenceKey - The key that will be used to save entries from this URL panel as persistent between sessions. Null to inhibit persistence. browseType - The browse mode for local file browsing: Open file, Save file or Open directory. Returns: The input url component provider which can be used to interact with the component. Since: 23
### createScrollPane

public static [JScrollPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JScrollPane.html) createScrollPane([Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) view, int vsbPolicy, int hsbPolicy)

Creates a ScrollPane that displays a view component in a viewport whose view position can be controlled with a pair of scrollbars. The scrollbar policies specify when the scrollbars are displayed.
  Parameters: view - The component to display in the viewport. vsbPolicy - Determines when the vertical scrollbar appears in the scrollpane. The possible values are:
        * ScrollPaneConstants.VERTICAL_SCROLLBAR_AS_NEEDED
        * ScrollPaneConstants.VERTICAL_SCROLLBAR_NEVER
        * ScrollPaneConstants.VERTICAL_SCROLLBAR_ALWAYS
 hsbPolicy - Determines when the horizontal scrollbar appears in the scrollpane. The possible values are:
        * ScrollPaneConstants.HORIZONTAL_SCROLLBAR_AS_NEEDED
        * ScrollPaneConstants.HORIZONTAL_SCROLLBAR_NEVER
        * ScrollPaneConstants.HORIZONTAL_SCROLLBAR_ALWAYS
 Returns: The scroll pane. Since: 24
### createHTMLEditorPane

public static [JEditorPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JEditorPane.html) createHTMLEditorPane([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, boolean useStandardTextFont)

Creates a JEditorPane to edit HTML content.
  Parameters: text - the text to initialize the Editor useStandardTextFont - true if the Editor should use the same font as a standard JTextArea. Returns: The JEditorPane Since: 25.0
### createTextArea

public static [JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) createTextArea([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

Create a javax.swing.JTextArea extension with undo/redo support. It also has an "edit" contextual menu (Cut, Copy, Paste, etc.). The current line in the text area is highlighted.
  Parameters: contentType - The content type used for color syntax highlight. The content types are available in ro.sync.basic.contenttypes.ContentTypes. If null, the plain text content type will be used. Returns: the text area. Since: 25.0
### createTextArea

public static [JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) createTextArea([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, boolean highlightCurrentLine)

Create a javax.swing.JTextArea extension extension with undo/redo support. It also has an "edit" contextual menu (Cut, Copy, Paste, etc.).
  Parameters: contentType - The content type used for color syntax highlight. The content types are available in ro.sync.basic.contenttypes.ContentTypes. If null, the plain text content type will be used. highlightCurrentLine - true to highlight the current line Returns: the text area. Since: 26.1
### createTextArea

public static [JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) createTextArea([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType, boolean highlightCurrentLine, boolean indentOnEnter)

Create a javax.swing.JTextArea extension extension with undo/redo support. It also has an "edit" contextual menu (Cut, Copy, Paste, etc.).
  Parameters: contentType - The content type used for color syntax highlight. The content types are available in ro.sync.basic.contenttypes.ContentTypes. If null, the plain text content type will be used. highlightCurrentLine - true to highlight the current line indentOnEnter - true to indent on enter. Returns: the text area. Since: 28.0  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

### changeContentType

public static void changeContentType([JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) textArea, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

Changes the content type of a text area created with Oxygen API [createTextArea(String)](#createTextArea(java.lang.String))
  Parameters: textArea - The text area to change the content type. The text area should be an Oxygen API text area contentType - The content type used for color syntax highlight. The content types are available in ro.sync.basic.contenttypes.ContentTypes. If null, the plain text content type will be used. Since: 25.0
### createCheckBoxMenuItem

public static [JCheckBoxMenuItem](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JCheckBoxMenuItem.html) createCheckBoxMenuItem([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)

Create a checkbox menu item over given action.
  Parameters: action - The action to execute. Returns: the checkbox menu item. Since: 27
### createRadioMenuItem

public static [JRadioButtonMenuItem](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JRadioButtonMenuItem.html) createRadioMenuItem([Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) action)

Create a radio button menu item over given action.
  Parameters: action - The action to execute. Returns: the radio button menu item. Since: 27
### createLinkLabel

public static [JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) createLinkLabel([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) text, [ActionListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionListener.html) listener)

Create a clickable label which looks like a link. The label renders the specified text and calls the specified action listener when the label is clicked.
  Parameters: text - The specified text to render on the link label. listener - The action listener that is called when the label is clicked. Never null. Returns: the link label. Since: 27.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
