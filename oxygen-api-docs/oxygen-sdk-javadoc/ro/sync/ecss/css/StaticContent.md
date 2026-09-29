Package [ro.sync.ecss.css](package-summary.md)

# Interface StaticContent
    All Known Implementing Classes: [EditorContent](EditorContent.md), [LabelContent](LabelContent.md), [StringContent](StringContent.md), [URIContent](URIContent.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public interface StaticContent
Static content which should be generated for an element

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [CONTENT_CONTENT](#CONTENT_CONTENT)
Content type for the CSS content() from the string-set property.
  static final int [COUNTER_CONTENT](#COUNTER_CONTENT)
Counter content type.
  static final int [COUNTERS_CONTENT](#COUNTERS_CONTENT)
Counters content type.
  static final int [EDITOR_CONTENT](#EDITOR_CONTENT)
Content type for form controls..
  static final int [LABEL_CONTENT](#LABEL_CONTENT)
Content type for a label.
  static final int [LEADER_CONTENT](#LEADER_CONTENT)
Content type for the CSS leader().
  static final int [STRING_FUNCTION_CONTENT](#STRING_FUNCTION_CONTENT)
The equivalent of a 'string' function, it is used to extract the value of a named string defined by a 'string-set' property.
  static final int [TARGET_COUNTER_CONTENT](#TARGET_COUNTER_CONTENT)
Content type for the CSS target-counter().
  static final int [TARGET_COUNTERS_CONTENT](#TARGET_COUNTERS_CONTENT)
Content type for the CSS target-counters().
  static final int [TEXT_CONTENT](#TEXT_CONTENT)
Text content type
  static final int [URI_CONTENT](#URI_CONTENT)
URI content type

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getType](#getType())()
Gets the content type.

## Field Details

### TEXT_CONTENT

static final int TEXT_CONTENT

Text content type
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.TEXT_CONTENT)

### URI_CONTENT

static final int URI_CONTENT

URI content type
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.URI_CONTENT)

### COUNTER_CONTENT

static final int COUNTER_CONTENT

Counter content type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.COUNTER_CONTENT)

### COUNTERS_CONTENT

static final int COUNTERS_CONTENT

Counters content type.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.COUNTERS_CONTENT)

### EDITOR_CONTENT

static final int EDITOR_CONTENT

Content type for form controls..
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.EDITOR_CONTENT)

### LABEL_CONTENT

static final int LABEL_CONTENT

Content type for a label. Allows styling.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.LABEL_CONTENT)

### LEADER_CONTENT

static final int LEADER_CONTENT

Content type for the CSS leader(). This is used only in the CSS to FO converter.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.LEADER_CONTENT)

### TARGET_COUNTER_CONTENT

static final int TARGET_COUNTER_CONTENT

Content type for the CSS target-counter(). This is used only in the CSS to FO converter.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.TARGET_COUNTER_CONTENT)

### TARGET_COUNTERS_CONTENT

static final int TARGET_COUNTERS_CONTENT

Content type for the CSS target-counters(). This is used only in the CSS to FO converter.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.TARGET_COUNTERS_CONTENT)

### CONTENT_CONTENT

static final int CONTENT_CONTENT

Content type for the CSS content() from the string-set property. This is used only in the CSS to FO converter.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.CONTENT_CONTENT)

### STRING_FUNCTION_CONTENT

static final int STRING_FUNCTION_CONTENT

The equivalent of a 'string' function, it is used to extract the value of a named string defined by a 'string-set' property. This is used only in the CSS to FO converter.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.StaticContent.STRING_FUNCTION_CONTENT)

## Method Details

### getType

int getType()

Gets the content type.
  Returns: The content type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
