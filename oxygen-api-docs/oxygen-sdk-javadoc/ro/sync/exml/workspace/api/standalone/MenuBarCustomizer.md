Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface MenuBarCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface MenuBarCustomizer
Customizes components from the main menu bar.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizeMainMenu](#customizeMainMenu(javax.swing.JMenuBar))([JMenuBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenuBar.html) mainMenu)
Customize the components which get displayed on the main menu bar.

## Method Details

### customizeMainMenu

void customizeMainMenu([JMenuBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JMenuBar.html) mainMenu)

Customize the components which get displayed on the main menu bar. This callback may be received multiple times during the editing session and you need to avoid adding your actions multiple times, check if they have already been added and if they have avoid adding them again to the menu.
  Parameters: mainMenu - The main menu bar.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
