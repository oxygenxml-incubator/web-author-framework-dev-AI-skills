Package [ro.sync.ecss.extensions.api.structure](package-summary.md)

# Class AuthorBreadCrumbCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.structure.AuthorBreadCrumbCustomizer
   All Implemented Interfaces: [AuthorNodeRendererCustomizer](AuthorNodeRendererCustomizer.md), [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorBreadCrumbCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorNodeRendererCustomizer](AuthorNodeRendererCustomizer.md), [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md)
Author Bread Crumb (components path which appears in the top of the Author editor) customizer used for nodes rendering and pop-up customization.
  Since: 11.2
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorBreadCrumbCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess)
Customize a pop-up menu in the Author page before showing it.
  void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorNode](../node/AuthorNode.md) clickedNode)
Customize a pop-up menu in the Author page before showing it.
  void [customizeRenderingInformation](#customizeRenderingInformation(ro.sync.ecss.extensions.api.structure.RenderingInformation))([RenderingInformation](RenderingInformation.md) renderInfo)
Customize the tooltip, text and additional info to be presented in the Outline and Breadcrumb for the given node.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorBreadCrumbCustomizer

public AuthorBreadCrumbCustomizer()

## Method Details

### customizeRenderingInformation

public void customizeRenderingInformation([RenderingInformation](RenderingInformation.md) renderInfo)

Customize the tooltip, text and additional info to be presented in the Outline and Breadcrumb for the given node. The breadcrumb cannot assign a certain icon for a rendered node. By default a node is represented in the Outline by its tag name and a additional information obtained from a specific attribute or text. You can set custom values for each rendered field. If you need to change the way the XML elements are displayed, you may consider using a configuration file. For more information, search the oXygen documentation for "cc_config.xml" configuration file. For DITA, this file is in "frameworks/dita/resources/cc_config.xml".
  Specified by: [customizeRenderingInformation](AuthorNodeRendererCustomizer.md#customizeRenderingInformation(ro.sync.ecss.extensions.api.structure.RenderingInformation)) in interface [AuthorNodeRendererCustomizer](AuthorNodeRendererCustomizer.md) Parameters: renderInfo - The default information which will get displayed. You can set custom values for each field
### customizePopUpMenu

public void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess))
Customize a pop-up menu in the Author page before showing it. If everything is removed then the menu will not be shown.For the standalone implementation the object is a *JPopupMenu*.For the eclipse implementation the object is a *IMenuManager*.
  Specified by: [customizePopUpMenu](AuthorPopupMenuCustomizer.md#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md) Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. See Also:
        * [AuthorPopupMenuCustomizer.customizePopUpMenu(java.lang.Object, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorPopupMenuCustomizer.md#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess))

### customizePopUpMenu

public void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess, [AuthorNode](../node/AuthorNode.md) clickedNode)

Customize a pop-up menu in the Author page before showing it. If everything is removed then the menu will not be shown.For the standalone implementation the object is a *JPopupMenu*.For the eclipse implementation the object is a *IMenuManager*.
  Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. clickedNode - The current clicked node in the Author page. Since: 14.2
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
