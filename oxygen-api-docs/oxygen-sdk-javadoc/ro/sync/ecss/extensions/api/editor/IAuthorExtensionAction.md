Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface IAuthorExtensionAction
    All Known Subinterfaces: [AuthorExtensionAskAction](AuthorExtensionAskAction.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface IAuthorExtensionAction
An author action created over an author operation. These actions are configured in the associated document type of the current document.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_ID](#ACTION_ID)
The ID of the action as specified when the action was configured in the framework.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_NAME](#ACTION_NAME)
The name of the action as specified when the action was configured in the framework.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DESCRIPTION](#DESCRIPTION)
A short description for the action.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LARGE_ICON_PATH](#LARGE_ICON_PATH)
The path for a large icon associated with the action.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SMALL_ICON_PATH](#SMALL_ICON_PATH)
The absolute path for a small icon associated with the action.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getValue](#getValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property)
Gets the value for the given property.
  void [performAction](#performAction())()
Perform the action.
  void [performAction](#performAction(int))(int imposedActionOffset)
Perform the action.

## Field Details

### ACTION_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_ID

The ID of the action as specified when the action was configured in the framework.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.IAuthorExtensionAction.ACTION_ID)

### ACTION_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_NAME

The name of the action as specified when the action was configured in the framework.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.IAuthorExtensionAction.ACTION_NAME)

### SMALL_ICON_PATH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SMALL_ICON_PATH

The absolute path for a small icon associated with the action. Can contain editor variables.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.IAuthorExtensionAction.SMALL_ICON_PATH)

### LARGE_ICON_PATH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LARGE_ICON_PATH

The path for a large icon associated with the action. can contain editor variables.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.IAuthorExtensionAction.LARGE_ICON_PATH)

### DESCRIPTION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DESCRIPTION

A short description for the action.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.IAuthorExtensionAction.DESCRIPTION)

## Method Details

### getValue

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property)

Gets the value for the given property.
  Parameters: property - The property to get the value. Returns: The value for the property.
### performAction

void performAction()

Perform the action.

### performAction

void performAction(int imposedActionOffset)

Perform the action.
  Parameters: imposedActionOffset - The imposed offset where the action should take place.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
