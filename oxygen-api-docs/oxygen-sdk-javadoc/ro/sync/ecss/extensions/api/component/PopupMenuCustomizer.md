Package [ro.sync.ecss.extensions.api.component](package-summary.md)

# Interface PopupMenuCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface PopupMenuCustomizer
Can be used to customize a JPopupMenu before showing it.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customize](#customize(javax.swing.JPopupMenu))([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp)
Customize a pop-up menu in the Author page before showing it.

## Method Details

### customize

void customize([JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) popUp)

Customize a pop-up menu in the Author page before showing it. If everything is removed then the menu will not be shown.
  Parameters: popUp - The pop-up Menu.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
