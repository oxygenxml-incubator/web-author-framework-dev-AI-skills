Package [ro.sync.exml.workspace.api.editor.page.text](package-summary.md)

# Class TextPopupMenuCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.text.TextPopupMenuCustomizer
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class TextPopupMenuCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Can be used to customize a pop-up menu before showing it.
  Since: 14.1
## Constructor Summary
 Constructors
Constructor

Description
 [TextPopupMenuCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object,ro.sync.exml.workspace.api.editor.page.text.WSTextEditorPage))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [WSTextEditorPage](WSTextEditorPage.md) textPage)
Customize a pop-up menu in the Text page before showing it.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TextPopupMenuCustomizer

public TextPopupMenuCustomizer()

## Method Details

### customizePopUpMenu

public abstract void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [WSTextEditorPage](WSTextEditorPage.md) textPage)

Customize a pop-up menu in the Text page before showing it. If everything is removed then the menu will not be shown.For the standalone implementation the object is a *JPopupMenu*.For the eclipse implementation the object is a *IMenuManager*.
  Parameters: popUp - The pop-up Menu. textPage - The page over which the pop-up will be presented.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
