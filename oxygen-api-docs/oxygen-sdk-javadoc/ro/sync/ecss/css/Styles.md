Package [ro.sync.ecss.css](package-summary.md)

# Class Styles

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.css.Styles
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class Styles extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)
Represents the **computed** style properties for a particular element. These styles are taken from the CSS. See: http://www.w3.org/TR/CSS21/cascade.html#q1

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected static int [counter](#counter)
Constants counter
  static final float [EX_FACTOR](#EX_FACTOR)
This is the factor: ex-height / em-height The ex unit is defined by the font's x-height.
  static final int [FONT_WEIGHT_BOLD](#FONT_WEIGHT_BOLD)
Value for the "bold" in the font-weight propery.
  static final int [FONT_WEIGHT_NORMAL](#FONT_WEIGHT_NORMAL)
Value for the "normal" in the font-weight propery.
  static final int [KEY_ALIGNMENT_BASELINE](#KEY_ALIGNMENT_BASELINE)
Property for CSS media paged, the alignment relative to the baseline.
  static final int [KEY_BACKGROUND_COLOR](#KEY_BACKGROUND_COLOR)
Background color.
  static final int [KEY_BACKGROUND_IMAGE](#KEY_BACKGROUND_IMAGE)
Key used to store the property 'background-image' value.
  static final int [KEY_BACKGROUND_POSITION](#KEY_BACKGROUND_POSITION)
Key used to store the property 'background-position' value.
  static final int [KEY_BACKGROUND_REPEAT](#KEY_BACKGROUND_REPEAT)
Key used to store the property 'background-repeat' value.
  static final int [KEY_BACKGROUND_SIZE](#KEY_BACKGROUND_SIZE)
Key used to store the property 'background-size' value.
  static final int [KEY_BOOKMARK_LABEL](#KEY_BOOKMARK_LABEL)
Bookmark label.
  static final int [KEY_BOOKMARK_LEVEL](#KEY_BOOKMARK_LEVEL)
Bookmark level.
  static final int [KEY_BOOKMARK_STATE](#KEY_BOOKMARK_STATE)
Bookmark state.
  static final int [KEY_BORDER_BOTTOM_COLOR](#KEY_BORDER_BOTTOM_COLOR)
Border bottom color
  static final int [KEY_BORDER_BOTTOM_LEFT_RADIUS](#KEY_BORDER_BOTTOM_LEFT_RADIUS)
border-bottom-left-radius.
  static final int [KEY_BORDER_BOTTOM_RIGHT_RADIUS](#KEY_BORDER_BOTTOM_RIGHT_RADIUS)
border-bottom-right-radius.
  static final int [KEY_BORDER_BOTTOM_STYLE](#KEY_BORDER_BOTTOM_STYLE)
Border bottom style
  static final int [KEY_BORDER_BOTTOM_WIDTH](#KEY_BORDER_BOTTOM_WIDTH)
Border bottom width
  static final int [KEY_BORDER_COLLAPSE](#KEY_BORDER_COLLAPSE)
This property selects a table's border model.
  static final int [KEY_BORDER_LEFT_COLOR](#KEY_BORDER_LEFT_COLOR)
Border left color
  static final int [KEY_BORDER_LEFT_STYLE](#KEY_BORDER_LEFT_STYLE)
Border right style
  static final int [KEY_BORDER_LEFT_WIDTH](#KEY_BORDER_LEFT_WIDTH)
Border left width
  static final int [KEY_BORDER_RIGHT_COLOR](#KEY_BORDER_RIGHT_COLOR)
Border right color
  static final int [KEY_BORDER_RIGHT_STYLE](#KEY_BORDER_RIGHT_STYLE)
Border right style
  static final int [KEY_BORDER_RIGHT_WIDTH](#KEY_BORDER_RIGHT_WIDTH)
Border right width
  static final int [KEY_BORDER_SPACING](#KEY_BORDER_SPACING)
Key for the border spacing array
  static final int [KEY_BORDER_TOP_COLOR](#KEY_BORDER_TOP_COLOR)
Border top color
  static final int [KEY_BORDER_TOP_LEFT_RADIUS](#KEY_BORDER_TOP_LEFT_RADIUS)
border-top-left-radius.
  static final int [KEY_BORDER_TOP_RIGHT_RADIUS](#KEY_BORDER_TOP_RIGHT_RADIUS)
border-top-right-radius.
  static final int [KEY_BORDER_TOP_STYLE](#KEY_BORDER_TOP_STYLE)
Border top style
  static final int [KEY_BORDER_TOP_WIDTH](#KEY_BORDER_TOP_WIDTH)
Border top width
  static final int [KEY_BOTTOM](#KEY_BOTTOM)
The 'bottom' property.
  static final int [KEY_BREAK_AFTER](#KEY_BREAK_AFTER)
Property for CSS media paged, signal the break policy that applies
  static final int [KEY_BREAK_BEFORE](#KEY_BREAK_BEFORE)
Property for CSS media paged, signal the break policy that applies
  static final int [KEY_BREAK_INSIDE](#KEY_BREAK_INSIDE)
Property for CSS media paged, signal the break policy that applies
  static final int [KEY_CAPTION_SIDE](#KEY_CAPTION_SIDE)
Property for CSS caption-side property.
  static final int [KEY_COLUMN_SPAN](#KEY_COLUMN_SPAN)
Specify how an element can span over a multiple column layout.
  static final int [KEY_COUNTER_INCREMENT](#KEY_COUNTER_INCREMENT)
The key for counter-increment .
  static final int [KEY_COUNTER_RESET](#KEY_COUNTER_RESET)
The key for counter-reset .
  static final int [KEY_DIRECT_WHITESPACE](#KEY_DIRECT_WHITESPACE)
Whitespace specified directly on the node, not inherited.
  static final int [KEY_DIRECTION](#KEY_DIRECTION)
Key used to store the property 'direction' value.
  static final int [KEY_DISPLAY](#KEY_DISPLAY)
Display type
  static final int [KEY_DISPLAY_TAGS](#KEY_DISPLAY_TAGS)
Key used to hide sentinel markers.
  static final int [KEY_EDITABLE](#KEY_EDITABLE)
True if this view is editable
  static final int [KEY_EMPTY_CELLS](#KEY_EMPTY_CELLS)
Key used to store the property 'empty-cells' value as string.
  static final int [KEY_EMPTY_CELLS_BOOLEAN](#KEY_EMPTY_CELLS_BOOLEAN)
Key used to store the property 'empty-cells' value as boolean.
  static final int [KEY_FILTERED_OUT](#KEY_FILTERED_OUT)
Key set for filtered out nodes.
  static final int [KEY_FLOAT](#KEY_FLOAT)
Property for CSS media paged "float".
  static final int [KEY_FOLDABLE](#KEY_FOLDABLE)
Key used to store the property 'foldable' value.
  static final int [KEY_FOLDED](#KEY_FOLDED)
Key used to store the property 'folded' value.
  static final int [KEY_FONT](#KEY_FONT)
Used font
  static final int [KEY_FONT_FAMILY](#KEY_FONT_FAMILY)
Font family.
  static final int [KEY_FONT_SIZE](#KEY_FONT_SIZE)
Font size.
  static final int [KEY_FONT_STYLE](#KEY_FONT_STYLE)
Font style.
  static final int [KEY_FONT_VARIANT](#KEY_FONT_VARIANT)
Font variant
  static final int [KEY_FONT_VARIANT_ALTERNATES](#KEY_FONT_VARIANT_ALTERNATES)
Font variant alternates.
  static final int [KEY_FONT_VARIANT_LIGATURES](#KEY_FONT_VARIANT_LIGATURES)
Font variant ligatures.
  static final int [KEY_FONT_VARIANT_NUMERIC](#KEY_FONT_VARIANT_NUMERIC)
Font variant numeric.
  static final int [KEY_FONT_WEIGHT](#KEY_FONT_WEIGHT)
Font weight
  static final int [KEY_FOREGROUND_COLOR](#KEY_FOREGROUND_COLOR)
Foreground
  static final int [KEY_HEIGHT](#KEY_HEIGHT)
Height.
  static final int [KEY_HYPHENS](#KEY_HYPHENS)
This property controls whether hyphenation is allowed to create more soft wrap opportunities within a line of text.
  static final int [KEY_IMAGE_RESOLUTION](#KEY_IMAGE_RESOLUTION)
Key used to specify the image DPI.
  static final int [KEY_IMPOSED_DISPLAY](#KEY_IMPOSED_DISPLAY)
Key used to override the display property defined in the css.
  static final int [KEY_LEFT](#KEY_LEFT)
The 'left' property.
  static final int [KEY_LETTER_SPACING](#KEY_LETTER_SPACING)
Font letter spacing.
  static final int [KEY_LINE_HEIGHT](#KEY_LINE_HEIGHT)
If it is a float, it means a line height multiplier, which is relative to the current font, and was specified as a number without metric or a percent.
  static final int [KEY_LINK](#KEY_LINK)
Key used to store the URL for link elements.
  static final int [KEY_LINK_URL](#KEY_LINK_URL)  Deprecated.
since 17
   static final int [KEY_LIST_STYLE_IMAGE](#KEY_LIST_STYLE_IMAGE)
List style image
  static final int [KEY_LIST_STYLE_POSITION](#KEY_LIST_STYLE_POSITION)
List style position
  static final int [KEY_LIST_STYLE_TYPE](#KEY_LIST_STYLE_TYPE)
List style type
  static final int [KEY_MARGIN_BOTTOM](#KEY_MARGIN_BOTTOM)
Margin dimensions
  static final int [KEY_MARGIN_LEFT](#KEY_MARGIN_LEFT)
Margin left
  static final int [KEY_MARGIN_RIGHT](#KEY_MARGIN_RIGHT)
Margin right
  static final int [KEY_MARGIN_TOP](#KEY_MARGIN_TOP)
Margin top
  static final int [KEY_MAX_HEIGHT](#KEY_MAX_HEIGHT)
Maximum height.
  static final int [KEY_MAX_WIDTH](#KEY_MAX_WIDTH)
Maximum width.
  static final int [KEY_MIN_HEIGHT](#KEY_MIN_HEIGHT)
Minimum height.
  static final int [KEY_MIN_WIDTH](#KEY_MIN_WIDTH)
Minimum width.
  static final int [KEY_MIXED_CONTENT](#KEY_MIXED_CONTENT)
Generated mixed Content property key.
  static final int [KEY_NON_FOLDABLE_CHILD_NAME](#KEY_NON_FOLDABLE_CHILD_NAME)
Key used to store the property 'non foldable child name' value.
  static final int [KEY_ORPHANS](#KEY_ORPHANS)
Property for CSS media paged "orphans".
  static final int [KEY_OUTLINE_COLOR](#KEY_OUTLINE_COLOR)
Outline color
  static final int [KEY_OUTLINE_STYLE](#KEY_OUTLINE_STYLE)
Outline style
  static final int [KEY_OUTLINE_WIDTH](#KEY_OUTLINE_WIDTH)
Outline width
  static final int [KEY_OVERFLOW_WRAP](#KEY_OVERFLOW_WRAP)
Overflow wrap.
  static final int [KEY_OXY_ALT_TEXT](#KEY_OXY_ALT_TEXT)
Key used to specify the accessibility alternate text.
  static final int [KEY_OXY_AVOID_BREAKING_LINE_AT_HYPHENS](#KEY_OXY_AVOID_BREAKING_LINE_AT_HYPHENS)
Controls the line breaking status for hyphens.
  static final int [KEY_OXY_BORDERS_CONDITIONALITY](#KEY_OXY_BORDERS_CONDITIONALITY)
Property for -oxy-borders-conditionality which allow borders on line breaks.
  static final int [KEY_OXY_BREAK_LINE_AT_HYPHENS](#KEY_OXY_BREAK_LINE_AT_HYPHENS)
Controls the line breaking status for hyphens.
  static final int [KEY_OXY_CAPTION_REPEAT_ON_NEXT_PAGES](#KEY_OXY_CAPTION_REPEAT_ON_NEXT_PAGES)
Property enabling the table caption repetition on next pages (When the table is long and it spans multiple pages).
  static final int [KEY_OXY_CHANGEBAR_COLOR](#KEY_OXY_CHANGEBAR_COLOR)
Property for -oxy-changebar-color, set the changebar color.
  static final int [KEY_OXY_CHANGEBAR_OFFSET](#KEY_OXY_CHANGEBAR_OFFSET)
Property for -oxy-changebar-offset, set the distance from the column edge.
  static final int [KEY_OXY_CHANGEBAR_PLACEMENT](#KEY_OXY_CHANGEBAR_PLACEMENT)
Property for -oxy-changebar-placement, set the changebar position.
  static final int [KEY_OXY_CHANGEBAR_STYLE](#KEY_OXY_CHANGEBAR_STYLE)
Property for -oxy-changebar-style, set how the change bar appears.
  static final int [KEY_OXY_CHANGEBAR_WIDTH](#KEY_OXY_CHANGEBAR_WIDTH)
Property for -oxy-changebar-width, set the changebar color.
  static final int [KEY_OXY_COLUMN_BREAK_AFTER](#KEY_OXY_COLUMN_BREAK_AFTER)
Property for CSS media paged, signals the column break policy that applies.
  static final int [KEY_OXY_COLUMN_BREAK_BEFORE](#KEY_OXY_COLUMN_BREAK_BEFORE)
Property for CSS media paged, signals the column break policy that applies.
  static final int [KEY_OXY_COLUMN_BREAK_INSIDE](#KEY_OXY_COLUMN_BREAK_INSIDE)
Property for CSS media paged, signals the column break policy that applies.
  static final int [KEY_OXY_FLOATING_TOOLBAR](#KEY_OXY_FLOATING_TOOLBAR)
Key used to store the property -oxy-floating-toolbar.
  static final int [KEY_OXY_FOREGROUND_IMAGE](#KEY_OXY_FOREGROUND_IMAGE)
Key used to store the property '-oxy-foreground-image' value.
  static final int [KEY_OXY_HYPHENATION_CHARACTER](#KEY_OXY_HYPHENATION_CHARACTER)
An oxygen extension, mostly used to hide the hyphen characters.
  static final int [KEY_OXY_HYPHENATION_PUSH_CHARACTER_COUNT](#KEY_OXY_HYPHENATION_PUSH_CHARACTER_COUNT)
The minimum number of characters in a hyphenated word after the hyphenation character.
  static final int [KEY_OXY_HYPHENATION_REMAIN_CHARACTER_COUNT](#KEY_OXY_HYPHENATION_REMAIN_CHARACTER_COUNT)
The hyphenation-remain-character-count specifies the minimum number of characters in a hyphenated word before the hyphenation character.
  static final int [KEY_OXY_LINK_ACTIVATION_TRIGGER](#KEY_OXY_LINK_ACTIVATION_TRIGGER)
Key used to store the property '-oxy-link-activation-trigger' value.
  static final int [KEY_OXY_PAGE_GROUP](#KEY_OXY_PAGE_GROUP)
The oxy-page-group property.
  static final int [KEY_OXY_PDF_EXTRACT_FILE](#KEY_OXY_PDF_EXTRACT_FILE)
A pointer for fragments to be extracted as PDF.
  static final int [KEY_OXY_PDF_META_AUTHOR](#KEY_OXY_PDF_META_AUTHOR)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_COPYRIGHT](#KEY_OXY_PDF_META_COPYRIGHT)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_COPYRIGHT_URL](#KEY_OXY_PDF_META_COPYRIGHT_URL)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_COPYRIGHTED](#KEY_OXY_PDF_META_COPYRIGHTED)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_CUSTOM](#KEY_OXY_PDF_META_CUSTOM)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_DESCRIPTION](#KEY_OXY_PDF_META_DESCRIPTION)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_KEYWORD](#KEY_OXY_PDF_META_KEYWORD)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_KEYWORDS](#KEY_OXY_PDF_META_KEYWORDS)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_META_TITLE](#KEY_OXY_PDF_META_TITLE)
Key used for PDF metadata.
  static final int [KEY_OXY_PDF_TABLE_OMIT_FOOTER_BREAK](#KEY_OXY_PDF_TABLE_OMIT_FOOTER_BREAK)
A flag specifying if the footer of a table should be omitted at break.
  static final int [KEY_OXY_PDF_TABLE_OMIT_HEADER_BREAK](#KEY_OXY_PDF_TABLE_OMIT_HEADER_BREAK)
A flag specifying if the header of a table should be omitted at break.
  static final int [KEY_OXY_PDF_TAG_TYPE](#KEY_OXY_PDF_TAG_TYPE)
Key used to specify the accessibility PDF tag.
  static final int [KEY_OXY_PDF_VIEWER_DISPLAY_FILENAME](#KEY_OXY_PDF_VIEWER_DISPLAY_FILENAME)
A flag specifying if the doc title should be displayed.
  static final int [KEY_OXY_PDF_VIEWER_FIT_WINDOW](#KEY_OXY_PDF_VIEWER_FIT_WINDOW)
A flag specifying whether to resize the documentï¿½s window to fit the size of the first displayed page.
  static final int [KEY_OXY_PDF_VIEWER_HIDE_MENUBAR](#KEY_OXY_PDF_VIEWER_HIDE_MENUBAR)
If the viewer menubar should be visible or not.
  static final int [KEY_OXY_PDF_VIEWER_HIDE_TOOLBAR](#KEY_OXY_PDF_VIEWER_HIDE_TOOLBAR)
If the viewer toolbarshould be visible or not.
  static final int [KEY_OXY_PDF_VIEWER_PAGE_LAYOUT](#KEY_OXY_PDF_VIEWER_PAGE_LAYOUT)
A name object specifying the page layout shall be used when the document is opened: single-page Display one page at a time one-column Display the pages in one column two-column-left Display the pages in two columns, with odd- numbered pages on the left two-column-right Display the pages in two columns, with odd- numbered pages on the right
  static final int [KEY_OXY_PDF_VIEWER_PAGE_MODE](#KEY_OXY_PDF_VIEWER_PAGE_MODE)
A name object specifying how the document shall be displayed when opened: none Neither document outline nor thumbnail images visible use-outlines Document outline visible use-thumbs Thumbnail images visible full-screen Full-screen mode, with no menu bar, window controls, or any other window visible
  static final int [KEY_OXY_PDF_VIEWER_ZOOM](#KEY_OXY_PDF_VIEWER_ZOOM)
The zoom factor applied to the viewport when the PDF document is loaded.
  static final int [KEY_OXY_SHOW_ONLY_WHEN_CAPTION_REPEATED_ON_NEXT_PAGES](#KEY_OXY_SHOW_ONLY_WHEN_CAPTION_REPEATED_ON_NEXT_PAGES)
Property that marks a pseudo :before or :after that is associated to a table caption.
  static final int [KEY_OXY_SPACE_AFTER_CONDITIONALITY](#KEY_OXY_SPACE_AFTER_CONDITIONALITY)
Property for -oxy-space-after-conditionality which allow margin-bottom drop on elements.
  static final int [KEY_OXY_SPACE_BEFORE_CONDITIONALITY](#KEY_OXY_SPACE_BEFORE_CONDITIONALITY)
Property for-oxy-space-before-conditionality which allow margin-top drop on elements.
  static final int [KEY_OXY_STYLE](#KEY_OXY_STYLE)
The -oxy-style property that defines additional styles.
  static final int [KEY_OXY_VIDEO_COVER](#KEY_OXY_VIDEO_COVER)
Key used to store the property '-oxy-video-cover' value.
  static final int [KEY_PADDING_BOTTOM](#KEY_PADDING_BOTTOM)
Padding dimensions
  static final int [KEY_PADDING_LEFT](#KEY_PADDING_LEFT)
Pad left
  static final int [KEY_PADDING_RIGHT](#KEY_PADDING_RIGHT)
Pad right
  static final int [KEY_PADDING_TOP](#KEY_PADDING_TOP)
Pad top
  static final int [KEY_PAGE](#KEY_PAGE)
The CSS page - for media print.
  static final int [KEY_PAGE_BREAK_AFTER](#KEY_PAGE_BREAK_AFTER)
Property for CSS media paged, signals the page break policy that applies.
  static final int [KEY_PAGE_BREAK_BEFORE](#KEY_PAGE_BREAK_BEFORE)
Property for CSS media paged, signals the page break policy that applies.
  static final int [KEY_PAGE_BREAK_INSIDE](#KEY_PAGE_BREAK_INSIDE)
Property for CSS media paged, signals the page break policy that applies.
  static final int [KEY_PLACEHOLDER_CONTENT](#KEY_PLACEHOLDER_CONTENT)
Key used to store the property 'placeholder-content' value.
  static final int [KEY_POSITION](#KEY_POSITION)
The 'position' property.
  static final int [KEY_RIGHT](#KEY_RIGHT)
The 'right' property.
  static final int [KEY_SHOW_PLACEHOLDER](#KEY_SHOW_PLACEHOLDER)
Key used to store the property 'show-placeholder' value.
  static final int [KEY_STRING_SET](#KEY_STRING_SET)
Property for CSS media paged "string-set".
  static final int [KEY_TABLE_COLUMN_SPAN](#KEY_TABLE_COLUMN_SPAN)
CSS property taken into account to compute the column spanning of a table cell.
  static final int [KEY_TABLE_LAYOUT](#KEY_TABLE_LAYOUT)
The 'table-layout' property controls the algorithm used to lay out the table cells, rows, and columns.
  static final int [KEY_TABLE_ROW_SPAN](#KEY_TABLE_ROW_SPAN)
CSS property taken into account to compute the row spanning of a table cell.
  static final int [KEY_TAGS_BACKGROUND_COLOR](#KEY_TAGS_BACKGROUND_COLOR)
Key used to store the property '-oxy-tags-background-color' value.
  static final int [KEY_TAGS_COLOR](#KEY_TAGS_COLOR)
Key used to store the property '-oxy-tags-color' value.
  static final int [KEY_TEXT_ALIGN](#KEY_TEXT_ALIGN)
Text align
  static final int [KEY_TEXT_DECORATION](#KEY_TEXT_DECORATION)  Deprecated.
It is a shorthand now, use [KEY_TEXT_DECORATION_LINE](#KEY_TEXT_DECORATION_LINE), [KEY_TEXT_DECORATION_COLOR](#KEY_TEXT_DECORATION_COLOR), [KEY_TEXT_DECORATION_STYLE](#KEY_TEXT_DECORATION_STYLE) instead.
   static final int [KEY_TEXT_DECORATION_COLOR](#KEY_TEXT_DECORATION_COLOR)
Key used to store color for text decoration.
  static final int [KEY_TEXT_DECORATION_LINE](#KEY_TEXT_DECORATION_LINE)
Key used to store 'text-decoration-line' property.
  static final int [KEY_TEXT_DECORATION_STYLE](#KEY_TEXT_DECORATION_STYLE)
Key used to store 'text-decoration' property.
  static final int [KEY_TEXT_INDENT](#KEY_TEXT_INDENT)
Text indent
  static final int [KEY_TEXT_TRANSFORM](#KEY_TEXT_TRANSFORM)
Text transform
  static final int [KEY_TOP](#KEY_TOP)
The 'top' property.
  static final int [KEY_TRANSFORM_ROTATION](#KEY_TRANSFORM_ROTATION)
Specify that the element can have a different rotation than the parent.
  static final int [KEY_UNICODE_BIDI](#KEY_UNICODE_BIDI)
Key used to store the property 'unicode-bidi' value.
  static final int [KEY_VERTICAL_ALIGN](#KEY_VERTICAL_ALIGN)
Key for vertical align.
  static final int [KEY_VISIBILITY](#KEY_VISIBILITY)
Key for the 'visibility' property.
  static final int [KEY_VISIBITY](#KEY_VISIBITY)  Deprecated.
This is a typo of the [KEY_VISIBILITY](#KEY_VISIBILITY).
   static final int [KEY_WHITESPACE](#KEY_WHITESPACE)
Whitespace
  static final int [KEY_WIDOWS](#KEY_WIDOWS)
Property for CSS media paged "widows".
  static final int [KEY_WIDTH](#KEY_WIDTH)
Width.
  protected static int [pmCounter](#pmCounter)
All the properties before this counter are for media screen.
  protected final [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] [stylesArray](#stylesArray)
The styles map

## Constructor Summary
 Constructors
Constructor

Description
 [Styles](#%3Cinit%3E())()
Constructor.
  [Styles](#%3Cinit%3E(boolean))(boolean enablePagedMediaProperties)
Constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 boolean [affectsCounters](#affectsCounters())()
Checks if the styles increment or reset some of the counters.
  boolean [canBeCached](#canBeCached())()
Verify if styles can be cached.
  [Styles](Styles.md) [clone](#clone())()
Shallow clone.
  boolean [dependsOnTargetCounter](#dependsOnTargetCounter())()
Checks if the style defines some static content using the target-counter or target-counters CSS function.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAlignmentBaseline](#getAlignmentBaseline())()

 [Color](../../exml/view/graphics/Color.md) [getBackgroundColor](#getBackgroundColor())()

 [URIContent](URIContent.md) [getBackgroundImage](#getBackgroundImage())()
This property sets the background image of an element.
  ro.sync.ecss.css.BackgroundPosition [getBackgroundPosition](#getBackgroundPosition())()
If a background position is specified, this property indicates the position of the background image relative to its box.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getBackgroundRepeat](#getBackgroundRepeat())()
If a background image is specified, this property specifies whether the image is repeated (tiled), and how.
  [Color](../../exml/view/graphics/Color.md) [getBorderBottomColor](#getBorderBottomColor())()

 [RelativeLength](RelativeLength.md) [getBorderBottomLeftRadius](#getBorderBottomLeftRadius())()

 [RelativeLength](RelativeLength.md) [getBorderBottomRightRadius](#getBorderBottomRightRadius())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getBorderBottomStyle](#getBorderBottomStyle())()

 int [getBorderBottomWidth](#getBorderBottomWidth())()

 [Color](../../exml/view/graphics/Color.md) [getBorderLeftColor](#getBorderLeftColor())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getBorderLeftStyle](#getBorderLeftStyle())()

 int [getBorderLeftWidth](#getBorderLeftWidth())()

 [Color](../../exml/view/graphics/Color.md) [getBorderRightColor](#getBorderRightColor())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getBorderRightStyle](#getBorderRightStyle())()

 int [getBorderRightWidth](#getBorderRightWidth())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getBordersConditionality](#getBordersConditionality())()

 [Color](../../exml/view/graphics/Color.md) [getBorderTopColor](#getBorderTopColor())()

 [RelativeLength](RelativeLength.md) [getBorderTopLeftRadius](#getBorderTopLeftRadius())()

 [RelativeLength](RelativeLength.md) [getBorderTopRightRadius](#getBorderTopRightRadius())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getBorderTopStyle](#getBorderTopStyle())()

 int [getBorderTopWidth](#getBorderTopWidth())()

 [RelativeLength](RelativeLength.md) [getBottom](#getBottom())()

 [Color](../../exml/view/graphics/Color.md) [getColor](#getColor())()

 [CSSCounter](CSSCounter.md)[] [getCounters](#getCounters())()

 [CSSCounterIncrement](CSSCounterIncrement.md)[] [getCountersIncrement](#getCountersIncrement())()

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.css.functions.customprop.CustomPropertyValue> [getCustomCssProperties](#getCustomCssProperties())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDirection](#getDirection())()
The direction CSS property should be set to match the direction of the text: rtl for Hebrew or Arabic text and ltr for other scripts.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDirectWhitespace](#getDirectWhitespace())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplay](#getDisplay())()
First it looks at the KEY_IMPOSED_DISPLAY property.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayTags](#getDisplayTags())()

 [Font](../../exml/view/graphics/Font.md) [getFont](#getFont())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFontVariant](#getFontVariant())()
Gets the font-variant.
  int [getFontWeight](#getFontWeight())()

 [RelativeLength](RelativeLength.md) [getHeight](#getHeight())()

 int [getHorizontalBorderSpacing](#getHorizontalBorderSpacing())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHyperlinkActivationType](#getHyperlinkActivationType())()

 [RelativeLength](RelativeLength.md) [getLeft](#getLeft())()

 org.w3c.css.sac.LexicalUnit [getLexicalUnit](#getLexicalUnit(int))(int key)
Gets a lexical unit.
  int [getLineHeight](#getLineHeight(ro.sync.exml.view.graphics.FontMetrics))([FontMetrics](../../exml/view/graphics/FontMetrics.md) fm)
Sets the distance between lines: normal number length %
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLinkURL](#getLinkURL())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getListStylePosition](#getListStylePosition())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getListStyleType](#getListStyleType())()

 [RelativeLength](RelativeLength.md) [getMarginBottom](#getMarginBottom())()

 [RelativeLength](RelativeLength.md) [getMarginLeft](#getMarginLeft())()

 [RelativeLength](RelativeLength.md) [getMarginRight](#getMarginRight())()

 [RelativeLength](RelativeLength.md) [getMarginTop](#getMarginTop())()

 [RelativeLength](RelativeLength.md) [getMaxWidth](#getMaxWidth())()

 [RelativeLength](RelativeLength.md) [getMinHeight](#getMinHeight())()
Gets the value associated with the min-height property
  [RelativeLength](RelativeLength.md) [getMinWidth](#getMinWidth())()

 [StaticContent](StaticContent.md)[] [getMixedContent](#getMixedContent())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNonFoldableChildName](#getNonFoldableChildName())()

 [Color](../../exml/view/graphics/Color.md) [getOutlineColor](#getOutlineColor())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOutlineStyle](#getOutlineStyle())()

 int [getOutlineWidth](#getOutlineWidth())()

 [RelativeLength](RelativeLength.md) [getPaddingBottom](#getPaddingBottom())()

 [RelativeLength](RelativeLength.md) [getPaddingLeft](#getPaddingLeft())()

 [RelativeLength](RelativeLength.md) [getPaddingRight](#getPaddingRight())()

 [RelativeLength](RelativeLength.md) [getPaddingTop](#getPaddingTop())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPlaceholderContent](#getPlaceholderContent())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPosition](#getPosition())()
Checks the 'position' property.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getProperty](#getProperty(int))(int property)

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getPropertyByName](#getPropertyByName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Retrieve the property by its name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPropertyName](#getPropertyName(int))(int index)

 int [getPseudoLevel](#getPseudoLevel())()
If this is the style for a pseudo element, get its level.
  int [getRecognizedPropertiesNumber](#getRecognizedPropertiesNumber())()
Use this to get the number of recognized properties.
  [RelativeLength](RelativeLength.md) [getRight](#getRight())()

 boolean [getShowEmptyCells](#getShowEmptyCells())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getShowPlaceholders](#getShowPlaceholders())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSpaceAfterConditionality](#getSpaceAfterConditionality())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSpaceBeforeConditionality](#getSpaceBeforeConditionality())()

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[StaticContent](StaticContent.md)[]> [getStringSet](#getStringSet())()
The string-set property contains one or more pairs, each consisting of an custom identifier (the name of the named string) followed by a content-list describing how to construct the value of the named string.
  int [getTableColumnSpan](#getTableColumnSpan())()
Gets the 'table-column-span' property value.
  int [getTableRowSpan](#getTableRowSpan())()
Gets the 'table-row-span' property value.
  [Color](../../exml/view/graphics/Color.md) [getTagsBackgroundColor](#getTagsBackgroundColor())()
Obtain the color for full-tags background.
  [Color](../../exml/view/graphics/Color.md) [getTagsColor](#getTagsColor())()
Obtain the color for full-tags background.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTextAlign](#getTextAlign())()
Aligns the text in an element: left right center justify.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTextDecoration](#getTextDecoration())()  Deprecated.
This was used to return only the text-decoration-line part from the text-decoration shorthand, as defined here https://drafts.csswg.org/css-text-decor-3/#text-decoration-property.
   [Color](../../exml/view/graphics/Color.md) [getTextDecorationColor](#getTextDecorationColor())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getTextDecorationLine](#getTextDecorationLine())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTextDecorationStyle](#getTextDecorationStyle())()

 [RelativeLength](RelativeLength.md) [getTextIndent](#getTextIndent())()
Gets the horizontal space that should be left before the beginning of the first line of the text content of an element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTextTransform](#getTextTransform())()

 [RelativeLength](RelativeLength.md) [getTop](#getTop())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getUnicodeBIDI](#getUnicodeBIDI())()
The unicode-bidi CSS property together with the direction property relates to the handling of bidirectional text in a document.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getVerticalAlign](#getVerticalAlign())()

 int [getVerticalBorderSpacing](#getVerticalBorderSpacing())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getVisibility](#getVisibility())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getWhitespace](#getWhitespace())()

 [RelativeLength](RelativeLength.md) [getWidth](#getWidth())()

 boolean [hasBorder](#hasBorder())()

 int [hashCode](#hashCode())()

 boolean [isChangebarDisplay](#isChangebarDisplay())()
Check if the display has '-oxy-change-bar-start' or '-oxy-change-bar-end' value.
  boolean [isEditable](#isEditable())()

 boolean [isEnablePagedMediaProperties](#isEnablePagedMediaProperties())()

 boolean [isFilteredOut](#isFilteredOut())()

 boolean [isFoldable](#isFoldable())()

 boolean [isFolded](#isFolded())()

 static boolean [isInheritable](#isInheritable(int))(int property)
Check if the given property should be copied from parent to child.
  static boolean [isInheritable](#isInheritable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property)
Check if the given property can be inherited from parent to child.
  boolean [isInline](#isInline())()
Gets the imposed display - it may be the same as the one specified in the CSS - and checks if it is inline or inline block.
  boolean [isInlineBlockInCSS](#isInlineBlockInCSS())()

 boolean [isInlineInCSS](#isInlineInCSS())()

 boolean [isInTable](#isInTable())()
Check if is a style from a table but not a cell.
  boolean [isInvisible](#isInvisible())()

 boolean [isListItem](#isListItem())()

 boolean [isMorphDisplay](#isMorphDisplay())()
Check if the display has 'morph' or '-oxy-morph' value.
  boolean [isSpecifiedTextAlign](#isSpecifiedTextAlign())()
Checks if the text-align property from the current element styles has a value specified by the CSS.
  boolean [isTable](#isTable())()
Checks if the display mode indicated to be a table.
  boolean [isTableCaption](#isTableCaption())()
Checks if the display mode indicated to be a table caption.
  boolean [isTableCell](#isTableCell())()
Checks if the display mode indicated to be a table cell.
  boolean [isTableColumn](#isTableColumn())()
Checks if the display mode indicated to be a table column.
  boolean [isTableColumnGroup](#isTableColumnGroup())()
Checks if the display mode indicated to be a table group of columns.
  boolean [isTableFooterGroup](#isTableFooterGroup())()
Checks if the display mode indicated to be a table group footer.
  boolean [isTableHeaderGroup](#isTableHeaderGroup())()
Checks if the display mode indicated to be a table group header.
  boolean [isTableRow](#isTableRow())()

 boolean [isTableRowGroup](#isTableRowGroup())()

 void [setCanBeCached](#setCanBeCached(boolean))(boolean canBeCached)
Sets if those styles can be shared between two or more nodes.
  void [setCustomProperty](#setCustomProperty(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.css.functions.customprop.CustomPropertyValue> props)
Sets the list of custom CSS properties and their values.
  void [setProperty](#setProperty(int,java.lang.Object))(int property, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)
Set a property to the map.
  void [setProperty](#setProperty(int,java.lang.Object,org.w3c.css.sac.LexicalUnit))(int property, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value, org.w3c.css.sac.LexicalUnit lu)
Set a property to the map.
  void [setPseudoLevel](#setPseudoLevel(int))(int pseudoLevel)
If this is the style for a pseudo element, keep here its level.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### EX_FACTOR

public static final float EX_FACTOR

This is the factor: ex-height / em-height The ex unit is defined by the font's x-height. The x-height is so called because it is often equal to the height of the lowercase "x". However, an ex is defined even for fonts that don't contain an "x".
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.Styles.EX_FACTOR)

### FONT_WEIGHT_NORMAL

public static final int FONT_WEIGHT_NORMAL

Value for the "normal" in the font-weight propery. Spec: normal Same as '400'.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.Styles.FONT_WEIGHT_NORMAL)

### FONT_WEIGHT_BOLD

public static final int FONT_WEIGHT_BOLD

Value for the "bold" in the font-weight propery. Spec: normal Same as '700'.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.css.Styles.FONT_WEIGHT_BOLD)

### counter

protected static int counter

Constants counter

### KEY_BACKGROUND_COLOR

public static final int KEY_BACKGROUND_COLOR

Background color.

### KEY_BORDER_BOTTOM_COLOR

public static final int KEY_BORDER_BOTTOM_COLOR

Border bottom color

### KEY_BORDER_BOTTOM_STYLE

public static final int KEY_BORDER_BOTTOM_STYLE

Border bottom style

### KEY_BORDER_BOTTOM_WIDTH

public static final int KEY_BORDER_BOTTOM_WIDTH

Border bottom width

### KEY_BORDER_LEFT_COLOR

public static final int KEY_BORDER_LEFT_COLOR

Border left color

### KEY_BORDER_LEFT_STYLE

public static final int KEY_BORDER_LEFT_STYLE

Border right style

### KEY_BORDER_LEFT_WIDTH

public static final int KEY_BORDER_LEFT_WIDTH

Border left width

### KEY_BORDER_RIGHT_COLOR

public static final int KEY_BORDER_RIGHT_COLOR

Border right color

### KEY_BORDER_RIGHT_STYLE

public static final int KEY_BORDER_RIGHT_STYLE

Border right style

### KEY_BORDER_RIGHT_WIDTH

public static final int KEY_BORDER_RIGHT_WIDTH

Border right width

### KEY_BORDER_TOP_COLOR

public static final int KEY_BORDER_TOP_COLOR

Border top color

### KEY_BORDER_TOP_STYLE

public static final int KEY_BORDER_TOP_STYLE

Border top style

### KEY_BORDER_TOP_WIDTH

public static final int KEY_BORDER_TOP_WIDTH

Border top width

### KEY_FOREGROUND_COLOR

public static final int KEY_FOREGROUND_COLOR

Foreground

### KEY_MIXED_CONTENT

public static final int KEY_MIXED_CONTENT

Generated mixed Content property key. The value set for this property must be an array of instances of the [StaticContent](StaticContent.md) interface. For example: new [StaticContent](StaticContent.md)[] { new [StringContent](StringContent.md)("Text value for the KEY_MIXED_CONTENT property") }

### KEY_DISPLAY

public static final int KEY_DISPLAY

Display type

### KEY_FONT

public static final int KEY_FONT

Used font

### KEY_FONT_WEIGHT

public static final int KEY_FONT_WEIGHT

Font weight

### KEY_LINE_HEIGHT

public static final int KEY_LINE_HEIGHT

If it is a float, it means a line height multiplier, which is relative to the current font, and was specified as a number without metric or a percent. If it is an integer, is a fixed value, specified using em, pt, ex, px, etc..

### KEY_LIST_STYLE_TYPE

public static final int KEY_LIST_STYLE_TYPE

List style type

### KEY_LIST_STYLE_POSITION

public static final int KEY_LIST_STYLE_POSITION

List style position

### KEY_MARGIN_BOTTOM

public static final int KEY_MARGIN_BOTTOM

Margin dimensions

### KEY_MARGIN_LEFT

public static final int KEY_MARGIN_LEFT

Margin left

### KEY_MARGIN_RIGHT

public static final int KEY_MARGIN_RIGHT

Margin right

### KEY_MARGIN_TOP

public static final int KEY_MARGIN_TOP

Margin top

### KEY_PADDING_BOTTOM

public static final int KEY_PADDING_BOTTOM

Padding dimensions

### KEY_PADDING_LEFT

public static final int KEY_PADDING_LEFT

Pad left

### KEY_PADDING_RIGHT

public static final int KEY_PADDING_RIGHT

Pad right

### KEY_PADDING_TOP

public static final int KEY_PADDING_TOP

Pad top

### KEY_WIDTH

public static final int KEY_WIDTH

Width. Applies to blocks. It can be null.

### KEY_HEIGHT

public static final int KEY_HEIGHT

Height. Applies to images for now. It can be null.

### KEY_MIN_WIDTH

public static final int KEY_MIN_WIDTH

Minimum width. Applies to blocks. It can be null.

### KEY_MAX_WIDTH

public static final int KEY_MAX_WIDTH

Maximum width. Applies to blocks. It can be null.

### KEY_TEXT_ALIGN

public static final int KEY_TEXT_ALIGN

Text align

### KEY_TEXT_INDENT

public static final int KEY_TEXT_INDENT

Text indent

### KEY_WHITESPACE

public static final int KEY_WHITESPACE

Whitespace

### KEY_EDITABLE

public static final int KEY_EDITABLE

True if this view is editable

### KEY_BORDER_SPACING

public static final int KEY_BORDER_SPACING

Key for the border spacing array

### KEY_VISIBILITY

public static final int KEY_VISIBILITY

Key for the 'visibility' property.

### KEY_VISIBITY

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static final int KEY_VISIBITY
 Deprecated.
This is a typo of the [KEY_VISIBILITY](#KEY_VISIBILITY).

Key for the 'visibility' property.

### KEY_EMPTY_CELLS

public static final int KEY_EMPTY_CELLS

Key used to store the property 'empty-cells' value as string.

### KEY_FOLDABLE

public static final int KEY_FOLDABLE

Key used to store the property 'foldable' value.

### KEY_NON_FOLDABLE_CHILD_NAME

public static final int KEY_NON_FOLDABLE_CHILD_NAME

Key used to store the property 'non foldable child name' value.

### KEY_VERTICAL_ALIGN

public static final int KEY_VERTICAL_ALIGN

Key for vertical align.

### KEY_COUNTER_RESET

public static final int KEY_COUNTER_RESET

The key for counter-reset .

### KEY_COUNTER_INCREMENT

public static final int KEY_COUNTER_INCREMENT

The key for counter-increment .

### KEY_IMPOSED_DISPLAY

public static final int KEY_IMPOSED_DISPLAY

Key used to override the display property defined in the css.

### KEY_TEXT_DECORATION_LINE

public static final int KEY_TEXT_DECORATION_LINE

Key used to store 'text-decoration-line' property.

### KEY_TEXT_DECORATION

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static final int KEY_TEXT_DECORATION
 Deprecated.
It is a shorthand now, use [KEY_TEXT_DECORATION_LINE](#KEY_TEXT_DECORATION_LINE), [KEY_TEXT_DECORATION_COLOR](#KEY_TEXT_DECORATION_COLOR), [KEY_TEXT_DECORATION_STYLE](#KEY_TEXT_DECORATION_STYLE) instead.

Key used to store 'text-decoration' property. It is mapped to the [KEY_TEXT_DECORATION_LINE](#KEY_TEXT_DECORATION_LINE). Starting from CSS level 3, the 'text-decoration' property is a shorthand, mapped to 'text-decoration-line', 'text-decoration-style' and 'text-decoration-color'.

### KEY_TEXT_DECORATION_COLOR

public static final int KEY_TEXT_DECORATION_COLOR

Key used to store color for text decoration.

### KEY_LINK

public static final int KEY_LINK

Key used to store the URL for link elements.

### KEY_LINK_URL

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public static final int KEY_LINK_URL
 Deprecated.
since 17

Alias for backward compatibility.

### KEY_DISPLAY_TAGS

public static final int KEY_DISPLAY_TAGS

Key used to hide sentinel markers.

### KEY_DIRECT_WHITESPACE

public static final int KEY_DIRECT_WHITESPACE

Whitespace specified directly on the node, not inherited.

### KEY_FILTERED_OUT

public static final int KEY_FILTERED_OUT

Key set for filtered out nodes.

### KEY_TEXT_TRANSFORM

public static final int KEY_TEXT_TRANSFORM

Text transform

### KEY_SHOW_PLACEHOLDER

public static final int KEY_SHOW_PLACEHOLDER

Key used to store the property 'show-placeholder' value.

### KEY_PLACEHOLDER_CONTENT

public static final int KEY_PLACEHOLDER_CONTENT

Key used to store the property 'placeholder-content' value.

### KEY_FOLDED

public static final int KEY_FOLDED

Key used to store the property 'folded' value.

### KEY_TAGS_BACKGROUND_COLOR

public static final int KEY_TAGS_BACKGROUND_COLOR

Key used to store the property '-oxy-tags-background-color' value.

### KEY_TAGS_COLOR

public static final int KEY_TAGS_COLOR

Key used to store the property '-oxy-tags-color' value.

### KEY_BACKGROUND_IMAGE

public static final int KEY_BACKGROUND_IMAGE

Key used to store the property 'background-image' value.

### KEY_OXY_FOREGROUND_IMAGE

public static final int KEY_OXY_FOREGROUND_IMAGE

Key used to store the property '-oxy-foreground-image' value.

### KEY_OXY_VIDEO_COVER

public static final int KEY_OXY_VIDEO_COVER

Key used to store the property '-oxy-video-cover' value.

### KEY_BACKGROUND_REPEAT

public static final int KEY_BACKGROUND_REPEAT

Key used to store the property 'background-repeat' value.

### KEY_BACKGROUND_POSITION

public static final int KEY_BACKGROUND_POSITION

Key used to store the property 'background-position' value.

### KEY_DIRECTION

public static final int KEY_DIRECTION

Key used to store the property 'direction' value.

### KEY_UNICODE_BIDI

public static final int KEY_UNICODE_BIDI

Key used to store the property 'unicode-bidi' value.

### KEY_TEXT_DECORATION_STYLE

public static final int KEY_TEXT_DECORATION_STYLE

Key used to store 'text-decoration' property.

### KEY_MIN_HEIGHT

public static final int KEY_MIN_HEIGHT

Minimum height. Applies to blocks. It can be null.

### KEY_MAX_HEIGHT

public static final int KEY_MAX_HEIGHT

Maximum height. Applies to blocks. It can be null.

### KEY_POSITION

public static final int KEY_POSITION

The 'position' property.

### KEY_TOP

public static final int KEY_TOP

The 'top' property.

### KEY_BOTTOM

public static final int KEY_BOTTOM

The 'bottom' property.

### KEY_LEFT

public static final int KEY_LEFT

The 'left' property.

### KEY_RIGHT

public static final int KEY_RIGHT

The 'right' property.

### KEY_OUTLINE_COLOR

public static final int KEY_OUTLINE_COLOR

Outline color

### KEY_OUTLINE_STYLE

public static final int KEY_OUTLINE_STYLE

Outline style

### KEY_OUTLINE_WIDTH

public static final int KEY_OUTLINE_WIDTH

Outline width

### KEY_OXY_STYLE

public static final int KEY_OXY_STYLE

The -oxy-style property that defines additional styles.

### KEY_EMPTY_CELLS_BOOLEAN

public static final int KEY_EMPTY_CELLS_BOOLEAN

Key used to store the property 'empty-cells' value as boolean.

### KEY_OXY_LINK_ACTIVATION_TRIGGER

public static final int KEY_OXY_LINK_ACTIVATION_TRIGGER

Key used to store the property '-oxy-link-activation-trigger' value.

### KEY_OXY_FLOATING_TOOLBAR

public static final int KEY_OXY_FLOATING_TOOLBAR

Key used to store the property -oxy-floating-toolbar. The value set for this property must be an array of instances of the [StaticContent](StaticContent.md) interface.

### KEY_BORDER_TOP_LEFT_RADIUS

public static final int KEY_BORDER_TOP_LEFT_RADIUS

border-top-left-radius.
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/border-top-left-radius"

### KEY_BORDER_TOP_RIGHT_RADIUS

public static final int KEY_BORDER_TOP_RIGHT_RADIUS

border-top-right-radius.
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/border-top-right-radius"

### KEY_BORDER_BOTTOM_RIGHT_RADIUS

public static final int KEY_BORDER_BOTTOM_RIGHT_RADIUS

border-bottom-right-radius.
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom-right-radius"

### KEY_BORDER_BOTTOM_LEFT_RADIUS

public static final int KEY_BORDER_BOTTOM_LEFT_RADIUS

border-bottom-left-radius.
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/border-bottom-left-radius"

### KEY_FONT_STYLE

public static final int KEY_FONT_STYLE

Font style. Used from the converter.The rest of the code can use the [KEY_FONT](#KEY_FONT), that integrates this property in the [Font](../../exml/view/graphics/Font.md) object.

### pmCounter

protected static int pmCounter

All the properties before this counter are for media screen. Now are following the properties for the paged media.

### KEY_LIST_STYLE_IMAGE

public static final int KEY_LIST_STYLE_IMAGE

List style image

### KEY_PAGE

public static final int KEY_PAGE

The CSS page - for media print.

### KEY_OXY_PAGE_GROUP

public static final int KEY_OXY_PAGE_GROUP

The oxy-page-group property. The presence of this property on an the element makes the Chemistry processor start a new page sequence that begins with that element, even if the element before it had the same page property.

### KEY_IMAGE_RESOLUTION

public static final int KEY_IMAGE_RESOLUTION

Key used to specify the image DPI.

### KEY_OXY_ALT_TEXT

public static final int KEY_OXY_ALT_TEXT

Key used to specify the accessibility alternate text.

### KEY_OXY_PDF_TAG_TYPE

public static final int KEY_OXY_PDF_TAG_TYPE

Key used to specify the accessibility PDF tag.

### KEY_OXY_PDF_META_AUTHOR

public static final int KEY_OXY_PDF_META_AUTHOR

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_AUTHOR

### KEY_OXY_PDF_META_TITLE

public static final int KEY_OXY_PDF_META_TITLE

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_TITLE

### KEY_OXY_PDF_META_DESCRIPTION

public static final int KEY_OXY_PDF_META_DESCRIPTION

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_DESCRIPTION

### KEY_OXY_PDF_META_KEYWORDS

public static final int KEY_OXY_PDF_META_KEYWORDS

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_KEYWORDS

### KEY_OXY_PDF_META_KEYWORD

public static final int KEY_OXY_PDF_META_KEYWORD

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_KEYWORD

### KEY_OXY_PDF_META_COPYRIGHT

public static final int KEY_OXY_PDF_META_COPYRIGHT

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_COPYRIGHT

### KEY_OXY_PDF_META_COPYRIGHTED

public static final int KEY_OXY_PDF_META_COPYRIGHTED

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_COPYRIGHTED

### KEY_OXY_PDF_META_COPYRIGHT_URL

public static final int KEY_OXY_PDF_META_COPYRIGHT_URL

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_COPYRIGHT_URL

### KEY_OXY_PDF_META_CUSTOM

public static final int KEY_OXY_PDF_META_CUSTOM

Key used for PDF metadata.
  See Also:
        * CSSPropertiesOxygenExtension.OXY_PDF_META_CUSTOM

### KEY_BACKGROUND_SIZE

public static final int KEY_BACKGROUND_SIZE

Key used to store the property 'background-size' value.

### KEY_BREAK_BEFORE

public static final int KEY_BREAK_BEFORE

Property for CSS media paged, signal the break policy that applies

### KEY_BREAK_AFTER

public static final int KEY_BREAK_AFTER

Property for CSS media paged, signal the break policy that applies

### KEY_BREAK_INSIDE

public static final int KEY_BREAK_INSIDE

Property for CSS media paged, signal the break policy that applies

### KEY_PAGE_BREAK_AFTER

public static final int KEY_PAGE_BREAK_AFTER

Property for CSS media paged, signals the page break policy that applies.

### KEY_PAGE_BREAK_BEFORE

public static final int KEY_PAGE_BREAK_BEFORE

Property for CSS media paged, signals the page break policy that applies.

### KEY_PAGE_BREAK_INSIDE

public static final int KEY_PAGE_BREAK_INSIDE

Property for CSS media paged, signals the page break policy that applies.

### KEY_OXY_COLUMN_BREAK_AFTER

public static final int KEY_OXY_COLUMN_BREAK_AFTER

Property for CSS media paged, signals the column break policy that applies.

### KEY_OXY_COLUMN_BREAK_BEFORE

public static final int KEY_OXY_COLUMN_BREAK_BEFORE

Property for CSS media paged, signals the column break policy that applies.

### KEY_OXY_COLUMN_BREAK_INSIDE

public static final int KEY_OXY_COLUMN_BREAK_INSIDE

Property for CSS media paged, signals the column break policy that applies.

### KEY_OXY_BORDERS_CONDITIONALITY

public static final int KEY_OXY_BORDERS_CONDITIONALITY

Property for -oxy-borders-conditionality which allow borders on line breaks.

### KEY_OXY_SPACE_BEFORE_CONDITIONALITY

public static final int KEY_OXY_SPACE_BEFORE_CONDITIONALITY

Property for-oxy-space-before-conditionality which allow margin-top drop on elements.

### KEY_OXY_SPACE_AFTER_CONDITIONALITY

public static final int KEY_OXY_SPACE_AFTER_CONDITIONALITY

Property for -oxy-space-after-conditionality which allow margin-bottom drop on elements.

### KEY_OXY_CHANGEBAR_OFFSET

public static final int KEY_OXY_CHANGEBAR_OFFSET

Property for -oxy-changebar-offset, set the distance from the column edge.

### KEY_OXY_CHANGEBAR_STYLE

public static final int KEY_OXY_CHANGEBAR_STYLE

Property for -oxy-changebar-style, set how the change bar appears.

### KEY_OXY_CHANGEBAR_PLACEMENT

public static final int KEY_OXY_CHANGEBAR_PLACEMENT

Property for -oxy-changebar-placement, set the changebar position.

### KEY_OXY_CHANGEBAR_COLOR

public static final int KEY_OXY_CHANGEBAR_COLOR

Property for -oxy-changebar-color, set the changebar color.

### KEY_OXY_CHANGEBAR_WIDTH

public static final int KEY_OXY_CHANGEBAR_WIDTH

Property for -oxy-changebar-width, set the changebar color.

### KEY_ORPHANS

public static final int KEY_ORPHANS

Property for CSS media paged "orphans". The minimum number of lines of a paragraph that must be left at the **bottom** of a page. Supports as values:  | inherit, default is 2.

### KEY_WIDOWS

public static final int KEY_WIDOWS

Property for CSS media paged "widows". The minimum number of lines of a paragraph that must be left at the **top** of a page. Supports as values:  | inherit, default is 2.

### KEY_STRING_SET

public static final int KEY_STRING_SET

Property for CSS media paged "string-set". The string-set property contains one or more pairs, each consisting of an custom identifier (the name of the named string) followed by a content-list describing how to construct the value of the named string.

### KEY_FLOAT

public static final int KEY_FLOAT

Property for CSS media paged "float". Used specially for the footnotes. https://www.w3.org/TR/css-page-floats-3/#float-property

### KEY_TABLE_ROW_SPAN

public static final int KEY_TABLE_ROW_SPAN

CSS property taken into account to compute the row spanning of a table cell. Non-standard property. The default is 1.

### KEY_TABLE_COLUMN_SPAN

public static final int KEY_TABLE_COLUMN_SPAN

CSS property taken into account to compute the column spanning of a table cell. Non-standard property. The default is 1.

### KEY_CAPTION_SIDE

public static final int KEY_CAPTION_SIDE

Property for CSS caption-side property. Used specially for the tables. https://www.w3.org/TR/CSS2/tables.html#caption-side

### KEY_TABLE_LAYOUT

public static final int KEY_TABLE_LAYOUT

The 'table-layout' property controls the algorithm used to lay out the table cells, rows, and columns. https://www.w3.org/TR/2011/REC-CSS2-20110607/tables.html#propdef-table-layout

### KEY_BORDER_COLLAPSE

public static final int KEY_BORDER_COLLAPSE

This property selects a table's border model. https://www.w3.org/TR/2011/REC-CSS2-20110607/tables.html#borders

### KEY_COLUMN_SPAN

public static final int KEY_COLUMN_SPAN

Specify how an element can span over a multiple column layout. https://drafts.csswg.org/css-multicol-1/#column-span

### KEY_TRANSFORM_ROTATION

public static final int KEY_TRANSFORM_ROTATION

Specify that the element can have a different rotation than the parent. Has the CSS angles, later will be converted to FO angles accepted by the FO attribute "reference-orientation".
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/transform"
        * "https://www.w3.org/TR/xsl/#reference-orientation"

### KEY_HYPHENS

public static final int KEY_HYPHENS

This property controls whether hyphenation is allowed to create more soft wrap opportunities within a line of text.
  See Also:
        * "https://drafts.csswg.org/css-text-3/#propdef-hyphens"

### KEY_BOOKMARK_LEVEL

public static final int KEY_BOOKMARK_LEVEL

Bookmark level. Used by the PDF converter.
  See Also:
        * "https://www.w3.org/TR/css-gcpm-3/#bookmark-level"

### KEY_BOOKMARK_LABEL

public static final int KEY_BOOKMARK_LABEL

Bookmark label. Used by the PDF converter.
  See Also:
        * "https://www.w3.org/TR/css-gcpm-3/#bookmark-label"

### KEY_BOOKMARK_STATE

public static final int KEY_BOOKMARK_STATE

Bookmark state. Used by the PDF converter.
  See Also:
        * "https://www.w3.org/TR/css-gcpm-3/#bookmark-state"

### KEY_LETTER_SPACING

public static final int KEY_LETTER_SPACING

Font letter spacing. Used from the converter. The rest of the code can use the [KEY_FONT](#KEY_FONT), that integrates this property in the [Font](../../exml/view/graphics/Font.md) object.

### KEY_FONT_FAMILY

public static final int KEY_FONT_FAMILY

Font family. Used from the converter.The rest of the code can use the [KEY_FONT](#KEY_FONT), that integrates this property in the [Font](../../exml/view/graphics/Font.md) object.

### KEY_FONT_SIZE

public static final int KEY_FONT_SIZE

Font size. Used from the converter.The rest of the code can use the [KEY_FONT](#KEY_FONT), that integrates this property in the [Font](../../exml/view/graphics/Font.md) object.

### KEY_FONT_VARIANT

public static final int KEY_FONT_VARIANT

Font variant

### KEY_FONT_VARIANT_ALTERNATES

public static final int KEY_FONT_VARIANT_ALTERNATES

Font variant alternates.
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-alternates"

### KEY_FONT_VARIANT_LIGATURES

public static final int KEY_FONT_VARIANT_LIGATURES

Font variant ligatures.
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-ligatures"

### KEY_FONT_VARIANT_NUMERIC

public static final int KEY_FONT_VARIANT_NUMERIC

Font variant numeric.
  See Also:
        * "https://developer.mozilla.org/en-US/docs/Web/CSS/font-variant-numeric"

### KEY_OVERFLOW_WRAP

public static final int KEY_OVERFLOW_WRAP

Overflow wrap.

### KEY_OXY_HYPHENATION_CHARACTER

public static final int KEY_OXY_HYPHENATION_CHARACTER

An oxygen extension, mostly used to hide the hyphen characters. The classic hyphen can be replaced with a zero width space for instance.
  See Also:
        * "https://www.w3.org/TR/xsl11/#hyphenation-character"

### KEY_OXY_HYPHENATION_PUSH_CHARACTER_COUNT

public static final int KEY_OXY_HYPHENATION_PUSH_CHARACTER_COUNT

The minimum number of characters in a hyphenated word after the hyphenation character. This is the minimum number of characters in the word pushed to the next line after the line ending with the hyphenation character. Inherited.
  See Also:
        * "https://www.w3.org/TR/xsl11/#hyphenation-push-character-count"

### KEY_OXY_HYPHENATION_REMAIN_CHARACTER_COUNT

public static final int KEY_OXY_HYPHENATION_REMAIN_CHARACTER_COUNT

The hyphenation-remain-character-count specifies the minimum number of characters in a hyphenated word before the hyphenation character. This is the minimum number of characters in the word left on the line ending with the hyphenation character.
  See Also:
        * "https://www.w3.org/TR/xsl11/#hyphenation-remain-character-count"

### KEY_ALIGNMENT_BASELINE

public static final int KEY_ALIGNMENT_BASELINE

Property for CSS media paged, the alignment relative to the baseline.

### KEY_OXY_CAPTION_REPEAT_ON_NEXT_PAGES

public static final int KEY_OXY_CAPTION_REPEAT_ON_NEXT_PAGES

Property enabling the table caption repetition on next pages (When the table is long and it spans multiple pages).

### KEY_OXY_SHOW_ONLY_WHEN_CAPTION_REPEATED_ON_NEXT_PAGES

public static final int KEY_OXY_SHOW_ONLY_WHEN_CAPTION_REPEATED_ON_NEXT_PAGES

Property that marks a pseudo :before or :after that is associated to a table caption. It signals that the static content to be used only when the caption is displayed the second time, on the next page (When the table is long and it spans multiple pages).

### KEY_OXY_AVOID_BREAKING_LINE_AT_HYPHENS

public static final int KEY_OXY_AVOID_BREAKING_LINE_AT_HYPHENS

Controls the line breaking status for hyphens. Deprecated, [KEY_OXY_BREAK_LINE_AT_HYPHENS](#KEY_OXY_BREAK_LINE_AT_HYPHENS) should be used instead.

### KEY_OXY_BREAK_LINE_AT_HYPHENS

public static final int KEY_OXY_BREAK_LINE_AT_HYPHENS

Controls the line breaking status for hyphens.

### KEY_OXY_PDF_VIEWER_ZOOM

public static final int KEY_OXY_PDF_VIEWER_ZOOM

The zoom factor applied to the viewport when the PDF document is loaded. Should be a percent.

### KEY_OXY_PDF_VIEWER_HIDE_TOOLBAR

public static final int KEY_OXY_PDF_VIEWER_HIDE_TOOLBAR

If the viewer toolbarshould be visible or not.

### KEY_OXY_PDF_VIEWER_HIDE_MENUBAR

public static final int KEY_OXY_PDF_VIEWER_HIDE_MENUBAR

If the viewer menubar should be visible or not.

### KEY_OXY_PDF_VIEWER_FIT_WINDOW

public static final int KEY_OXY_PDF_VIEWER_FIT_WINDOW

A flag specifying whether to resize the documentï¿½s window to fit the size of the first displayed page. Default value: false.

### KEY_OXY_PDF_VIEWER_DISPLAY_FILENAME

public static final int KEY_OXY_PDF_VIEWER_DISPLAY_FILENAME

A flag specifying if the doc title should be displayed.

### KEY_OXY_PDF_TABLE_OMIT_HEADER_BREAK

public static final int KEY_OXY_PDF_TABLE_OMIT_HEADER_BREAK

A flag specifying if the header of a table should be omitted at break.

### KEY_OXY_PDF_TABLE_OMIT_FOOTER_BREAK

public static final int KEY_OXY_PDF_TABLE_OMIT_FOOTER_BREAK

A flag specifying if the footer of a table should be omitted at break.

### KEY_OXY_PDF_EXTRACT_FILE

public static final int KEY_OXY_PDF_EXTRACT_FILE

A pointer for fragments to be extracted as PDF.

### KEY_OXY_PDF_VIEWER_PAGE_MODE

public static final int KEY_OXY_PDF_VIEWER_PAGE_MODE

A name object specifying how the document shall be displayed when opened: none Neither document outline nor thumbnail images visible use-outlines Document outline visible use-thumbs Thumbnail images visible full-screen Full-screen mode, with no menu bar, window controls, or any other window visible

### KEY_OXY_PDF_VIEWER_PAGE_LAYOUT

public static final int KEY_OXY_PDF_VIEWER_PAGE_LAYOUT

A name object specifying the page layout shall be used when the document is opened: single-page Display one page at a time one-column Display the pages in one column two-column-left Display the pages in two columns, with odd- numbered pages on the left two-column-right Display the pages in two columns, with odd- numbered pages on the right

### stylesArray

protected final [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)[] stylesArray

The styles map

## Constructor Details

### Styles

public Styles()

Constructor.

### Styles

public Styles(boolean enablePagedMediaProperties)

Constructor.
  Parameters: enablePagedMediaProperties - true if the styles object is built for the PDF converter, and all the known paged media features must be taken into account.
## Method Details

### isEnablePagedMediaProperties

public boolean isEnablePagedMediaProperties()
  Returns: Returns true if the entire set of CSS properties, including the ones defined for paged media are supported.
### getPropertyName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPropertyName(int index)
  Parameters: index - The index of the property. Returns: The property name.
### getPropertyByName

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getPropertyByName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Retrieve the property by its name.
  Parameters: name - The property name. Returns: The property.
### getBackgroundColor

public [Color](../../exml/view/graphics/Color.md) getBackgroundColor()
  Returns: the value of the background-color property. Returns null if the background color is transparent.
### getBackgroundImage

public [URIContent](URIContent.md) getBackgroundImage()

This property sets the background image of an element. When setting a background image, authors should also specify a background color that will be used when the image is unavailable. When the image is available, it is rendered on top of the background color. (Thus, the color is visible in the transparent parts of the image).
  Returns: the value of the background-image property. Returns null if the background image is not defined.
### getBackgroundRepeat

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getBackgroundRepeat()

If a background image is specified, this property specifies whether the image is repeated (tiled), and how. All tiling covers the content, padding and border areas of a box.
  Returns: One of CSS.
### getBackgroundPosition

public ro.sync.ecss.css.BackgroundPosition getBackgroundPosition()

If a background position is specified, this property indicates the position of the background image relative to its box.
  Returns: A position, or null.
### getTagsBackgroundColor

public [Color](../../exml/view/graphics/Color.md) getTagsBackgroundColor()

Obtain the color for full-tags background.
  Returns: the value of the -oxy-tags-background-color property. Returns null if no background color was defined in css.
### getTagsColor

public [Color](../../exml/view/graphics/Color.md) getTagsColor()

Obtain the color for full-tags background.
  Returns: the value of the -oxy-tags-background-color property. Returns null if no background color was defined in css.
### hasBorder

public boolean hasBorder()
  Returns: true if the styles define a visible border.
### getBorderBottomColor

public [Color](../../exml/view/graphics/Color.md) getBorderBottomColor()
  Returns: the value of the borderBottomColor property.
### getBorderBottomStyle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getBorderBottomStyle()
  Returns: the value of the borderBottomStyle property.
### getBorderLeftColor

public [Color](../../exml/view/graphics/Color.md) getBorderLeftColor()
  Returns: the value of the borderLeftColor property.
### getBorderLeftStyle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getBorderLeftStyle()
  Returns: the value of the borderLeftStyle property.
### getBorderRightColor

public [Color](../../exml/view/graphics/Color.md) getBorderRightColor()
  Returns: the value of the borderRightColor property.
### getBorderRightStyle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getBorderRightStyle()
  Returns: the value of the borderRightStyle property.
### getBorderTopColor

public [Color](../../exml/view/graphics/Color.md) getBorderTopColor()
  Returns: the value of the borderTopColor property.
### getBorderTopStyle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getBorderTopStyle()
  Returns: the value of the borderTopStyle property.
### getOutlineColor

public [Color](../../exml/view/graphics/Color.md) getOutlineColor()
  Returns: the value of the outline-color property. If is not set returns the
### getOutlineStyle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOutlineStyle()
  Returns: the value of the outline-style property.
### getOutlineWidth

public int getOutlineWidth()
  Returns: the value of outline-width property.
### getColor

public [Color](../../exml/view/graphics/Color.md) getColor()
  Returns: the value of the color property.
### getMixedContent

public [StaticContent](StaticContent.md)[] getMixedContent()
  Returns: a List of ContentPart objects representing the content property.
### getDisplay

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplay()

First it looks at the KEY_IMPOSED_DISPLAY property. If it is not set it looks at the KEY_DISPLAY property.
  Returns: the value of the display property or CSS.INLINE if nothing is specified.
### getPosition

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPosition()

Checks the 'position' property.
  Returns: one of CSSValues.STATIC, CSSValues.RELATIVE, CSSValues.FIXED or CSSValues.ABSOLUTE .
### isMorphDisplay

public boolean isMorphDisplay()

Check if the display has 'morph' or '-oxy-morph' value.
  Returns: true for morph display.
### isChangebarDisplay

public boolean isChangebarDisplay()

Check if the display has '-oxy-change-bar-start' or '-oxy-change-bar-end' value.
  Returns: true if is a change bar.
### isInvisible

public boolean isInvisible()
  Returns: true if the associated element is invisible.
### isListItem

public boolean isListItem()
  Returns: true if the associated element is a list item.
### getFont

public [Font](../../exml/view/graphics/Font.md) getFont()
  Returns: the value of the font property. Never null.
### getFontWeight

public int getFontWeight()
  Returns: the value of the fontWeight property.
### getFontVariant

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFontVariant()

Gets the font-variant.
  Returns: the value of the font-variant property. One of 'normal' or 'small-caps'. Never null.
### getLineHeight

public int getLineHeight([FontMetrics](../../exml/view/graphics/FontMetrics.md) fm)

Sets the distance between lines: normal number length %
  Parameters: fm - Font metrics for this style's font Returns: the value of the lineHeight property.
### getListStyleType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getListStyleType()
  Returns: the value of the listStyleType property.
### getListStylePosition

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getListStylePosition()
  Returns: the value of the listStylePosition property.
### getTextAlign

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTextAlign()

Aligns the text in an element: left right center justify.
  Returns: the value of the textAlign property.
### isSpecifiedTextAlign

public boolean isSpecifiedTextAlign()

Checks if the text-align property from the current element styles has a value specified by the CSS. The text-align value could be inherited.
  Returns: true if the text align was specified for the current element or one of its parents.
### getTextIndent

public [RelativeLength](RelativeLength.md) getTextIndent()

Gets the horizontal space that should be left before the beginning of the first line of the text content of an element.
  Returns: the value of the text-indent property, or null if none.
### isInline

public boolean isInline()

Gets the imposed display - it may be the same as the one specified in the CSS - and checks if it is inline or inline block.
  Returns: true if this element has the display property set to CSS.INLINE and thus it must be rendered as an inline box. Note that if this method returns false it doesn't necessarily mean that the element must be rendered as a block. The isInvisible() should be taken into account as well. See LayoutUtils.isInvisible()
### isTableRowGroup

public boolean isTableRowGroup()
  Returns: true if this element is table-formatted, or false otherwise.
### isTableRow

public boolean isTableRow()
  Returns: true if this element is table-formatted, or false otherwise.
### getBorderBottomWidth

public int getBorderBottomWidth()
  Returns: the value of border-bottom-width
### getBorderLeftWidth

public int getBorderLeftWidth()
  Returns: the value of border-left-width
### getBorderRightWidth

public int getBorderRightWidth()
  Returns: the value of border-right-width
### getBorderTopWidth

public int getBorderTopWidth()
  Returns: the value of border-top-width
### getMarginBottom

public [RelativeLength](RelativeLength.md) getMarginBottom()
  Returns: the value of margin-bottom
### getBorderBottomLeftRadius

public [RelativeLength](RelativeLength.md) getBorderBottomLeftRadius()
  Returns: the value of border bottom left radius
### getBorderBottomRightRadius

public [RelativeLength](RelativeLength.md) getBorderBottomRightRadius()
  Returns: the value of border bottom right radius
### getBorderTopLeftRadius

public [RelativeLength](RelativeLength.md) getBorderTopLeftRadius()
  Returns: the value of border top left radius
### getBorderTopRightRadius

public [RelativeLength](RelativeLength.md) getBorderTopRightRadius()
  Returns: the value of border top right radius
### getMarginLeft

public [RelativeLength](RelativeLength.md) getMarginLeft()
  Returns: the value of margin-left
### getMarginRight

public [RelativeLength](RelativeLength.md) getMarginRight()
  Returns: the value of margin-right
### getMarginTop

public [RelativeLength](RelativeLength.md) getMarginTop()
  Returns: the value of margin-top
### getPaddingBottom

public [RelativeLength](RelativeLength.md) getPaddingBottom()
  Returns: the value of padding-bottom
### getDirection

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDirection()

The direction CSS property should be set to match the direction of the text: rtl for Hebrew or Arabic text and ltr for other scripts.
The property sets the base text direction of block-level elements and the direction of embeddings created by the unicode-bidi property. It also sets the default alignment of text and block-level elements and the direction that cells flow within a table row. Unlike the dir attribute in HTML, the direction property is not inherited from table columns into table cells, since CSS inheritance follows the document tree, and table cells are inside of the rows but not inside of the columns.

This is inheritable. The initial value is CSSValues.LTR.

  Returns: The direction, one of CSSValues.LTR or CSSValues.RTL.
### getUnicodeBIDI

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getUnicodeBIDI()

The unicode-bidi CSS property together with the direction property relates to the handling of bidirectional text in a document. For example, if a block of text contains both left-to-right and right-to-left text then the user-agent uses a complex Unicode algorithm to decide how to display the text. This property overrides this algorithm and allows the developer to control the text embedding.
This is not inheritable. The initial value is CSSValues.NORMAL.

  Returns: one of CSSValues.EMBED, CSSValues.BIDI_OVERRIDE or CSSValues.NORMAL.
### getPaddingLeft

public [RelativeLength](RelativeLength.md) getPaddingLeft()
  Returns: the value of padding-left
### getPaddingRight

public [RelativeLength](RelativeLength.md) getPaddingRight()
  Returns: the value of padding-right
### getPaddingTop

public [RelativeLength](RelativeLength.md) getPaddingTop()
  Returns: the value of padding-top
### isTable

public boolean isTable()

Checks if the display mode indicated to be a table.
  Returns: True if it is.
### isTableCell

public boolean isTableCell()

Checks if the display mode indicated to be a table cell.
  Returns: True if it is.
### getWhitespace

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getWhitespace()
  Returns: The whitespace value.
### getDirectWhitespace

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDirectWhitespace()
  Returns: The whitespace value, specified directly on the node by the CSS rules, not inherited.
### isTableHeaderGroup

public boolean isTableHeaderGroup()

Checks if the display mode indicated to be a table group header.
  Returns: True if it is.
### isTableFooterGroup

public boolean isTableFooterGroup()

Checks if the display mode indicated to be a table group footer.
  Returns: True if it is.
### isTableColumn

public boolean isTableColumn()

Checks if the display mode indicated to be a table column.
  Returns: True if it is.
### isTableColumnGroup

public boolean isTableColumnGroup()

Checks if the display mode indicated to be a table group of columns.
  Returns: True if it is.
### getWidth

public [RelativeLength](RelativeLength.md) getWidth()
  Returns: The specified width, as a relative length, or null if not specified by the CSS.
### getHeight

public [RelativeLength](RelativeLength.md) getHeight()
  Returns: The specified height, as a relative length, or null if not specified by the CSS.
### getMinWidth

public [RelativeLength](RelativeLength.md) getMinWidth()
  Returns: The minimum width, or null if not specified.
### getMaxWidth

public [RelativeLength](RelativeLength.md) getMaxWidth()
  Returns: The maximum width, or null if not specified.
### isEditable

public boolean isEditable()
  Returns: true if the view is editable
### getHorizontalBorderSpacing

public int getHorizontalBorderSpacing()
  Returns: The horizontal border spacing between table cells.
### getVerticalBorderSpacing

public int getVerticalBorderSpacing()
  Returns: The vertical border spacing between table cells.
### setProperty

public void setProperty(int property, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

Set a property to the map.
  Parameters: property - The key of the property to be set. It can be one of the keys defined in this class. value - The value of the property. Accepted values depend on the property and can have as type [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html), [Color](../../exml/view/graphics/Color.md), [RelativeLength](RelativeLength.md), [CSSCounter](CSSCounter.md), [CSSCounterIncrement](CSSCounterIncrement.md) or a subclass of [StaticContent](StaticContent.md). The actual values are the Java representations of the ones accepted in the CSS specification. Read more about the CSS support in the Developer Guide.
### setProperty

public void setProperty(int property, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value, org.w3c.css.sac.LexicalUnit lu)

Set a property to the map.
  Parameters: property - The key of the property to be set. It can be one of the keys defined in this class. value - The value of the property. Accepted values depend on the property and can have as type [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html), [Color](../../exml/view/graphics/Color.md), [RelativeLength](RelativeLength.md), [CSSCounter](CSSCounter.md), [CSSCounterIncrement](CSSCounterIncrement.md) or a subclass of [StaticContent](StaticContent.md)The actual values are the Java representations of the ones accepted in the CSS specification. Read more about the CSS support in the Developer Guide. lu - The CSS lexical unit that was evaluated to the value of the property. Normally, this is ignored, but may be useful to subclasses (for instance in the CSS to FO processor).
### getProperty

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getProperty(int property)
  Parameters: property - The property name. Returns: The value of the property.
### isInheritable

public static boolean isInheritable(int property)

Check if the given property should be copied from parent to child. A property can be copied if is marked as being inheritable.
  Parameters: property - The index of the CSS property. One of the KEY_ constants. Use [getRecognizedPropertiesNumber()](#getRecognizedPropertiesNumber()) to get the limit. Returns: true if the given property can be copied.
### isInheritable

public static boolean isInheritable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) property)

Check if the given property can be inherited from parent to child. IMPORTANT: This method will check only the expanded properties, not the shorthand ones. For instance it will return true for "border" or "border-right" (is a shorthand, does not know about it), but false for "border-right-color".
  Parameters: property - The name of the CSS property. Must not be a shorthand! Returns: true if the given property is inherited.
### getVisibility

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getVisibility()
  Returns: The value of the 'visibility'
### getShowPlaceholders

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getShowPlaceholders()
  Returns: The value of the 'show-placeholder' property.
### getPlaceholderContent

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPlaceholderContent()
  Returns: The value of the 'placeholder-content' property.
### getShowEmptyCells

public boolean getShowEmptyCells()
  Returns: Return true if table empty cells are shown. See http://www.w3.org/TR/CSS21/tables.html#empty-cells.
### isFoldable

public boolean isFoldable()
  Returns: true if this element is foldable
### isFolded

public boolean isFolded()
  Returns: true if this element is folded
### getNonFoldableChildName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNonFoldableChildName()
  Returns: The name of the child which is non foldable
### isTableCaption

public boolean isTableCaption()

Checks if the display mode indicated to be a table caption.
  Returns: True if it is.
### isInlineInCSS

public boolean isInlineInCSS()
  Returns: true if element is specified as INLINE in CSS source.
### isInlineBlockInCSS

public boolean isInlineBlockInCSS()
  Returns: true if element is specified as INLINE_BLOCK in CSS source.
### getVerticalAlign

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getVerticalAlign()
  Returns: The vertical align.
### getTextDecoration

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTextDecoration()
 Deprecated.
This was used to return only the text-decoration-line part from the text-decoration shorthand, as defined here https://drafts.csswg.org/css-text-decor-3/#text-decoration-property.
   Returns: The values defining the decoration line from the 'text-decoration' property.
### getTextDecorationLine

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getTextDecorationLine()
  Returns: The value of 'text-decoration' property.
### getTextDecorationStyle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTextDecorationStyle()
  Returns: The value of 'text-decoration-style' property.
### getTextDecorationColor

public [Color](../../exml/view/graphics/Color.md) getTextDecorationColor()
  Returns: The color to be used for paint text decoration.
### getCounters

public [CSSCounter](CSSCounter.md)[] getCounters()
  Returns: The counters declared on this element or empty array if none.
### getCountersIncrement

public [CSSCounterIncrement](CSSCounterIncrement.md)[] getCountersIncrement()
  Returns: The 'counters increment' declared on this element or empty array if none.
### isInTable

public boolean isInTable()

Check if is a style from a table but not a cell.
  Returns: true if the current style is a one of CSS.TABLE, CSS.INLINE_TABLE, CSS.TABLE_ROW, CSS.TABLE_ROW_GROUP, CSS.TABLE_FOOTER_GROUP, CSS.TABLE_HEADER_GROUP
### getLinkURL

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLinkURL()
  Returns: The value of the 'link' property. Null if property was absent.
### getHyperlinkActivationType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHyperlinkActivationType()
  Returns: The hyperlink activation behavior: auto, click, modifier-click(ctrl+click), inherit.
### getDisplayTags

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayTags()
  Returns: Returns the value of the property 'display-tags'. The possible values are:
        * CSS.DEFAULT - display tag markers depending on the current display mode;
        * CSS.NONE - tag markers will not be shown.
The default value is CSS.DEFAULT.
### getTextTransform

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTextTransform()
  Returns: Returns the value of the property 'text-transform'. The possible values are:
        * CSS.CAPITALIZE
        * CSS.UPPERCASE
        * CSS.LOWERCASE
The default value is null
### isFilteredOut

public boolean isFilteredOut()
  Returns: true if a node should be represented with faded colors.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### clone

public [Styles](Styles.md) clone()

Shallow clone.
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
### canBeCached

public boolean canBeCached()

Verify if styles can be cached. Can be cached if properties values does not depends by attributes or document structure.
  Returns: True if styles can be cached.
### setCanBeCached

public void setCanBeCached(boolean canBeCached)

Sets if those styles can be shared between two or more nodes.
  Parameters: canBeCached - True when be shared between two or more nodes.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### getMinHeight

public [RelativeLength](RelativeLength.md) getMinHeight()

Gets the value associated with the min-height property
  Returns: The relative length (to the viewport width) of the minimum height.
### getLeft

public [RelativeLength](RelativeLength.md) getLeft()
  Returns: The left position offset. May be null.
### getRight

public [RelativeLength](RelativeLength.md) getRight()
  Returns: The right position offset. May be null.
### getTop

public [RelativeLength](RelativeLength.md) getTop()
  Returns: The top position offset. May be null.
### getBottom

public [RelativeLength](RelativeLength.md) getBottom()
  Returns: The bottom position offset. May be null.
### setPseudoLevel

public void setPseudoLevel(int pseudoLevel)

If this is the style for a pseudo element, keep here its level. For a :before(2), 2 is the pseudo level.
  Parameters: pseudoLevel - The level of the pseudo element, if the style is associated to one.
### getPseudoLevel

public int getPseudoLevel()

If this is the style for a pseudo element, get its level. For a :before(2), 2 is the pseudo level. For :before, the level is 1.
  Returns: Returns the pseudo level, zero if it is not the style of a pseudo element, 1 if is the "normal" pseudo element.
### getRecognizedPropertiesNumber

public int getRecognizedPropertiesNumber()

Use this to get the number of recognized properties. You can iterate over the properties up to this number. If the [isEnablePagedMediaProperties()](#isEnablePagedMediaProperties()) is true, there are many more properties recognized.
  Returns: The total number of recognized properties.
### getLexicalUnit

public org.w3c.css.sac.LexicalUnit getLexicalUnit(int key)

Gets a lexical unit. In this implementation, it returns null.
  Parameters: key - The property key. Returns: The CSS lexical unit that generated the value for that property. Can be null.
### getTableRowSpan

public int getTableRowSpan()

Gets the 'table-row-span' property value. Used from the XML+CSS converter only. Not used by the Author layout engine.
  Returns: An integer, or the default value 1 if the property was not set.
### getTableColumnSpan

public int getTableColumnSpan()

Gets the 'table-column-span' property value. Used from the XML+CSS converter only. Not used by the Author layout engine.
  Returns: An integer, or the default value 1 if the property was not set.
### getStringSet

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[StaticContent](StaticContent.md)[]> getStringSet()

The string-set property contains one or more pairs, each consisting of an custom identifier (the name of the named string) followed by a content-list describing how to construct the value of the named string. Used from the XML+CSS converter only. Not used by the Author layout engine.
  Returns: a map from a string name to an array of static content. Never null.
### getAlignmentBaseline

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAlignmentBaseline()
  Returns: The alignment baseline. Never null. Default is 'baseline'.
### getBordersConditionality

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getBordersConditionality()
  Returns: the value of for the '-oxy-borders-conditionality' property, or 'discard' if nothing was set.
### getSpaceBeforeConditionality

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSpaceBeforeConditionality()
  Returns: the value of for the '-oxy-space-before-conditionality' property, or 'discard' if nothing was set.
### getSpaceAfterConditionality

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSpaceAfterConditionality()
  Returns: the value of for the '-oxy-space-after-conditionality' property, or 'discard' if nothing was set.
### dependsOnTargetCounter

public boolean dependsOnTargetCounter()

Checks if the style defines some static content using the target-counter or target-counters CSS function.
  Returns: true if target-counter or target-counters are used.
### affectsCounters

public boolean affectsCounters()

Checks if the styles increment or reset some of the counters.
  Returns: true if the styles are affecting the counters state.
### setCustomProperty

public void setCustomProperty([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.css.functions.customprop.CustomPropertyValue> props)

Sets the list of custom CSS properties and their values.
  Parameters: props - Custom CSS properties
### getCustomCssProperties

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.ecss.css.functions.customprop.CustomPropertyValue> getCustomCssProperties()
  Returns: Returns the customCssProperties.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
