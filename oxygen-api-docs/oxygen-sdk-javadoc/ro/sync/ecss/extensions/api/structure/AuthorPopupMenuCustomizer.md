Package [ro.sync.ecss.extensions.api.structure](package-summary.md)

# Interface AuthorPopupMenuCustomizer
    All Known Implementing Classes: [AuthorBreadCrumbCustomizer](AuthorBreadCrumbCustomizer.md), [AuthorOutlineCustomizer](AuthorOutlineCustomizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorPopupMenuCustomizer
Can be used to customize a pop-up menu before showing it.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess)
Customize a pop-up menu in the Author page before showing it.

## Method Details

### customizePopUpMenu

void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess)

Customize a pop-up menu in the Author page before showing it. If everything is removed then the menu will not be shown.For the standalone implementation the object is a *JPopupMenu*.For the eclipse implementation the object is a *IMenuManager*.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
