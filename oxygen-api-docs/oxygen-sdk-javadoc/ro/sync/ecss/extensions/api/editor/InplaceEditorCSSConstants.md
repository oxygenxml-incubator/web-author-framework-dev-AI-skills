Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface InplaceEditorCSSConstants
    All Known Subinterfaces: [InplaceEditorArgumentKeys](InplaceEditorArgumentKeys.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface InplaceEditorCSSConstants
Arguments of the oxy_editor function as well as built-in values for some of these arguments.
  Since: 14.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_CONTEXT_CARET](#ACTION_CONTEXT_CARET)
Possible value for [PROPERTY_ACTION_CONTEXT](#PROPERTY_ACTION_CONTEXT).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_CONTEXT_ELEMENT](#ACTION_CONTEXT_ELEMENT)
Possible value for [PROPERTY_ACTION_CONTEXT](#PROPERTY_ACTION_CONTEXT).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [COMMA](#COMMA)
The variable used to add a comma in property values.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDIT_CUSTOM](#EDIT_CUSTOM)
Value of the PROPERTY_EDIT that indicates that the editor is doing a custom edit session and it's up to the editor to update the document.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDIT_TEXT_CONTENT](#EDIT_TEXT_CONTENT)
Value of the PROPERTY_EDIT that indicates that the text content of the element must be edited.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDIT_XML_CONTENT](#EDIT_XML_CONTENT)
Handled only for a text area editor [TYPE_TEXT_AREA](#TYPE_TEXT_AREA).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FALSE](#FALSE)
Possible value for PROPERTY_EDITABLE that marks the combo as NOT being editable.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [INHERIT](#INHERIT)
Value constant used for the color property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ACTION](#PROPERTY_ACTION)
Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and represents the action that must be invoked when the button is pressed.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ACTION_CONTEXT](#PROPERTY_ACTION_CONTEXT)
Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ACTION_DISPLAY_STYLE](#PROPERTY_ACTION_DISPLAY_STYLE)
Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and specifies what to display for an action: icon, text or both.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ACTION_ID](#PROPERTY_ACTION_ID)
Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and represents the ID of the action that must be invoked when the button is pressed.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ACTION_IDS](#PROPERTY_ACTION_IDS)
Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and contains a list of comma separated IDs of the actions that are presented to the user in a pop-up menu.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ACTIONS](#PROPERTY_ACTIONS)
Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and represents the list of the actions that can be invoked.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_CAN_REMOVE_VALUE](#PROPERTY_CAN_REMOVE_VALUE)
Property used for a non-editable combo box form control.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_CLASSPATH](#PROPERTY_CLASSPATH)
If the form control is a custom implementation this property can be used to specify the class path where the custom implementation will loaded from.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_COLOR](#PROPERTY_COLOR)
Property used to specify the foreground color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_COLUMNS](#PROPERTY_COLUMNS)
The number of columns that the editor should have.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_CONTENT_TYPE](#PROPERTY_CONTENT_TYPE)
Property used to specify the content type of the edited string.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME](#PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME)
Heavy weight form controls extension point.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_EDIT](#PROPERTY_EDIT)  Deprecated.
Use [InplaceEditorArgumentKeys.PROPERTY_EDIT_QUALIFIED](InplaceEditorArgumentKeys.md#PROPERTY_EDIT_QUALIFIED) instead.
   static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_EDITABLE](#PROPERTY_EDITABLE)
Only applies when the editor is a combo box and marks the combo as being editable or not.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_EDITOR_SORT](#PROPERTY_EDITOR_SORT)
Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION) and [PROPERTY_SELECTION_MODE](#PROPERTY_SELECTION_MODE) is set to [SELECTION_MODE_MULTIPLE](#SELECTION_MODE_MULTIPLE).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ENABLE_IN_READ_ONLY_CONTEXT](#PROPERTY_ENABLE_IN_READ_ONLY_CONTEXT)
Controls whether the button is enabled/disabled in read-only context.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_FILE_FILTER](#PROPERTY_FILE_FILTER)
A set of file extensions specifying the file types that should be shown in the dialog displayed by a URL chooser.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_FONT_INHERIT](#PROPERTY_FONT_INHERIT)
Property used to specify that the font is inherited from the parent element.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_FORMAT](#PROPERTY_FORMAT)
It applies only on date picker form control.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_HAS_MULTIPLE_VALUES](#PROPERTY_HAS_MULTIPLE_VALUES)
Property that can be set on a text field form control.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_HEIGHT](#PROPERTY_HEIGHT)
Imposes a height for a [TYPE_VIDEO_PLAYER](#TYPE_VIDEO_PLAYER) and [TYPE_BROWSER](#TYPE_BROWSER).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_HREF](#PROPERTY_HREF)
The location of a file.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_HTML_EMBEDDED_CONTENT](#PROPERTY_HTML_EMBEDDED_CONTENT)
For an "oxy_html_content" function, this is the HTML content to render given embedded in the CSS.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ICON](#PROPERTY_ICON)
Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and specifies the path to an Icon to be displayed on the button.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ID](#PROPERTY_ID)
The ID of an HTML element from the file specified by the "href" argument of "oxy_html_content".
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_INDENT_ON_TAB](#PROPERTY_INDENT_ON_TAB)
Controls the TAB behavior in the text area form control.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_LABEL](#PROPERTY_LABEL)
Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and specifies the label of the button that triggers the pop-up menu.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_LABELS](#PROPERTY_LABELS)
A set of labels to be associated with PROPERTY_VALUES.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ON_CHANGE](#PROPERTY_ON_CHANGE)
Combo box property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ON_HOVER_PSEUDO_CLASS_NAME](#PROPERTY_ON_HOVER_PSEUDO_CLASS_NAME)
Common property for all form controls.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_RENDERER_CLASS_NAME](#PROPERTY_RENDERER_CLASS_NAME)
Class name of the renderer.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_RENDERER_SEPARATOR](#PROPERTY_RENDERER_SEPARATOR)
Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_RENDERER_SORT](#PROPERTY_RENDERER_SORT)
Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_ROWS](#PROPERTY_ROWS)
The number of rows that the editor should have.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME](#PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME)
Heavy weight form controls extension point.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SELECTION_MODE](#PROPERTY_SELECTION_MODE)
Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SEPARATOR](#PROPERTY_SEPARATOR)
Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_CHECKBOX](#TYPE_CHECKBOX) or [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SHOW_ICON](#PROPERTY_SHOW_ICON)
Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and specifies if the icon should be displayed on the button.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SHOW_TEXT](#PROPERTY_SHOW_TEXT)
Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and specifies if the text should be displayed on the button.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SORT](#PROPERTY_SORT)
Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION)and [PROPERTY_SELECTION_MODE](#PROPERTY_SELECTION_MODE) is set to [SELECTION_MODE_MULTIPLE](#SELECTION_MODE_MULTIPLE).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SPELL_CHECK](#PROPERTY_SPELL_CHECK)
Only applies to text fields, text areas and editable combo boxes. The accepted values are true and false.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SWING_EDITOR_CLASS_NAME](#PROPERTY_SWING_EDITOR_CLASS_NAME)
Class name of the editor.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_SWT_EDITOR_CLASS_NAME](#PROPERTY_SWT_EDITOR_CLASS_NAME)
Class name of the editor.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_TOOLTIP](#PROPERTY_TOOLTIP)
Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and [TYPE_TEXT](#TYPE_TEXT) and specifies the tooltip for the button that triggers the pop-up menu with the actions in the group.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_TOOLTIPS](#PROPERTY_TOOLTIPS)
A set of tooltips to be associated with PROPERTY_VALUES.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_TRANSPARENT](#PROPERTY_TRANSPARENT)
Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and ensures whether the button will have a more flat appearance (transparent).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_TYPE](#PROPERTY_TYPE)
Indicates the editor that should be used to edit.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_UNCHECKED_VALUES](#PROPERTY_UNCHECKED_VALUES)
Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_CHECKBOX](#TYPE_CHECKBOX).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_VALIDATE_INPUT](#PROPERTY_VALIDATE_INPUT)
Controls the validation of the input.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_VALUES](#PROPERTY_VALUES)
A set of values to be presented as choices.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_VISIBLE](#PROPERTY_VISIBLE)
Property used to specify if an in-place editor is visible.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_WEBAPP_RENDERER_CLASS_NAME](#PROPERTY_WEBAPP_RENDERER_CLASS_NAME)
Class name of the server-side renderer used in the Author Webapp.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_WIDTH](#PROPERTY_WIDTH)
Imposes a width for the form control.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SELECTION_MODE_MULTIPLE](#SELECTION_MODE_MULTIPLE)
Possible value for ["selectionMode"](#PROPERTY_SELECTION_MODE).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SELECTION_MODE_SINGLE](#SELECTION_MODE_SINGLE)
Possible value for ["selectionMode"](#PROPERTY_SELECTION_MODE).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SORT_ASCENDING](#SORT_ASCENDING)
Value Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SORT_DESCENDING](#SORT_DESCENDING)
Value Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TRUE](#TRUE)
Possible value for PROPERTY_EDITABLE that marks the combo as being editable.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_AUDIO_PLAYER](#TYPE_AUDIO_PLAYER)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_BROWSER](#TYPE_BROWSER)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_BUTTON](#TYPE_BUTTON)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_CHECKBOX](#TYPE_CHECKBOX)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_COMBOBOX](#TYPE_COMBOBOX)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_DATE_PICKER](#TYPE_DATE_PICKER)
An editor that can be used to edit dates.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_HTML_CONTENT](#TYPE_HTML_CONTENT)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_OLD_URL_CHOOSER](#TYPE_OLD_URL_CHOOSER)
The old url chooser.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION)
The renderer presents a simple or compose value and the editor shows a pop-up like panel in which we can choose the values.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_TEXT](#TYPE_TEXT)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_TEXT_AREA](#TYPE_TEXT_AREA)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_URL_CHOOSER](#TYPE_URL_CHOOSER)
Possible value for PROPERTY_TYPE.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TYPE_VIDEO_PLAYER](#TYPE_VIDEO_PLAYER)
Possible value for PROPERTY_TYPE.

## Field Details

### PROPERTY_ON_HOVER_PSEUDO_CLASS_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ON_HOVER_PSEUDO_CLASS_NAME

Common property for all form controls. If such a class is given, when the cursor is hovering a form control this class will be set on the element on which the form control is added. When the cursor leaves the form control this class is removed. As a result you can have CSS rules that change the rendering of the element when it is hovered.
```


body:after {
    content:
        oxy_button(
            hoverPseudoclassName, "activeElement",
            actionID, 'action.id');
}

body {
    border:1px solid white;
}

body:activeElement {
    border:1px solid red;
}

```

  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ON_HOVER_PSEUDO_CLASS_NAME)

### PROPERTY_HTML_EMBEDDED_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_HTML_EMBEDDED_CONTENT

For an "oxy_html_content" function, this is the HTML content to render given embedded in the CSS.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_HTML_EMBEDDED_CONTENT)

### PROPERTY_HREF

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_HREF

The location of a file.
Used by [TYPE_HTML_CONTENT](#TYPE_HTML_CONTENT) to specify where is stored the content to be inserted by an "oxy_html_content" function.

Used by [TYPE_VIDEO_PLAYER](#TYPE_VIDEO_PLAYER) and [TYPE_BROWSER](#TYPE_BROWSER) to specify the location of the file to load.

  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_HREF)

### PROPERTY_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ID

The ID of an HTML element from the file specified by the "href" argument of "oxy_html_content". It identifies the element to be rendered.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ID)

### PROPERTY_FILE_FILTER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_FILE_FILTER

A set of file extensions specifying the file types that should be shown in the dialog displayed by a URL chooser. The extensions are comma-separated.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_FILE_FILTER)

### PROPERTY_TYPE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_TYPE

Indicates the editor that should be used to edit. One of TYPE_ constants or a class name. This is a shorthand to specify a built-in type of renderer and editor as opposed to using properties PROPERTY_RENDERER_CLASS_NAME, PROPERTY_SWING_EDITOR_CLASS_NAME and PROPERTY_SWT_EDITOR_CLASS_NAME.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_TYPE)

### PROPERTY_EDIT

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_EDIT
 Deprecated.
Use [InplaceEditorArgumentKeys.PROPERTY_EDIT_QUALIFIED](InplaceEditorArgumentKeys.md#PROPERTY_EDIT_QUALIFIED) instead. In case of an attribute it will offer a clark name instead of the QName used in the CSS.

Indicates if we should edit an attribute value or the text value of the element. The following values are accepted:
        * To edit an attribute value the value of the property is "@attr_name".
        * To edit the text content the value should be equal with [EDIT_TEXT_CONTENT](#EDIT_TEXT_CONTENT)
        * To let the editor do the editing itself, the value should be equal with [EDIT_CUSTOM](#EDIT_CUSTOM)

  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_EDIT)

### PROPERTY_VALUES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_VALUES

A set of values to be presented as choices. If not present these values will be taken from the schema. The processed value for this property is a list of [CIValue](../../../../contentcompletion/xml/CIValue.md).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_VALUES)

### PROPERTY_CAN_REMOVE_VALUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_CAN_REMOVE_VALUE

Property used for a non-editable combo box form control. If it is set to true, then the combo box will have an "<Empty>" value inside, which will clear/remove the last combo box value.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_CAN_REMOVE_VALUE)

### PROPERTY_UNCHECKED_VALUES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_UNCHECKED_VALUES

Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_CHECKBOX](#TYPE_CHECKBOX). These are the values that are committed for a checkbox when it is unchecked. If missing, an unchecked button will commit no value. The processed value for this property is a list of [CIValue](../../../../contentcompletion/xml/CIValue.md).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_UNCHECKED_VALUES)

### PROPERTY_LABELS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_LABELS

A set of labels to be associated with PROPERTY_VALUES. The processed value for this property is a java.util.List<String>
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_LABELS)

### PROPERTY_TOOLTIPS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_TOOLTIPS

A set of tooltips to be associated with PROPERTY_VALUES. The processed value for this property is a java.util.List<String>
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_TOOLTIPS)

### PROPERTY_ROWS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ROWS

The number of rows that the editor should have. It's interpretation is dependent to the editor being used.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ROWS)

### PROPERTY_COLUMNS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_COLUMNS

The number of columns that the editor should have. It's interpretation is dependent to the editor being used.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_COLUMNS)

### PROPERTY_WIDTH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_WIDTH

Imposes a width for the form control. The values are the same like the width property from CSS.
```

 elem {
   content: oxy_textfield(edit, '#text', width, 12em)
 }

```
If a form control also supports the [PROPERTY_COLUMNS](#PROPERTY_COLUMNS) and both of these properties are present, then [PROPERTY_WIDTH](#PROPERTY_WIDTH) will take precedence. The value for this property should not be requested directly but using [DynamicPropertyEvaluator.evaluateWidthProperty(java.util.Map, int)](DynamicPropertyEvaluator.md#evaluateWidthProperty(java.util.Map,int)). Such an instance can be obtain from [AuthorInplaceContext](AuthorInplaceContext.md). If you want to set this property from the API, it is best to use [InplaceEditorArgumentKeys.PROPERTY_PROCESSED_WIDTH](InplaceEditorArgumentKeys.md#PROPERTY_PROCESSED_WIDTH) instead.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_WIDTH)

### PROPERTY_SEPARATOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SEPARATOR

Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_CHECKBOX](#TYPE_CHECKBOX) or [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION). This is the separator that will be used to compose the values from the check-boxes into one string that will be committed into the document. If no separator is specified, a space will be used.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SEPARATOR)

### PROPERTY_RENDERER_SEPARATOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_RENDERER_SEPARATOR

Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION). This is the separator that will be used to compose the values from the check-boxes into one string that will be rendered in the document. If no separator is specified, [PROPERTY_SEPARATOR](#PROPERTY_SEPARATOR) will be used to identify tokens.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_RENDERER_SEPARATOR)

### PROPERTY_SORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SORT

Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION)and [PROPERTY_SELECTION_MODE](#PROPERTY_SELECTION_MODE) is set to [SELECTION_MODE_MULTIPLE](#SELECTION_MODE_MULTIPLE). This is the order in which the values in the element or attribute will appear. This sorting property will apply to both the values rendered in the editor and the ones presented in the pop-up editor. If no sort order is specified, the values will be rendered in the order in which they appear in the document.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SORT)

### PROPERTY_RENDERER_SORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_RENDERER_SORT

Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION). This is the order in which the values in the element or attribute will appear rendered in the editor. If no sort order is specified, the values will be rendered in the order in which they appear in the document.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_RENDERER_SORT)

### PROPERTY_EDITOR_SORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_EDITOR_SORT

Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION) and [PROPERTY_SELECTION_MODE](#PROPERTY_SELECTION_MODE) is set to [SELECTION_MODE_MULTIPLE](#SELECTION_MODE_MULTIPLE). This is the order in which the values specified for the element or attribute will be presented in the pop-up editor. If no sort order is specified, the values will be presented in the order in which they appear in the document.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_EDITOR_SORT)

### SORT_ASCENDING

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SORT_ASCENDING

Value Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION). Sort in ascending lexicographical order.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.SORT_ASCENDING)

### SORT_DESCENDING

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SORT_DESCENDING

Value Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION). Sort in descending lexicographical order.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.SORT_DESCENDING)

### PROPERTY_EDITABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_EDITABLE

Only applies when the editor is a combo box and marks the combo as being editable or not. possible values are Boolean.TRUE and Boolean.FALSE.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_EDITABLE)

### PROPERTY_ACTION_ID

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ACTION_ID

Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and represents the ID of the action that must be invoked when the button is pressed. It's processed value is an [IAuthorExtensionAction](IAuthorExtensionAction.md). If an action with the given ID wasn't found the value remains the given string ID.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ACTION_ID)

### PROPERTY_ACTION_CONTEXT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ACTION_CONTEXT

Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP). It specifies the context in which the action associated with the form control will be executed in. The default value is [ACTION_CONTEXT_ELEMENT](#ACTION_CONTEXT_ELEMENT).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ACTION_CONTEXT)

### PROPERTY_TRANSPARENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_TRANSPARENT

Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and ensures whether the button will have a more flat appearance (transparent). The accepted values are true and false. The default value is false which will determine a classic looking button. When true, the SWING button will have no borders while the SWT one will be a tool item. The processed values will be either Boolean.TRUE or Boolean.FALSE.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_TRANSPARENT)

### PROPERTY_ACTION_IDS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ACTION_IDS

Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and contains a list of comma separated IDs of the actions that are presented to the user in a pop-up menu. It's processed value is a list of [IAuthorExtensionAction](IAuthorExtensionAction.md). If one of the actions IDs wasn't found the value remains the given string ID.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ACTION_IDS)

### PROPERTY_ICON

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ICON

Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and specifies the path to an Icon to be displayed on the button. The processed value is an Icon to be displayed on the button or null if no icon is specified or the specified one cannot be loaded.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ICON)

### PROPERTY_SHOW_TEXT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SHOW_TEXT

Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and specifies if the text should be displayed on the button. If missing, the button displays only the icon if it is available, or the text if the icon is not available. This is a boolean property.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SHOW_TEXT)

### PROPERTY_SHOW_ICON

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SHOW_ICON

Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and specifies if the icon should be displayed on the button. If missing, the button displays only the icon if it is available, or the text if the icon is not available. This is a boolean property.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SHOW_ICON)

### PROPERTY_ENABLE_IN_READ_ONLY_CONTEXT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ENABLE_IN_READ_ONLY_CONTEXT

Controls whether the button is enabled/disabled in read-only context. Default value is [FALSE](#FALSE).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ENABLE_IN_READ_ONLY_CONTEXT)

### PROPERTY_LABEL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_LABEL

Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and specifies the label of the button that triggers the pop-up menu.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_LABEL)

### PROPERTY_TOOLTIP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_TOOLTIP

Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and [TYPE_TEXT](#TYPE_TEXT) and specifies the tooltip for the button that triggers the pop-up menu with the actions in the group.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_TOOLTIP)

### PROPERTY_ACTION_DISPLAY_STYLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ACTION_DISPLAY_STYLE

Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and specifies what to display for an action: icon, text or both.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ACTION_DISPLAY_STYLE)

### PROPERTY_RENDERER_CLASS_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_RENDERER_CLASS_NAME

Class name of the renderer. This must be a SWING implementation for both the Oxygen stand alone or Eclipse plugin version. This class will be look for in the class path of the associated document type or in the [PROPERTY_CLASSPATH](#PROPERTY_CLASSPATH).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_RENDERER_CLASS_NAME)

### PROPERTY_SWING_EDITOR_CLASS_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SWING_EDITOR_CLASS_NAME

Class name of the editor. The SWING implementation is used for the Oxygen stand alone. This class will be look for in the class path of the associated document type or in the [PROPERTY_CLASSPATH](#PROPERTY_CLASSPATH).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SWING_EDITOR_CLASS_NAME)

### PROPERTY_SWT_EDITOR_CLASS_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SWT_EDITOR_CLASS_NAME

Class name of the editor. The SWT implementation is used for the Eclipse plugin version. This class will be look for in the class path of the associated document type or in the [PROPERTY_CLASSPATH](#PROPERTY_CLASSPATH).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SWT_EDITOR_CLASS_NAME)

### PROPERTY_WEBAPP_RENDERER_CLASS_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_WEBAPP_RENDERER_CLASS_NAME

Class name of the server-side renderer used in the Author Webapp. This class will be looked for in the class path of the associated document type or in the [PROPERTY_CLASSPATH](#PROPERTY_CLASSPATH).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_WEBAPP_RENDERER_CLASS_NAME)

### PROPERTY_CLASSPATH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_CLASSPATH

If the form control is a custom implementation this property can be used to specify the class path where the custom implementation will loaded from. A comma separated enumeration of URLs.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_CLASSPATH)

### PROPERTY_SELECTION_MODE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SELECTION_MODE

Used only when [PROPERTY_TYPE](#PROPERTY_TYPE) is set to [TYPE_POPUP_SELECTION](#TYPE_POPUP_SELECTION). Its possible values are [SELECTION_MODE_SINGLE](#SELECTION_MODE_SINGLE) and [SELECTION_MODE_MULTIPLE](#SELECTION_MODE_MULTIPLE). The default value is [SELECTION_MODE_MULTIPLE](#SELECTION_MODE_MULTIPLE).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SELECTION_MODE)

### PROPERTY_FONT_INHERIT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_FONT_INHERIT

Property used to specify that the font is inherited from the parent element. Its possible values are true or false.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_FONT_INHERIT)

### PROPERTY_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_COLOR

Property used to specify the foreground color. Its possible values are a color or 'inherit' if the color should be inherited from the element.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_COLOR)

### PROPERTY_CONTENT_TYPE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_CONTENT_TYPE

Property used to specify the content type of the edited string. The values belongs to the ContentTypes
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_CONTENT_TYPE)

### PROPERTY_VISIBLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_VISIBLE

Property used to specify if an in-place editor is visible. Its possible values are true or false.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_VISIBLE)

### PROPERTY_VALIDATE_INPUT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_VALIDATE_INPUT

Controls the validation of the input.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_VALIDATE_INPUT)

### PROPERTY_INDENT_ON_TAB

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_INDENT_ON_TAB

Controls the TAB behavior in the text area form control. If this property is true, TAB is used for indentation instead of navigation. By default, it is set to true.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_INDENT_ON_TAB)

### ACTION_CONTEXT_ELEMENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_CONTEXT_ELEMENT

Possible value for [PROPERTY_ACTION_CONTEXT](#PROPERTY_ACTION_CONTEXT). The action will be executed in the context of the element associated with the form control.
We want the form control below to delete the li element even if the caret is located in a descendant of li.

```

 li:before {
   content:oxy_button(actionID, 'delete.element', actionContext, 'element')
 }

```

  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.ACTION_CONTEXT_ELEMENT)

### ACTION_CONTEXT_CARET

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_CONTEXT_CARET

Possible value for [PROPERTY_ACTION_CONTEXT](#PROPERTY_ACTION_CONTEXT). The action will be executed in the current selection context. The selection/caret must be inside the element associated with the form control. Otherwise the action will be executed in [ACTION_CONTEXT_ELEMENT](#ACTION_CONTEXT_ELEMENT) context.
The form control is added on a 'para' element. Whenever the user makes a selection inside 'para' and clicks the button we want to wrap the existing selection in a 'b' element.

```

 para:before {
   content:oxy_button(actionID, 'bold.wrap', actionContext, 'caret')
 }

```

  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.ACTION_CONTEXT_CARET)

### TYPE_BUTTON

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_BUTTON

Possible value for PROPERTY_TYPE. Indicates that a combo box should be used to render and edit.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_BUTTON)

### TYPE_COMBOBOX

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_COMBOBOX

Possible value for PROPERTY_TYPE. Indicates that a combo box should be used to render and edit.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_COMBOBOX)

### TYPE_TEXT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_TEXT

Possible value for PROPERTY_TYPE. Indicates that a text field with content completion support should be used to render and edit.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_TEXT)

### TYPE_TEXT_AREA

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_TEXT_AREA

Possible value for PROPERTY_TYPE. Indicates that a text area with syntax highlight support should be used to render and edit.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_TEXT_AREA)

### TYPE_HTML_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_HTML_CONTENT

Possible value for PROPERTY_TYPE. Indicates that a pane with HTML interpreting support should be used to render.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_HTML_CONTENT)

### TYPE_CHECKBOX

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_CHECKBOX

Possible value for PROPERTY_TYPE. Indicates that a check box panel should be used to render and edit.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_CHECKBOX)

### TYPE_POPUP_SELECTION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_POPUP_SELECTION

The renderer presents a simple or compose value and the editor shows a pop-up like panel in which we can choose the values.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_POPUP_SELECTION)

### TYPE_URL_CHOOSER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_URL_CHOOSER

Possible value for PROPERTY_TYPE. Indicates that a URL chooser should be used to render and edit. The new type of URL chooser that uses an InputUrlPanel.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_URL_CHOOSER)

### TYPE_BUTTON_GROUP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_BUTTON_GROUP

Possible value for PROPERTY_TYPE. Indicates that a button with a pop-up menu that contains a list of actions should be used to render and edit.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_BUTTON_GROUP)

### EDIT_TEXT_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDIT_TEXT_CONTENT

Value of the PROPERTY_EDIT that indicates that the text content of the element must be edited.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.EDIT_TEXT_CONTENT)

### EDIT_XML_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDIT_XML_CONTENT

Handled only for a text area editor [TYPE_TEXT_AREA](#TYPE_TEXT_AREA). This parameter is useful when an element has mixed or element-only content and you want to edit its content inside a text area form control. For example:
XML:

```
<codeblock outputclass="language-xml">START_TEXT<ph>phase</ph><apiname><text>API</text></apiname></codeblock>
```

CSS

```
codeblock:before{
content:
    oxy_textArea(
      edit, content,
      contentType, 'text/xml');
}
```
The text area form control will edit this fragment:
START_TEXT<ph>phase</ph><apiname><text>API</text></apiname>

  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.EDIT_XML_CONTENT)

### EDIT_CUSTOM

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDIT_CUSTOM

Value of the PROPERTY_EDIT that indicates that the editor is doing a custom edit session and it's up to the editor to update the document.

In this situation it is recommended for the editor to give an [EditingEvent.customEdit](EditingEvent.md#customEdit)on [InplaceEditingListener.commitValue(EditingEvent)](InplaceEditingListener.md#commitValue(ro.sync.ecss.extensions.api.editor.EditingEvent)). If that's not done the following apply:

In this case the notification [InplaceEditingListener.commitValue(EditingEvent)](InplaceEditingListener.md#commitValue(ro.sync.ecss.extensions.api.editor.EditingEvent)) will do nothing since it's not clear where should the given value be committed.

The notification [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent)) will also stop the editing session without committing any value. It's up to the custom editor to make the necessary changes into the document (but only after the previous mentioned notification was issued).

 Warning:All changes to the document (that the custom editor must do) must be performed after the [InplaceEditingListener.editingStopped(EditingEvent)](InplaceEditingListener.md#editingStopped(ro.sync.ecss.extensions.api.editor.EditingEvent))notification was fired. Because the editing is automatically stopped on any document modification an infinite loop will happen if the previous condition is not met.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.EDIT_CUSTOM)

### FALSE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FALSE

Possible value for PROPERTY_EDITABLE that marks the combo as NOT being editable.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.FALSE)

### TRUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TRUE

Possible value for PROPERTY_EDITABLE that marks the combo as being editable.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TRUE)

### SELECTION_MODE_SINGLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SELECTION_MODE_SINGLE

Possible value for ["selectionMode"](#PROPERTY_SELECTION_MODE). Only a single value will be selected.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.SELECTION_MODE_SINGLE)

### SELECTION_MODE_MULTIPLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SELECTION_MODE_MULTIPLE

Possible value for ["selectionMode"](#PROPERTY_SELECTION_MODE). It allows multiple values to be selected.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.SELECTION_MODE_MULTIPLE)

### TYPE_DATE_PICKER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_DATE_PICKER

An editor that can be used to edit dates. It handles schema types xs:date and xs:datetime or any type with a specified Java format from CSS.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_DATE_PICKER)

### TYPE_OLD_URL_CHOOSER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_OLD_URL_CHOOSER

The old url chooser. Left here as a workaround if someone got really attached to it.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_OLD_URL_CHOOSER)

### PROPERTY_FORMAT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_FORMAT

It applies only on date picker form control. It specifies the date-time format of the edited value.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_FORMAT)

### COMMA

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) COMMA

The variable used to add a comma in property values. The real comma is used as a delimiter for multiple values thus this special variable is needed.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.COMMA)

### INHERIT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) INHERIT

Value constant used for the color property.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.INHERIT)

### PROPERTY_ACTION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ACTION

Only applies to the [TYPE_BUTTON](#TYPE_BUTTON) and represents the action that must be invoked when the button is pressed. The processed value is an [IAuthorExtensionAction](IAuthorExtensionAction.md) that is stored into the [PROPERTY_ACTION_ID](#PROPERTY_ACTION_ID).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ACTION)

### PROPERTY_ACTIONS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ACTIONS

Only applies to the [TYPE_BUTTON_GROUP](#TYPE_BUTTON_GROUP) and represents the list of the actions that can be invoked. The processed value is a list of a [IAuthorExtensionAction](IAuthorExtensionAction.md) that is stored into the [PROPERTY_ACTION_IDS](#PROPERTY_ACTION_IDS).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ACTIONS)

### PROPERTY_HAS_MULTIPLE_VALUES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_HAS_MULTIPLE_VALUES

Property that can be set on a text field form control. If true, then the form control can have multiple values, separated by spaces. If false, it can have a single value. The default is true.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_HAS_MULTIPLE_VALUES)

### TYPE_VIDEO_PLAYER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_VIDEO_PLAYER

Possible value for PROPERTY_TYPE. Indicates a video player.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_VIDEO_PLAYER)

### TYPE_AUDIO_PLAYER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_AUDIO_PLAYER

Possible value for PROPERTY_TYPE. Indicates an audio player.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_AUDIO_PLAYER)

### TYPE_BROWSER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TYPE_BROWSER

Possible value for PROPERTY_TYPE. Indicates a JavaFX-based browser.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.TYPE_BROWSER)

### PROPERTY_HEIGHT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_HEIGHT

Imposes a height for a [TYPE_VIDEO_PLAYER](#TYPE_VIDEO_PLAYER) and [TYPE_BROWSER](#TYPE_BROWSER). The values are the same like height property from CSS with one exception:
% Defines the height in percent of the entire viewport height

```

 elem {
   content: oxy_video(href, 'page.html', width, 12em, height, 10em)
 }

```
The value for this property should not be requested directly but using [DynamicPropertyEvaluator.evaluateHeightProperty(java.util.Map, int)](DynamicPropertyEvaluator.md#evaluateHeightProperty(java.util.Map,int)). Such an instance can be obtain from [AuthorInplaceContext](AuthorInplaceContext.md).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_HEIGHT)

### PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME

Heavy weight form controls extension point. These form controls differ from the classic form control by the fact that they are placed in the component hierarchy from the very beginning. Class name of a heavy weight form control. This implementation is used in the Desktop version of Oxygen.
**Note** If Oxygen is running as a Eclipse plugin then you'll have to use [PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME](#PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME)

**Note** If Oxygen is running as a Standalone or Desktop version then you'll have to use [PROPERTY_WEBAPP_RENDERER_CLASS_NAME](#PROPERTY_WEBAPP_RENDERER_CLASS_NAME)
This class will be look for in the class path of the associated document type or in the [PROPERTY_CLASSPATH](#PROPERTY_CLASSPATH).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME)

### PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME

Heavy weight form controls extension point. These form controls differ from the classic form control by the fact that they are placed in the component hierarchy from the very beginning. Class name of a heavy weight form control. This implementation is used when Oxygen is running inside an Eclipse environment.
**Note** If Oxygen is running as a Standalone or Desktop version then you'll have to use [PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME](#PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME)

**Note** If Oxygen is running as a Standalone or Desktop version then you'll have to use [PROPERTY_WEBAPP_RENDERER_CLASS_NAME](#PROPERTY_WEBAPP_RENDERER_CLASS_NAME)
 This class will be look for in the class path of the associated document type or in the [PROPERTY_CLASSPATH](#PROPERTY_CLASSPATH).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME)

### PROPERTY_ON_CHANGE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_ON_CHANGE

Combo box property. Can be used to invoke an action every time combo changes its value.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_ON_CHANGE)

### PROPERTY_SPELL_CHECK

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_SPELL_CHECK

Only applies to text fields, text areas and editable combo boxes. The accepted values are true and false. The default value is false. When true, the content inside the text field is spell-checked if the automatic spell checking is enabled in the application. The processed values will be either Boolean.TRUE or Boolean.FALSE.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorCSSConstants.PROPERTY_SPELL_CHECK)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
