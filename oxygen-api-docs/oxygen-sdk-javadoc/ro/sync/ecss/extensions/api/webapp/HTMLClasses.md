Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface HTMLClasses
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface HTMLClasses
HTML classes used to identify the role of HTML elements.
  Since: 15.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DOCUMENT](#DOCUMENT)
Class used to identify the document root.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EMPTY_PLACEHOLDER](#EMPTY_PLACEHOLDER)
Class used to identify the span generated as a placeholder in empty elements.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [END_SENTINEL_MARKER](#END_SENTINEL_MARKER)
Class used to identify a marker that surrounds an end sentinel.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FILTERED](#FILTERED)
Marks content that is filtered by the active profiling conditions.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FOLDABLE](#FOLDABLE)
Class that marks foldable nodes.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FOLDED_BY_DEFAULT](#FOLDED_BY_DEFAULT)
Class that marks folded nodes.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [GHOST_MARKER](#GHOST_MARKER)
If a delete marker covers a sentinel, but not its pair the XML PI serialization does not cover the sentinel.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [IMAGE_MARKER](#IMAGE_MARKER)
Class used to identify a marker that surrounds an image.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [IMAGE_WRAPPER](#IMAGE_WRAPPER)
Class used to identify wrapper elements used to style images for change tracking and comments.
  static final [CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) [LABEL](#LABEL)
Class of oxy_label spans.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LABEL_WIDTH_SPECIFIED](#LABEL_WIDTH_SPECIFIED)
Extra class for oxy_label spans which have a specified width.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MARKER](#MARKER)
Class used to identify elements that correspond to markers.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MARKER_PSEUDO_ELEMENT_OUTSIDE](#MARKER_PSEUDO_ELEMENT_OUTSIDE)
Class added to CSS ::marker pseudo-elements that need to be rendered outside their parent.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXY_COLLAPSE_TEXT](#OXY_COLLAPSE_TEXT)
Class that marks nodes with "visibility: -oxy-collapse-text".
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXY_QUICK_UP_DOWN](#OXY_QUICK_UP_DOWN)
Class that marks root node when the quickUPDownNavigation option is on
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PRIORITY_BOOST](#PRIORITY_BOOST)
Class added to the document root and used in CSS in order to adjust the specificity of some rules.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SENTINEL](#SENTINEL)
Class used to identify sentinels.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SENTINEL_DISPLAY_PREFIX](#SENTINEL_DISPLAY_PREFIX)
Prefix for classes used to identify the type of the sentinel.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SENTINEL_MARKER](#SENTINEL_MARKER)
Class used to identify a marker that surrounds a sentinel.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SENTINEL_MARKER_DISPLAY_PREFIX](#SENTINEL_MARKER_DISPLAY_PREFIX)
Prefix for classes used to identify the type of the sentinel that a marker surrounds.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [START_SENTINEL_MARKER](#START_SENTINEL_MARKER)
Class used to identify a marker that surrounds a start sentinel.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [STATIC_CONTENT](#STATIC_CONTENT)
Class used to identify a piece of static content.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TABLE_CONTAINER](#TABLE_CONTAINER)
Class added to HTML elements that correspond to an XML table.

## Field Details

### MARKER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MARKER

Class used to identify elements that correspond to markers.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.MARKER)

### IMAGE_WRAPPER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) IMAGE_WRAPPER

Class used to identify wrapper elements used to style images for change tracking and comments.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.IMAGE_WRAPPER)

### DOCUMENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DOCUMENT

Class used to identify the document root.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.DOCUMENT)

### PRIORITY_BOOST

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PRIORITY_BOOST

Class added to the document root and used in CSS in order to adjust the specificity of some rules.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.PRIORITY_BOOST)

### SENTINEL_MARKER_DISPLAY_PREFIX

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SENTINEL_MARKER_DISPLAY_PREFIX

Prefix for classes used to identify the type of the sentinel that a marker surrounds.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.SENTINEL_MARKER_DISPLAY_PREFIX)

### SENTINEL_MARKER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SENTINEL_MARKER

Class used to identify a marker that surrounds a sentinel.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.SENTINEL_MARKER)

### IMAGE_MARKER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) IMAGE_MARKER

Class used to identify a marker that surrounds an image.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.IMAGE_MARKER)

### START_SENTINEL_MARKER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) START_SENTINEL_MARKER

Class used to identify a marker that surrounds a start sentinel.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.START_SENTINEL_MARKER)

### END_SENTINEL_MARKER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) END_SENTINEL_MARKER

Class used to identify a marker that surrounds an end sentinel.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.END_SENTINEL_MARKER)

### SENTINEL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SENTINEL

Class used to identify sentinels.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.SENTINEL)

### SENTINEL_DISPLAY_PREFIX

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SENTINEL_DISPLAY_PREFIX

Prefix for classes used to identify the type of the sentinel.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.SENTINEL_DISPLAY_PREFIX)

### EMPTY_PLACEHOLDER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EMPTY_PLACEHOLDER

Class used to identify the span generated as a placeholder in empty elements.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.EMPTY_PLACEHOLDER)

### STATIC_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) STATIC_CONTENT

Class used to identify a piece of static content.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.STATIC_CONTENT)

### LABEL

static final [CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html) LABEL

Class of oxy_label spans.

### LABEL_WIDTH_SPECIFIED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LABEL_WIDTH_SPECIFIED

Extra class for oxy_label spans which have a specified width.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.LABEL_WIDTH_SPECIFIED)

### OXY_COLLAPSE_TEXT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXY_COLLAPSE_TEXT

Class that marks nodes with "visibility: -oxy-collapse-text".
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.OXY_COLLAPSE_TEXT)

### OXY_QUICK_UP_DOWN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXY_QUICK_UP_DOWN

Class that marks root node when the quickUPDownNavigation option is on
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.OXY_QUICK_UP_DOWN)

### FOLDABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FOLDABLE

Class that marks foldable nodes.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.FOLDABLE)

### FOLDED_BY_DEFAULT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FOLDED_BY_DEFAULT

Class that marks folded nodes.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.FOLDED_BY_DEFAULT)

### TABLE_CONTAINER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TABLE_CONTAINER

Class added to HTML elements that correspond to an XML table. These elements are usually div-s and have an HTML <table> element as a child.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.TABLE_CONTAINER)

### GHOST_MARKER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) GHOST_MARKER

If a delete marker covers a sentinel, but not its pair the XML PI serialization does not cover the sentinel. In Author mode, we do not strike-through that sentinel. In the HTML rendering we do not render a span around that sentinel.

The only exception happens when a marker contains only such sentinels. These markers are called ghost markers because they are present in the markers model but are not serialized in XML.

 When we render the HTML, we generate a span for these markers and add this class to make sure that they will not show a visual strike-through.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.GHOST_MARKER)

### FILTERED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FILTERED

Marks content that is filtered by the active profiling conditions.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.FILTERED)

### MARKER_PSEUDO_ELEMENT_OUTSIDE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MARKER_PSEUDO_ELEMENT_OUTSIDE

Class added to CSS ::marker pseudo-elements that need to be rendered outside their parent.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.HTMLClasses.MARKER_PSEUDO_ELEMENT_OUTSIDE)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
