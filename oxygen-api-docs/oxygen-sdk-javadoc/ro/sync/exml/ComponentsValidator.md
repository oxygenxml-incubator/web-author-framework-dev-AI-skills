Package [ro.sync.exml](package-summary.md)

# Class ComponentsValidator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.ComponentsValidator
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ComponentsValidator extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Validator interface for menus, toolbars and their actions.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SEP](#SEP)
Separator for menus and actions.

## Constructor Summary
 Constructors
Constructor

Description
 [ComponentsValidator](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [canonicalize](#canonicalize(java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] path)
Get a path from all the tags.
  abstract boolean [isDebuggerPerspectiveAllowed](#isDebuggerPerspectiveAllowed())()
Check if the debugger perspective is allowed in the current distribution.
  boolean [isMasterFilesSupportAvailable](#isMasterFilesSupportAvailable())()
Return true if main files support is available or not.
  boolean [isPerspectiveAllowed](#isPerspectiveAllowed(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) perspID)
Check if the perspective with the given ID is allowed.
  abstract boolean [validateAccelAction](#validateAccelAction(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) category, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tag)
Check if the given accel action is allowed.
  abstract boolean [validateComponent](#validateComponent(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Check if the given component is allowed.
  abstract boolean [validateContentType](#validateContentType(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Validate the given content type.
  boolean [validateEditorPage](#validateEditorPage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageID)
Check if the page is available for a certain distribution
  abstract boolean [validateLibrary](#validateLibrary(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) library)
Validate the given library.
  abstract boolean [validateMenuOrTaggedAction](#validateMenuOrTaggedAction(java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] menuOrActionPath)
Check if an menu or a tag action from a menu is allowed.
  abstract boolean [validateNewEditorTemplate](#validateNewEditorTemplate(ro.sync.exml.editor.EditorTemplate))([EditorTemplate](editor/EditorTemplate.md) editorTemplate)
Validate the given template for a new editor in the current distribution.
  abstract boolean [validateOption](#validateOption(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey)
Validate the given option.
  abstract boolean [validateOptionPane](#validateOptionPane(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionPaneKey)
Validate the given option pane.
  boolean [validateScenario](#validateScenario(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scenarioType)
Validate scenario type for the current distribution.
  abstract boolean [validateSHMarker](#validateSHMarker(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) marker)
Check if this marker is allowed in the current distribution.
  boolean [validateToolbarComposite](#validateToolbarComposite(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarCompositeTag)
Checks if the toolbar composite is available.
  abstract boolean [validateToolbarTaggedAction](#validateToolbarTaggedAction(java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] toolbarOrAction)
Check if an action from a toolbar is allowed.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### SEP

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SEP

Separator for menus and actions.
  See Also:
        * [Constant Field Values](../../../constant-values.md#ro.sync.exml.ComponentsValidator.SEP)

## Constructor Details

### ComponentsValidator

public ComponentsValidator()

## Method Details

### validateMenuOrTaggedAction

public abstract boolean validateMenuOrTaggedAction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] menuOrActionPath)

Check if an menu or a tag action from a menu is allowed.
  Parameters: menuOrActionPath - The tag of the menu/action and the tags of its parent menus if any. The last component is the current one. A menu path is an array of [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)s representing the Tags, ending with the current menu tag, or null. Returns: true if the action is allowed.
### validateToolbarTaggedAction

public abstract boolean validateToolbarTaggedAction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] toolbarOrAction)

Check if an action from a toolbar is allowed.
  Parameters: toolbarOrAction - The tag of the action from a toolbar and the tag of its parent toolbar if any. Returns: true if the action is allowed.
### validateToolbarComposite

public boolean validateToolbarComposite([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toolbarCompositeTag)

Checks if the toolbar composite is available. A toolbar composite is a toolbar component such as a drop-down list.
  Parameters: toolbarCompositeTag - The tag of the toolbar composite. Returns: true if the toolbar composite is allowed. Since: 17
### validateComponent

public abstract boolean validateComponent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Check if the given component is allowed.
  Parameters: key - Tag identifying the view. Usually one of the constants from MainFrameComponentProvider Returns: true if the view is allowed.
### validateAccelAction

public abstract boolean validateAccelAction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) category, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tag)

Check if the given accel action is allowed. An accel action can be uniquely identified so it doesn't matter if it is from a toolbar or menu.
  Parameters: category - The category of the action. tag - The tag of the action. Returns: true if the action is allowed.
### validateContentType

public abstract boolean validateContentType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

Validate the given content type.
  Parameters: contentType - The content type. A constant from ContentTypes interface. Returns: true if in the current distribution we support the given content type.
### validateOptionPane

public abstract boolean validateOptionPane([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionPaneKey)

Validate the given option pane.
  Parameters: optionPaneKey - The option pane key. A constant defined in OptionTags. Returns: true if in the current distribution we should add the given option pane in the option tree.
### validateOption

public abstract boolean validateOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey)

Validate the given option.
  Parameters: optionKey - The option key. A constant defined in OptionTags. Returns: true if in the current distribution we should add the given option in the option page.
### validateLibrary

public abstract boolean validateLibrary([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) library)

Validate the given library.
  Parameters: library - The library. Returns: true if in the current distribution we should add the given library in the about dialog.
### validateNewEditorTemplate

public abstract boolean validateNewEditorTemplate([EditorTemplate](editor/EditorTemplate.md) editorTemplate)

Validate the given template for a new editor in the current distribution.
  Parameters: editorTemplate - The editor template. Returns: true if it is allowed.
### isDebuggerPerspectiveAllowed

public abstract boolean isDebuggerPerspectiveAllowed()

Check if the debugger perspective is allowed in the current distribution. Also see [isPerspectiveAllowed(String)](#isPerspectiveAllowed(java.lang.String)).
  Returns: true if the debugger functionality is allowed.
### isPerspectiveAllowed

public boolean isPerspectiveAllowed([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) perspID)

Check if the perspective with the given ID is allowed. Also see [isDebuggerPerspectiveAllowed()](#isDebuggerPerspectiveAllowed()).
  Parameters: perspID - Perspective ID. See the constants from [UIPerspectives](UIPerspectives.md). Returns: true if the perspective is allowed. Since: 22
### validateSHMarker

public abstract boolean validateSHMarker([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) marker)

Check if this marker is allowed in the current distribution.
  Parameters: marker - The marker to be checked. A constant from SHMarker class. Returns: true if the marker is allowed.
### validateEditorPage

public boolean validateEditorPage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageID)

Check if the page is available for a certain distribution
  Parameters: pageID - The page ID Returns: true if the editor page is available. Since: 16
### canonicalize

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) canonicalize([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] path)

Get a path from all the tags.
  Parameters: path - The tags for the action/menu/toolbar and its menu/toolbar ancestors. Returns: A path that can be used to identify it.
### isMasterFilesSupportAvailable

public boolean isMasterFilesSupportAvailable()

Return true if main files support is available or not.
  Returns: Return true if main files support is available or not.
### validateScenario

public boolean validateScenario([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) scenarioType)

Validate scenario type for the current distribution.
  Parameters: scenarioType - The scenario type. Returns: true if the scenario is allowed, false otherwise. Since: 26.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
