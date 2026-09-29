Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface InplaceEditorArgumentKeys
    All Superinterfaces: [InplaceEditorCSSConstants](InplaceEditorCSSConstants.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface InplaceEditorArgumentKeysextends [InplaceEditorCSSConstants](InplaceEditorCSSConstants.md)
Properties of the oxy_editor function extended with other computed properties that the renderer/editor might need.
  Since: 14.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [BG_COLOR](#BG_COLOR)
The default background color to be used by the renderers/editors.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DEFAULT_VALUE](#DEFAULT_VALUE)
The default value for the property being edited.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FONT](#FONT)
The font to be used by the renderer/editor or null to go with the default.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [INITIAL_VALUE](#INITIAL_VALUE)
The current value for the property being edited.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [INITIAL_VALUE_PARSER_IMPL](#INITIAL_VALUE_PARSER_IMPL)
A parser used to process the initial value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_EDIT_QUALIFIED](#PROPERTY_EDIT_QUALIFIED)
Same as [InplaceEditorCSSConstants.PROPERTY_EDIT](InplaceEditorCSSConstants.md#PROPERTY_EDIT) except when we are editing an attribute and this attribute was specified as a QName.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_HTML_CONTENT_BASE_URL](#PROPERTY_HTML_CONTENT_BASE_URL)
The base URL for the HTML content rendered by an [InplaceEditorCSSConstants.TYPE_HTML_CONTENT](InplaceEditorCSSConstants.md#TYPE_HTML_CONTENT)form control.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_IMAGE_MAP_SUPPORT_FACTORY](#PROPERTY_IMAGE_MAP_SUPPORT_FACTORY)
The name of a Java class that implements [WebappImageMapSupportFactory](../webapp/imagemap/WebappImageMapSupportFactory.md).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_IMAGE_URL](#PROPERTY_IMAGE_URL)
The URL of the image used by the image map for control for Web Author.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_PROCESSED_WIDTH](#PROPERTY_PROCESSED_WIDTH)
The value of this property is computed from [InplaceEditorCSSConstants.PROPERTY_WIDTH](InplaceEditorCSSConstants.md#PROPERTY_WIDTH).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROPERTY_VALUES_FOR_EDITING](#PROPERTY_VALUES_FOR_EDITING)
A set of values to be presented as choices.

### Fields inherited from interface ro.sync.ecss.extensions.api.editor.[InplaceEditorCSSConstants](InplaceEditorCSSConstants.md)
 [ACTION_CONTEXT_CARET](InplaceEditorCSSConstants.md#ACTION_CONTEXT_CARET), [ACTION_CONTEXT_ELEMENT](InplaceEditorCSSConstants.md#ACTION_CONTEXT_ELEMENT), [COMMA](InplaceEditorCSSConstants.md#COMMA), [EDIT_CUSTOM](InplaceEditorCSSConstants.md#EDIT_CUSTOM), [EDIT_TEXT_CONTENT](InplaceEditorCSSConstants.md#EDIT_TEXT_CONTENT), [EDIT_XML_CONTENT](InplaceEditorCSSConstants.md#EDIT_XML_CONTENT), [FALSE](InplaceEditorCSSConstants.md#FALSE), [INHERIT](InplaceEditorCSSConstants.md#INHERIT), [PROPERTY_ACTION](InplaceEditorCSSConstants.md#PROPERTY_ACTION), [PROPERTY_ACTION_CONTEXT](InplaceEditorCSSConstants.md#PROPERTY_ACTION_CONTEXT), [PROPERTY_ACTION_DISPLAY_STYLE](InplaceEditorCSSConstants.md#PROPERTY_ACTION_DISPLAY_STYLE), [PROPERTY_ACTION_ID](InplaceEditorCSSConstants.md#PROPERTY_ACTION_ID), [PROPERTY_ACTION_IDS](InplaceEditorCSSConstants.md#PROPERTY_ACTION_IDS), [PROPERTY_ACTIONS](InplaceEditorCSSConstants.md#PROPERTY_ACTIONS), [PROPERTY_CAN_REMOVE_VALUE](InplaceEditorCSSConstants.md#PROPERTY_CAN_REMOVE_VALUE), [PROPERTY_CLASSPATH](InplaceEditorCSSConstants.md#PROPERTY_CLASSPATH), [PROPERTY_COLOR](InplaceEditorCSSConstants.md#PROPERTY_COLOR), [PROPERTY_COLUMNS](InplaceEditorCSSConstants.md#PROPERTY_COLUMNS), [PROPERTY_CONTENT_TYPE](InplaceEditorCSSConstants.md#PROPERTY_CONTENT_TYPE), [PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_ECLIPSE_HEAVY_FORM_CONTROL_CLASS_NAME), [PROPERTY_EDIT](InplaceEditorCSSConstants.md#PROPERTY_EDIT), [PROPERTY_EDITABLE](InplaceEditorCSSConstants.md#PROPERTY_EDITABLE), [PROPERTY_EDITOR_SORT](InplaceEditorCSSConstants.md#PROPERTY_EDITOR_SORT), [PROPERTY_ENABLE_IN_READ_ONLY_CONTEXT](InplaceEditorCSSConstants.md#PROPERTY_ENABLE_IN_READ_ONLY_CONTEXT), [PROPERTY_FILE_FILTER](InplaceEditorCSSConstants.md#PROPERTY_FILE_FILTER), [PROPERTY_FONT_INHERIT](InplaceEditorCSSConstants.md#PROPERTY_FONT_INHERIT), [PROPERTY_FORMAT](InplaceEditorCSSConstants.md#PROPERTY_FORMAT), [PROPERTY_HAS_MULTIPLE_VALUES](InplaceEditorCSSConstants.md#PROPERTY_HAS_MULTIPLE_VALUES), [PROPERTY_HEIGHT](InplaceEditorCSSConstants.md#PROPERTY_HEIGHT), [PROPERTY_HREF](InplaceEditorCSSConstants.md#PROPERTY_HREF), [PROPERTY_HTML_EMBEDDED_CONTENT](InplaceEditorCSSConstants.md#PROPERTY_HTML_EMBEDDED_CONTENT), [PROPERTY_ICON](InplaceEditorCSSConstants.md#PROPERTY_ICON), [PROPERTY_ID](InplaceEditorCSSConstants.md#PROPERTY_ID), [PROPERTY_INDENT_ON_TAB](InplaceEditorCSSConstants.md#PROPERTY_INDENT_ON_TAB), [PROPERTY_LABEL](InplaceEditorCSSConstants.md#PROPERTY_LABEL), [PROPERTY_LABELS](InplaceEditorCSSConstants.md#PROPERTY_LABELS), [PROPERTY_ON_CHANGE](InplaceEditorCSSConstants.md#PROPERTY_ON_CHANGE), [PROPERTY_ON_HOVER_PSEUDO_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_ON_HOVER_PSEUDO_CLASS_NAME), [PROPERTY_RENDERER_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_RENDERER_CLASS_NAME), [PROPERTY_RENDERER_SEPARATOR](InplaceEditorCSSConstants.md#PROPERTY_RENDERER_SEPARATOR), [PROPERTY_RENDERER_SORT](InplaceEditorCSSConstants.md#PROPERTY_RENDERER_SORT), [PROPERTY_ROWS](InplaceEditorCSSConstants.md#PROPERTY_ROWS), [PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_SA_HEAVY_FORM_CONTROL_CLASS_NAME), [PROPERTY_SELECTION_MODE](InplaceEditorCSSConstants.md#PROPERTY_SELECTION_MODE), [PROPERTY_SEPARATOR](InplaceEditorCSSConstants.md#PROPERTY_SEPARATOR), [PROPERTY_SHOW_ICON](InplaceEditorCSSConstants.md#PROPERTY_SHOW_ICON), [PROPERTY_SHOW_TEXT](InplaceEditorCSSConstants.md#PROPERTY_SHOW_TEXT), [PROPERTY_SORT](InplaceEditorCSSConstants.md#PROPERTY_SORT), [PROPERTY_SPELL_CHECK](InplaceEditorCSSConstants.md#PROPERTY_SPELL_CHECK), [PROPERTY_SWING_EDITOR_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_SWING_EDITOR_CLASS_NAME), [PROPERTY_SWT_EDITOR_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_SWT_EDITOR_CLASS_NAME), [PROPERTY_TOOLTIP](InplaceEditorCSSConstants.md#PROPERTY_TOOLTIP), [PROPERTY_TOOLTIPS](InplaceEditorCSSConstants.md#PROPERTY_TOOLTIPS), [PROPERTY_TRANSPARENT](InplaceEditorCSSConstants.md#PROPERTY_TRANSPARENT), [PROPERTY_TYPE](InplaceEditorCSSConstants.md#PROPERTY_TYPE), [PROPERTY_UNCHECKED_VALUES](InplaceEditorCSSConstants.md#PROPERTY_UNCHECKED_VALUES), [PROPERTY_VALIDATE_INPUT](InplaceEditorCSSConstants.md#PROPERTY_VALIDATE_INPUT), [PROPERTY_VALUES](InplaceEditorCSSConstants.md#PROPERTY_VALUES), [PROPERTY_VISIBLE](InplaceEditorCSSConstants.md#PROPERTY_VISIBLE), [PROPERTY_WEBAPP_RENDERER_CLASS_NAME](InplaceEditorCSSConstants.md#PROPERTY_WEBAPP_RENDERER_CLASS_NAME), [PROPERTY_WIDTH](InplaceEditorCSSConstants.md#PROPERTY_WIDTH), [SELECTION_MODE_MULTIPLE](InplaceEditorCSSConstants.md#SELECTION_MODE_MULTIPLE), [SELECTION_MODE_SINGLE](InplaceEditorCSSConstants.md#SELECTION_MODE_SINGLE), [SORT_ASCENDING](InplaceEditorCSSConstants.md#SORT_ASCENDING), [SORT_DESCENDING](InplaceEditorCSSConstants.md#SORT_DESCENDING), [TRUE](InplaceEditorCSSConstants.md#TRUE), [TYPE_AUDIO_PLAYER](InplaceEditorCSSConstants.md#TYPE_AUDIO_PLAYER), [TYPE_BROWSER](InplaceEditorCSSConstants.md#TYPE_BROWSER), [TYPE_BUTTON](InplaceEditorCSSConstants.md#TYPE_BUTTON), [TYPE_BUTTON_GROUP](InplaceEditorCSSConstants.md#TYPE_BUTTON_GROUP), [TYPE_CHECKBOX](InplaceEditorCSSConstants.md#TYPE_CHECKBOX), [TYPE_COMBOBOX](InplaceEditorCSSConstants.md#TYPE_COMBOBOX), [TYPE_DATE_PICKER](InplaceEditorCSSConstants.md#TYPE_DATE_PICKER), [TYPE_HTML_CONTENT](InplaceEditorCSSConstants.md#TYPE_HTML_CONTENT), [TYPE_OLD_URL_CHOOSER](InplaceEditorCSSConstants.md#TYPE_OLD_URL_CHOOSER), [TYPE_POPUP_SELECTION](InplaceEditorCSSConstants.md#TYPE_POPUP_SELECTION), [TYPE_TEXT](InplaceEditorCSSConstants.md#TYPE_TEXT), [TYPE_TEXT_AREA](InplaceEditorCSSConstants.md#TYPE_TEXT_AREA), [TYPE_URL_CHOOSER](InplaceEditorCSSConstants.md#TYPE_URL_CHOOSER), [TYPE_VIDEO_PLAYER](InplaceEditorCSSConstants.md#TYPE_VIDEO_PLAYER)
## Field Details

### PROPERTY_VALUES_FOR_EDITING

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_VALUES_FOR_EDITING

A set of values to be presented as choices. If not present these values will be taken from the PROPERTY_VALUES key. The processed value for this property is a list of CIValue.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.PROPERTY_VALUES_FOR_EDITING)

### INITIAL_VALUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) INITIAL_VALUE

The current value for the property being edited.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.INITIAL_VALUE)

### INITIAL_VALUE_PARSER_IMPL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) INITIAL_VALUE_PARSER_IMPL

A parser used to process the initial value. AInitialValueParser} implementation.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.INITIAL_VALUE_PARSER_IMPL)

### DEFAULT_VALUE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DEFAULT_VALUE

The default value for the property being edited.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.DEFAULT_VALUE)

### FONT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FONT

The font to be used by the renderer/editor or null to go with the default. A [Font](../../../../exml/view/graphics/Font.md).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.FONT)

### BG_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) BG_COLOR

The default background color to be used by the renderers/editors.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.BG_COLOR)

### PROPERTY_EDIT_QUALIFIED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_EDIT_QUALIFIED

Same as [InplaceEditorCSSConstants.PROPERTY_EDIT](InplaceEditorCSSConstants.md#PROPERTY_EDIT) except when we are editing an attribute and this attribute was specified as a QName. The value of the property should have the format of the [QName.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html#toString()). Currently, it is the Clark's notation which has the form: {namespace}local_name.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.PROPERTY_EDIT_QUALIFIED)

### PROPERTY_PROCESSED_WIDTH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_PROCESSED_WIDTH

The value of this property is computed from [InplaceEditorCSSConstants.PROPERTY_WIDTH](InplaceEditorCSSConstants.md#PROPERTY_WIDTH). The value for this property is either a [RelativeLength](../../../css/RelativeLength.md) (such a value can be created by calling RelativeLength.createAbsolute(int value) ) or an org.w3c.css.sac.LexicalUnit (e.g. em - ems can be created by calling org.w3c.flute.parser.LexicalUnitImpl.createEMS(-1, -1, null, float value) ). Either way, to evaluate the property you must use the [DynamicPropertyEvaluator](DynamicPropertyEvaluator.md) available in [AuthorInplaceContext](AuthorInplaceContext.md).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.PROPERTY_PROCESSED_WIDTH)

### PROPERTY_HTML_CONTENT_BASE_URL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_HTML_CONTENT_BASE_URL

The base URL for the HTML content rendered by an [InplaceEditorCSSConstants.TYPE_HTML_CONTENT](InplaceEditorCSSConstants.md#TYPE_HTML_CONTENT)form control. This URL will be used to resolve relative references, for example an image reference:
```
<img src="AcceptValue16.png" alt="NOT FOUND" />
```
The value of this property is java.lang.String set to:
        * If the HTML content is provided using the property [InplaceEditorCSSConstants.PROPERTY_HREF](InplaceEditorCSSConstants.md#PROPERTY_HREF) then the base URL is [InplaceEditorCSSConstants.PROPERTY_HREF](InplaceEditorCSSConstants.md#PROPERTY_HREF)
        * If the HTML content is provided uning the [InplaceEditorCSSConstants.PROPERTY_HTML_EMBEDDED_CONTENT](InplaceEditorCSSConstants.md#PROPERTY_HTML_EMBEDDED_CONTENT)property then the base URL is the URL of the CSS in which the form control appears.

  Since: 17 See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.PROPERTY_HTML_CONTENT_BASE_URL)

### PROPERTY_IMAGE_URL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_IMAGE_URL

The URL of the image used by the image map for control for Web Author.
  Since: 25 See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.PROPERTY_IMAGE_URL)

### PROPERTY_IMAGE_MAP_SUPPORT_FACTORY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROPERTY_IMAGE_MAP_SUPPORT_FACTORY

The name of a Java class that implements [WebappImageMapSupportFactory](../webapp/imagemap/WebappImageMapSupportFactory.md). It is used by the image used by the image map for control for Web Author.
  Since: 25 See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.editor.InplaceEditorArgumentKeys.PROPERTY_IMAGE_MAP_SUPPORT_FACTORY)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
