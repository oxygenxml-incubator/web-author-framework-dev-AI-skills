Package [ro.sync.ecss.dom.builder](package-summary.md)

# Interface AuthorFormatCompatibilityModeConstants
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorFormatCompatibilityModeConstants
The way formatting when passing from author in text or on save.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [FORMAT_COMPATIBILITY_BREAKS_LINES_ONLY_BLOCKS_DO_NO_INDENT](#FORMAT_COMPATIBILITY_BREAKS_LINES_ONLY_BLOCKS_DO_NO_INDENT)
Compatibility mode.
  static final int [FORMAT_COMPATIBILITY_DO_NOT_BREAK_LINES_DO_NO_INDENT](#FORMAT_COMPATIBILITY_DO_NOT_BREAK_LINES_DO_NO_INDENT)
Compatibility mode.
  static final int [FORMAT_COMPATIBILITY_NONE](#FORMAT_COMPATIBILITY_NONE)
Compatibility mode.

## Field Details

### FORMAT_COMPATIBILITY_NONE

static final int FORMAT_COMPATIBILITY_NONE

Compatibility mode. Nothing special is done for compatibility purpose. The formatting is the default one.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.dom.builder.AuthorFormatCompatibilityModeConstants.FORMAT_COMPATIBILITY_NONE)

### FORMAT_COMPATIBILITY_DO_NOT_BREAK_LINES_DO_NO_INDENT

static final int FORMAT_COMPATIBILITY_DO_NOT_BREAK_LINES_DO_NO_INDENT

Compatibility mode. "Do not break lines, do not indent", avoids emitting newlines after elements start or end tags and no indent is used. The newlines added by the user in elements with xml:space preserve, like pre elements in HTML or codeblock in DITA are still emitted.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.dom.builder.AuthorFormatCompatibilityModeConstants.FORMAT_COMPATIBILITY_DO_NOT_BREAK_LINES_DO_NO_INDENT)

### FORMAT_COMPATIBILITY_BREAKS_LINES_ONLY_BLOCKS_DO_NO_INDENT

static final int FORMAT_COMPATIBILITY_BREAKS_LINES_ONLY_BLOCKS_DO_NO_INDENT

Compatibility mode. "Break lines only after elements displayed as blocks, do not indent" makes the editor emit newlines only after elements which have a CSS display property of blocks, tables, list items, etc (not inlines). In this case the CSS is dictating the formatting. The newlines added by the user in elements with xml:space preserve, like pre elements in HTML or codeblock in DITA are still emitted.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.dom.builder.AuthorFormatCompatibilityModeConstants.FORMAT_COMPATIBILITY_BREAKS_LINES_ONLY_BLOCKS_DO_NO_INDENT)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
