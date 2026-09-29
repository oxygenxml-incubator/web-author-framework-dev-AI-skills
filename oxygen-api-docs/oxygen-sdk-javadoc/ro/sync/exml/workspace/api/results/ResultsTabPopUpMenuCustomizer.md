Package [ro.sync.exml.workspace.api.results](package-summary.md)

# Interface ResultsTabPopUpMenuCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface ResultsTabPopUpMenuCustomizer
Customizes the contextual pop-up menu of a results tab.
  Since: 19.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp)
Customize the pop-up menu shown in a results tab before showing it.

## Method Details

### customizePopUpMenu

void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp)

Customize the pop-up menu shown in a results tab before showing it. If everything is removed then the menu will not be shown.For the stand-alone implementation the object is a JPopupMenu.For the eclipse implementation the object is a IMenuManager.
  Parameters: popUp - The pop-up menu.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
