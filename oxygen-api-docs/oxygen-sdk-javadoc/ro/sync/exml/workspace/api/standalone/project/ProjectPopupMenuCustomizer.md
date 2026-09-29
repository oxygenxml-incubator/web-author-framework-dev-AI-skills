Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Interface ProjectPopupMenuCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface ProjectPopupMenuCustomizer
Can be used to customize a pop-up menu before showing it.
  Since: 19.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp)
Customize a pop-up menu in the Project view.

## Method Details

### customizePopUpMenu

void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp)

Customize a pop-up menu in the Project view. If everything is removed then the menu will not be shown.For the standalone implementation the object is a *JPopupMenu*.
  Parameters: popUp - The pop-up Menu.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
