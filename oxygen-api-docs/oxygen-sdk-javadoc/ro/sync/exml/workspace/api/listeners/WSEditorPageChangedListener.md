Package [ro.sync.exml.workspace.api.listeners](package-summary.md)

# Class WSEditorPageChangedListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.listeners.WSEditorPageChangedListener
   Direct Known Subclasses: [WSEditorListener](WSEditorListener.md)   @API(type=EXTENDABLE, src=PUBLIC) public class WSEditorPageChangedListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
WS Editor page changed listener. Notified when an opened editor switches to another page.
  Since: 12
## Constructor Summary
 Constructors
Constructor

Description
 [WSEditorPageChangedListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [editorPageAboutToBeChangedVeto](#editorPageAboutToBeChangedVeto(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newPageID)
The current editing page (mode) is about to be changed.
  void [editorPageChanged](#editorPageChanged())()
The current page for an editor has changed

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WSEditorPageChangedListener

public WSEditorPageChangedListener()

## Method Details

### editorPageAboutToBeChangedVeto

public boolean editorPageAboutToBeChangedVeto([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newPageID)

The current editing page (mode) is about to be changed.
  Parameters: newPageID - The ID of the page to which the user switched, one of the constant fields: [EditorPageConstants.PAGE_TEXT](../../../editor/EditorPageConstants.md#PAGE_TEXT), [EditorPageConstants.PAGE_AUTHOR](../../../editor/EditorPageConstants.md#PAGE_AUTHOR), [EditorPageConstants.PAGE_GRID](../../../editor/EditorPageConstants.md#PAGE_GRID), [EditorPageConstants.PAGE_DESIGN](../../../editor/EditorPageConstants.md#PAGE_DESIGN), [EditorPageConstants.PAGE_DITA_MAP](../../../editor/EditorPageConstants.md#PAGE_DITA_MAP) Returns: true to continue switching to the page, false to cancel the switch operation. The switch operation cannot be vetoed in the Oxygen Plugin for Eclipse. Since: 16.1
### editorPageChanged

public void editorPageChanged()

The current page for an editor has changed

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
