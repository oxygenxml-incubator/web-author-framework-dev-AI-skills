Package [ro.sync.ecss.extensions.api.structure](package-summary.md)

# Class AuthorOutlineCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.structure.AuthorOutlineCustomizer
   All Implemented Interfaces: [AuthorNodeRendererCustomizer](AuthorNodeRendererCustomizer.md), [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorOutlineCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorNodeRendererCustomizer](AuthorNodeRendererCustomizer.md), [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md)
Author Outline customizer used for custom filtering and nodes rendering in the Outline.
  Since: 11.2
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorOutlineCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [customizePopUpMenu](#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess)
Customize a pop-up menu in the Author page before showing it.
  void [customizeRenderingInformation](#customizeRenderingInformation(ro.sync.ecss.extensions.api.structure.RenderingInformation))([RenderingInformation](RenderingInformation.md) renderInfo)
If you need to change the way the XML elements are displayed, you may consider using a configuration file.
  boolean [ignoreNode](#ignoreNode(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../node/AuthorNode.md) node)
If true this node and all its descendants are not shown in the Outline.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorOutlineCustomizer

public AuthorOutlineCustomizer()

## Method Details

### ignoreNode

public boolean ignoreNode([AuthorNode](../node/AuthorNode.md) node)

If true this node and all its descendants are not shown in the Outline.
  Parameters: node - The node to check for ignore. Returns: True if the given node and its descendants will not be presented in the Outline.
### customizeRenderingInformation

public void customizeRenderingInformation([RenderingInformation](RenderingInformation.md) renderInfo)

If you need to change the way the XML elements are displayed, you may consider using a configuration file. For more information, search the oXygen documentation for "cc_config.xml" configuration file. For DITA, this file is in "frameworks/dita/resources/cc_config.xml".
  Specified by: [customizeRenderingInformation](AuthorNodeRendererCustomizer.md#customizeRenderingInformation(ro.sync.ecss.extensions.api.structure.RenderingInformation)) in interface [AuthorNodeRendererCustomizer](AuthorNodeRendererCustomizer.md) Parameters: renderInfo - The default information which will get displayed. You can set custom values for each field See Also:
        * [AuthorNodeRendererCustomizer.customizeRenderingInformation(ro.sync.ecss.extensions.api.structure.RenderingInformation)](AuthorNodeRendererCustomizer.md#customizeRenderingInformation(ro.sync.ecss.extensions.api.structure.RenderingInformation))

### customizePopUpMenu

public void customizePopUpMenu([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) popUp, [AuthorAccess](../AuthorAccess.md) authorAccess)
 Description copied from interface: [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess))
Customize a pop-up menu in the Author page before showing it. If everything is removed then the menu will not be shown.For the standalone implementation the object is a *JPopupMenu*.For the eclipse implementation the object is a *IMenuManager*.
  Specified by: [customizePopUpMenu](AuthorPopupMenuCustomizer.md#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess)) in interface [AuthorPopupMenuCustomizer](AuthorPopupMenuCustomizer.md) Parameters: popUp - The pop-up Menu. authorAccess - Access class to the author functions. See Also:
        * [AuthorPopupMenuCustomizer.customizePopUpMenu(java.lang.Object, ro.sync.ecss.extensions.api.AuthorAccess)](AuthorPopupMenuCustomizer.md#customizePopUpMenu(java.lang.Object,ro.sync.ecss.extensions.api.AuthorAccess))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
