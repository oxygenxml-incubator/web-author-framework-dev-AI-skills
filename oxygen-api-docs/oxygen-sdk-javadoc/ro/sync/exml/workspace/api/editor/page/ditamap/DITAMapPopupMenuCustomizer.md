Package [ro.sync.exml.workspace.api.editor.page.ditamap](package-summary.md)

# Interface DITAMapPopupMenuCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface DITAMapPopupMenuCustomizer
Can be used to customize a pop-up menu before showing it.
  Since: 12.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorDocumentController))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorDocumentController](../../../../../../ecss/extensions/api/AuthorDocumentController.md) ditaMapDocumentController)
Customize a pop-up menu in the DITA Maps Manager page before showing it.

## Method Details

### customizePopUpMenu

void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorDocumentController](../../../../../../ecss/extensions/api/AuthorDocumentController.md) ditaMapDocumentController)

Customize a pop-up menu in the DITA Maps Manager page before showing it. If everything is removed then the menu will not be shown.For the standalone implementation the object is a *JPopupMenu*.
  Parameters: popUp - The pop-up Menu. ditaMapDocumentController - Access to modify the nodes in the DITA Map tree.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
