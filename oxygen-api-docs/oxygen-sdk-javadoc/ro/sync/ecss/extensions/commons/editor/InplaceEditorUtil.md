Package [ro.sync.ecss.extensions.commons.editor](package-summary.md)

# Class InplaceEditorUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.editor.InplaceEditorUtil
   @API(type=INTERNAL, src=PUBLIC) public final class InplaceEditorUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility methods for preparing the in-place editors for being displayed.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static <T> T [addToParent](#addToParent(java.awt.Component,java.awt.Container,java.util.function.Supplier))([Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) component, [Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html) parent, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<T> supplier)
Adds the child inside the parent, calls the given supplier and requests the results from the supplier.
  static [Dimension](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dimension.html) [getPreferredSize](#getPreferredSize(java.awt.Component,java.awt.Container))([Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) component, [Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html) parent)
Get the preferred size for the component.
  static [Dimension](../../../../exml/view/graphics/Dimension.md) [getPreferredSize](#getPreferredSize(javax.swing.JComboBox,ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) comboBox, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
Computes the preferred size for the given combo box.
  static [Dimension](../../../../exml/view/graphics/Dimension.md) [getPreferredSize](#getPreferredSize(javax.swing.JPanel,ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) panel, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
Computes the preferred size for the panel.
  static [Dimension](../../../../exml/view/graphics/Dimension.md) [getPreferredSize](#getPreferredSize(javax.swing.JTextField,ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([JTextField](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextField.html) textField, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
Computes the preferred size for the given text field.
  static void [relayout](#relayout(javax.swing.JComboBox,ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) comboBox, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
Computes the required size for the editor and positions the caret at the end of the text.
  static void [relayout](#relayout(javax.swing.JTextField,ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([JTextField](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextField.html) textField, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
Computes the required size for the editor and positions the caret at the end of the text.
  static void [setCaretAtEnd](#setCaretAtEnd(javax.swing.text.JTextComponent,ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([JTextComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/JTextComponent.html) textField, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
Sets the caret at the end of the text from the text field.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### getPreferredSize

public static [Dimension](../../../../exml/view/graphics/Dimension.md) getPreferredSize([JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) panel, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)

Computes the preferred size for the panel.
  Parameters: panel - A panel used as an editor. context - In-place editing context. Returns: The preferred size for the given context.
### getPreferredSize

public static [Dimension](../../../../exml/view/graphics/Dimension.md) getPreferredSize([JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) comboBox, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)

Computes the preferred size for the given combo box.
  Parameters: comboBox - A combo box used as an editor. context - In-place editing context. Returns: The preferred size for the given context.
### getPreferredSize

public static [Dimension](../../../../exml/view/graphics/Dimension.md) getPreferredSize([JTextField](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextField.html) textField, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)

Computes the preferred size for the given text field.
  Parameters: textField - A text field used as an editor. context - In-place editing context. Returns: The preferred size for the given context.
### relayout

public static void relayout([JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) comboBox, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)

Computes the required size for the editor and positions the caret at the end of the text. The caret offset will also be scrolled to be visible.
  Parameters: comboBox - Combo box used for editing. context - In-place editing context.
### relayout

public static void relayout([JTextField](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextField.html) textField, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)

Computes the required size for the editor and positions the caret at the end of the text. The caret offset will also be scrolled to be visible.
  Parameters: textField - Text field used for editing. context - In-place editing context.
### setCaretAtEnd

public static void setCaretAtEnd([JTextComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/JTextComponent.html) textField, [AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)

Sets the caret at the end of the text from the text field.
  Parameters: textField - Text field to be scrolled. context - In-place editing context.
### getPreferredSize

public static [Dimension](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Dimension.html) getPreferredSize([Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) component, [Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html) parent)

Get the preferred size for the component.
  Parameters: component - The component. parent - The parent component, where the component will eventually be added. Returns: the baseline
### addToParent

public static <T> T addToParent([Component](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Component.html) component, [Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html) parent, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<T> supplier)

Adds the child inside the parent, calls the given supplier and requests the results from the supplier.
  Parameters: component - The component. parent - The parent component, where the component will eventually be added. supplier - To be invoked. Returns: The results from the given supplier, after the component is added inside the parent.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
