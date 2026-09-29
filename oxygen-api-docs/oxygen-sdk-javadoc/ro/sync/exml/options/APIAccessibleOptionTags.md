Package [ro.sync.exml.options](package-summary.md)

# Interface APIAccessibleOptionTags
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface APIAccessibleOptionTags
Global Oxygen options which can be read and set via the API.
  Since: 18
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDITIONAL_FRAMEWORKS_DIRECTORIES](#ADDITIONAL_FRAMEWORKS_DIRECTORIES)
Array of strings indicating the additional frameworks directories.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDONS_UPDATE_SITES](#ADDONS_UPDATE_SITES)
Array of strings indicating the update sites list.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARCHIVE_DESCRIPTORS](#ARCHIVE_DESCRIPTORS)
All the extensions recognized as archives.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ASK_OPEN_DITA_MAP_IN_DITAMANAGER](#ASK_OPEN_DITA_MAP_IN_DITAMANAGER)
Remember if Oxygen should ask the user if the dita map will be opened in the dita maps manager.Possible integer values:ro.sync.exml.options.APIOptionConstants.ALWAYS_ASKro.sync.exml.options.APIOptionConstants.ALWAYS_NOro.sync.exml.options.APIOptionConstants.ALWAYS_YES
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTHOR_DISPLAY_REFERENCES_EXPANDED](#AUTHOR_DISPLAY_REFERENCES_EXPANDED)
Key for display references expanded author option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTHOR_EDITING_MODE](#AUTHOR_EDITING_MODE)
Option controlling the author schema aware editing from the "Editor / Edit Modes / Author / Schema-Aware" Preferences page.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTHOR_FORMAT_COMPATIBILITY](#AUTHOR_FORMAT_COMPATIBILITY)
Option for controlling the compatibility of the document serialization from Author editing mode with other tools.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTO_APPLY_STYLES_DITAVAL_MAIN_FILES](#AUTO_APPLY_STYLES_DITAVAL_MAIN_FILES)
Boolean value which controls applying styles defined in ditaval files placed in main files folder
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTO_SYNCHRONIZE_UNMODIFIED_EDITORS](#AUTO_SYNCHRONIZE_UNMODIFIED_EDITORS)
Auto synch unmodified editors with file system.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTOCHECKVERSION_ENABLE](#AUTOCHECKVERSION_ENABLE)
Boolean property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTOMATICALLY_ACCEPT_CERTIFICATES](#AUTOMATICALLY_ACCEPT_CERTIFICATES)
Option that controls if oXygen will accept all HTTPS certificates.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [AUTORECOVERY_LOCATION](#AUTORECOVERY_LOCATION)
A filepath string property defining the folder where the auto-recovery information for documents is stored.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [BULK_APPLY_ONLY_QUICK_FIXES_MARKED_VIA_DEFAULT_FIX_ATTRIBUTE](#BULK_APPLY_ONLY_QUICK_FIXES_MARKED_VIA_DEFAULT_FIX_ATTRIBUTE)
Option that controls whether only quick fixes marked via "default-fix" attribute are considered when applying in bulk.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CAN_EDIT_READ_ONLY_FILES](#CAN_EDIT_READ_ONLY_FILES)
Option for editing read-only files.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CATALOGS](#CATALOGS)
The catalogs key.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CHANGE_TRACKING_AUTHOR](#CHANGE_TRACKING_AUTHOR)
The author for change tracking.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CHECK_FOR_NOTIFICATIONS_ENABLE](#CHECK_FOR_NOTIFICATIONS_ENABLE)
Boolean property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CODE_INSIGHT_SHOW_ANNOTATIONS](#CODE_INSIGHT_SHOW_ANNOTATIONS)
Show annotations (documentation) for each entry in the content completion window.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CODE_INSIGHT_SHOW_ANNOTATIONS_TOOLTIP](#CODE_INSIGHT_SHOW_ANNOTATIONS_TOOLTIP)
Show annotations (documentation) when hovering the mouse over various elements.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CODE_TEMPLATES](#CODE_TEMPLATES)
Code-templates.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CREATE_KEYS_ATTRIBUTE_FOR_TOPICREF_BASED_ON_FILENAME](#CREATE_KEYS_ATTRIBUTE_FOR_TOPICREF_BASED_ON_FILENAME)
Option used to generate the "keys" attribute for topicrefs based on the filename (in DMM).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DIFF_IGNORE_XPATH_EXPRESSION](#DIFF_IGNORE_XPATH_EXPRESSION)
Option used to store the XPath expression used to ignore nodes when files are compared.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DIFF_INFO](#DIFF_INFO)
The current diff info.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_FILL_LINK_FORMAT_ATTR](#DITA_FILL_LINK_FORMAT_ATTR)
Option that controls if the format attribute value will be automatically filled when inserting a link reference.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_FILL_LINK_SCOPE_ATTR](#DITA_FILL_LINK_SCOPE_ATTR)
Option that controls if the scope attribute value will be automatically filled when inserting a link reference.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_FILL_LINK_TYPE_ATTR](#DITA_FILL_LINK_TYPE_ATTR)
Option that controls if the type attribute value will be automatically filled when inserting a link reference.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_FILL_TOPICREF_FORMAT_ATTR](#DITA_FILL_TOPICREF_FORMAT_ATTR)
Option that controls if the format attribute value will be automatically filled when inserting a topic reference.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_FILL_TOPICREF_NAVTITLE_ATTR](#DITA_FILL_TOPICREF_NAVTITLE_ATTR)
Option that controls if the navigation title attribute value will be automatically filled when inserting a topic reference.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_FILL_TOPICREF_SCOPE_ATTR](#DITA_FILL_TOPICREF_SCOPE_ATTR)
Option that controls if the scope attribute value will be automatically filled when inserting a topic reference.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_FILL_TOPICREF_TYPE_ATTR](#DITA_FILL_TOPICREF_TYPE_ATTR)
Option that controls if the type attribute value will be automatically filled when inserting a topic reference.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_OT_DIRECTORY](#DITA_OT_DIRECTORY)
DITA OT Directory.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DITA_SHOW_CONSOLE_OUTPUT](#DITA_SHOW_CONSOLE_OUTPUT)
Option regarding when to show the DITA transformation console output.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDIT_RESOLVED_REFERRED_CONTENT_IN_AUTHOR](#EDIT_RESOLVED_REFERRED_CONTENT_IN_AUTHOR)
Boolean option to allow in-place editing for referred content in Author page.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_DETECT_INDENT_ON_OPEN](#EDITOR_DETECT_INDENT_ON_OPEN)
Boolean property.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_FONT](#EDITOR_FONT)
A property with a string value of the form "name,style,size".
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_FORMAT_INDENT_INLINE_ELEMENTS](#EDITOR_FORMAT_INDENT_INLINE_ELEMENTS)
Indent inline elements.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_INDENT_SIZE](#EDITOR_INDENT_SIZE)
The number of space characters for one indentation level.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_LINE_WIDTH](#EDITOR_LINE_WIDTH)
The maximum length of any line when the Format and Indent (pretty-print) operation is applied.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_SHOW_SPACE](#EDITOR_SHOW_SPACE)
Boolean property for displaying the SPACE characters as special marks or not displaying them in oXygen editors.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_SHOW_TAB_EOL_EOF](#EDITOR_SHOW_TAB_EOL_EOF)
Boolean property for displaying the characters TAB, END-OF-LINE and END-OF-FILE as special marks or not displaying them.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDITOR_USE_TABS](#EDITOR_USE_TABS)
If enabled the indentation will be made with tab characters, if disabled the indentation will be made with space characters.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ENABLE_DITA_2_X_SUPPORT](#ENABLE_DITA_2_X_SUPPORT)
Enable the creation and editing of DITA 2.x documents.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ENABLE_SYNCHRONIZE_UNMODIFIED_EDITORS](#ENABLE_SYNCHRONIZE_UNMODIFIED_EDITORS)
Enable update unmodified editors with file system.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FILE_TYPES_ASSOCIATION](#FILE_TYPES_ASSOCIATION)
File type association.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FONT_FOR_AUTHOR](#FONT_FOR_AUTHOR)
The default font for the author editor.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FONT_FOR_GUI](#FONT_FOR_GUI)
The font for the GUI controls.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FONT_FOR_SCHEMA](#FONT_FOR_SCHEMA)
The default font for the schema editor.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FONT_FOR_TEXT](#FONT_FOR_TEXT)
The font for the text controls.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FRAMEWORKS_DIRECTORY_URL](#FRAMEWORKS_DIRECTORY_URL)
The custom frameworks directory URL with editor variables, when a custom one is set.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [KEYS_CONTEXT_MAP](#KEYS_CONTEXT_MAP)
The keys context map.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPEN_FIND_RESOURCE_INDEXING_OPTIONS](#OPEN_FIND_RESOURCE_INDEXING_OPTIONS)
Options related to the indexing of the contents of the resources.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPEN_FIND_RESOURCE_SEARCHING_OPTIONS](#OPEN_FIND_RESOURCE_SEARCHING_OPTIONS)
Options related to the searching in contents of the resources.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPEN_MERGED_FILES](#OPEN_MERGED_FILES)
Open the modified files after the merge operation is performed
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PREFER_USING_KEYS_FOR_DITA_CROSS_REF](#PREFER_USING_KEYS_FOR_DITA_CROSS_REF)
Boolean option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PREFER_USING_KEYS_FOR_DITA_FILE_REFERENCE](#PREFER_USING_KEYS_FOR_DITA_FILE_REFERENCE)
Boolean option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PREFER_USING_KEYS_FOR_DITA_INSERT_MEDIA](#PREFER_USING_KEYS_FOR_DITA_INSERT_MEDIA)
Boolean option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PREFER_USING_KEYS_FOR_DITA_PUSH_CONTENT](#PREFER_USING_KEYS_FOR_DITA_PUSH_CONTENT)
Boolean option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PREFER_USING_KEYS_FOR_DITA_REUSE_CONTENT](#PREFER_USING_KEYS_FOR_DITA_REUSE_CONTENT)
Boolean option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PREFER_USING_KEYS_FOR_DITA_WEB_LINK](#PREFER_USING_KEYS_FOR_DITA_WEB_LINK)
Boolean option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROFILING_CONDITIONS_LIST](#PROFILING_CONDITIONS_LIST)
Stores information about the profiling conditions.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROFILING_CONDITIONS_SET_LIST](#PROFILING_CONDITIONS_SET_LIST)
Stores information about the profiling conditions sets.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROFILING_SHOW_ATTRIBUTES_COLORS](#PROFILING_SHOW_ATTRIBUTES_COLORS)
Key used to store information about the profiling conditions colors.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PROFILING_STYLES](#PROFILING_STYLES)
Option key for profiling styles associated with a profiling attribute value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RECENTLY_USED_CHARACTERS](#RECENTLY_USED_CHARACTERS)
Option for storing the recently used characters from CharacterMap.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RECENTLY_USED_CHARACTERS_SIZE](#RECENTLY_USED_CHARACTERS_SIZE)
The number of recently used characters that must be stored.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [REPORT_INVALID_ATTR_VALS_FOUND_IN_DOC](#REPORT_INVALID_ATTR_VALS_FOUND_IN_DOC)
Boolean option from the Profiling and Conditional Text options page which when set to true will report warnings if the current validated file has profiling attributes with values which are not defined in the application preferences "Profiling and Conditional Text" page.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RESTRICT_EDITING_REFERRED_CONTENT_TO_LOCAL_FILES_IN_AUTHOR](#RESTRICT_EDITING_REFERRED_CONTENT_TO_LOCAL_FILES_IN_AUTHOR)
Boolean option to allow editing also referred remote files false to allow editing of referred remote files.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_EXCLUDED_CONTENT](#SHOW_EXCLUDED_CONTENT)
"Show Excluded Content" option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_PROFILING_ATTRIBUTES](#SHOW_PROFILING_ATTRIBUTES)
"Show Profiling Attributes" option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_PROFILING_COLORS_AND_STYLES](#SHOW_PROFILING_COLORS_AND_STYLES)
"Show Profiling Colors and Styles" option.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_SAVE_AS_IN_NEW_DIALOG](#SHOW_SAVE_AS_IN_NEW_DIALOG)
Show "Save As" capability in New wizard dialog.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SPELL_CHECK_OPTIONS](#SPELL_CHECK_OPTIONS)
Can be used to set and obtain a persistent object of type "ro.sync.azcheck.ui.SpellCheckOptions" which contains information about the current spell checker language, automatic spell check state and so on.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SQF_QUICK_FIX_SUPPORT](#SQF_QUICK_FIX_SUPPORT)
Option that controls if the schematron quick fixes support is enabled or not.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SYNTAX_HIGHLIGHT_PROXY_MAP_BG_COLORS](#SYNTAX_HIGHLIGHT_PROXY_MAP_BG_COLORS)
Background colors for the "Editor / Syntax Highlight / Elements/Attributes by Prefix" preferences page.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SYNTAX_HIGHLIGHT_PROXY_MAP_COLORS](#SYNTAX_HIGHLIGHT_PROXY_MAP_COLORS)
Foreground colors for the "Editor / Syntax Highlight / Elements/Attributes by Prefix" preferences page.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SYNTAX_HIGHLIGHT_PROXY_MAP_PROXIES](#SYNTAX_HIGHLIGHT_PROXY_MAP_PROXIES)
List of XML prefixes for which the syntax highlight will have various foreground/background colors.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TAGS_COMPACT_MODE](#TAGS_COMPACT_MODE)
Compact layout for tags.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TAGS_DISPLAY_MODE](#TAGS_DISPLAY_MODE)
Tags display mode in tagless editor.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TRACK_CHANGES_INITIAL_DISPLAY_MODE](#TRACK_CHANGES_INITIAL_DISPLAY_MODE)
Option for track changes initial display mode (view changes/comments, view final, ...).
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [TRACK_CHANGES_INITIAL_STATE](#TRACK_CHANGES_INITIAL_STATE)
Option for track changes initial state.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_BACKGROUND_COLOR](#UI_BACKGROUND_COLOR)
Background color for user interface.Return a string containing the color RGB with comma delimiters.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_BORDER_COLOR](#UI_BORDER_COLOR)
Border color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_DARK_THEME](#UI_DARK_THEME)
true if the current theme is a dark one.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_DISABLED_FOREGROUND_COLOR](#UI_DISABLED_FOREGROUND_COLOR)
Disabled foreground color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_FOREGROUND_COLOR](#UI_FOREGROUND_COLOR)
Foreground color for user interface.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_INACTIVE_SELECTION_BACKGROUND_COLOR](#UI_INACTIVE_SELECTION_BACKGROUND_COLOR)
Inactive selection background color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_LINK_FOREGROUND_COLOR](#UI_LINK_FOREGROUND_COLOR)
Link foreground color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_MENUS_TOOLBARS_BACKGROUND_COLOR](#UI_MENUS_TOOLBARS_BACKGROUND_COLOR)
Background color for toolbars and menus.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_MENUS_TOOLBARS_SELECTION_BACKGROUND_COLOR](#UI_MENUS_TOOLBARS_SELECTION_BACKGROUND_COLOR)
Selection background color for toolbars and menus.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_SCROLLBARS_CHEVRONS_COLOR](#UI_SCROLLBARS_CHEVRONS_COLOR)
Color for scroll bars, chevrons.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_SELECTION_BACKGROUND_COLOR](#UI_SELECTION_BACKGROUND_COLOR)
Selection background color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_SELECTION_FOREGROUND_COLOR](#UI_SELECTION_FOREGROUND_COLOR)
Selection foreground color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_SEPARATOR_COLOR](#UI_SEPARATOR_COLOR)
Separator color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_STATUS_PANEL_BACKGROUND_COLOR](#UI_STATUS_PANEL_BACKGROUND_COLOR)
Background color for status panel.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_STATUS_PANEL_FOREGROUND_COLOR](#UI_STATUS_PANEL_FOREGROUND_COLOR)
Foreground color for status panel.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_TEXT_BACKGROUND_COLOR](#UI_TEXT_BACKGROUND_COLOR)
Background color for text components, trees, tables.Returns a string containing the color RGB with comma delimiters.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_TEXT_COMPONENTS_BORDER_COLOR](#UI_TEXT_COMPONENTS_BORDER_COLOR)
Border color for text components, trees, tables.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_VIEW_TABS_BORDER_COLOR](#UI_VIEW_TABS_BORDER_COLOR)
Color for view tabs border.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_VIEW_TITLES_BACKGROUND_COLOR](#UI_VIEW_TITLES_BACKGROUND_COLOR)
View titles background color.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_VIEW_TITLES_FONT](#UI_VIEW_TITLES_FONT)
Font for view titles.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UI_VIEW_TITLES_FOREGROUND_COLOR](#UI_VIEW_TITLES_FOREGROUND_COLOR)
Foreground color for view titles.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [USE_CUSTOM_FRAMEWORKS_DIRECTORY_URL](#USE_CUSTOM_FRAMEWORKS_DIRECTORY_URL)
Options that specifies if the custom frameworks directory is used or not.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [USER_DEFINED_EDITOR_VARIABLES](#USER_DEFINED_EDITOR_VARIABLES)
Option tag used to store user-defined editor variables in Oxygen's preferences.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [XML_DTD_AUTOMATIC_QUICK_FIX_SUPPORT](#XML_DTD_AUTOMATIC_QUICK_FIX_SUPPORT)
Option that controls if the automatic quick fixes support is enabled or not for the XML validated with DTD.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [XML_RNG_AUTOMATIC_QUICK_FIX_SUPPORT](#XML_RNG_AUTOMATIC_QUICK_FIX_SUPPORT)
Option that controls if the automatic quick fixes support is enabled or not for the XML validated with RNG.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [XML_XSD_AUTOMATIC_QUICK_FIX_SUPPORT](#XML_XSD_AUTOMATIC_QUICK_FIX_SUPPORT)
Option that controls if the automatic quick fixes support is enabled or not for the XML validated with XSD.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [XSL_AUTOMATIC_QUICK_FIX_SUPPORT](#XSL_AUTOMATIC_QUICK_FIX_SUPPORT)
Option that controls if the automatic quick fixes support is enabled or not for XSLT.

## Field Details

### OPEN_FIND_RESOURCE_SEARCHING_OPTIONS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPEN_FIND_RESOURCE_SEARCHING_OPTIONS

Options related to the searching in contents of the resources.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.OPEN_FIND_RESOURCE_SEARCHING_OPTIONS)

### OPEN_FIND_RESOURCE_INDEXING_OPTIONS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPEN_FIND_RESOURCE_INDEXING_OPTIONS

Options related to the indexing of the contents of the resources.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.OPEN_FIND_RESOURCE_INDEXING_OPTIONS)

### USER_DEFINED_EDITOR_VARIABLES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) USER_DEFINED_EDITOR_VARIABLES

Option tag used to store user-defined editor variables in Oxygen's preferences. The value stored for this tag is an array of UserEditorVariablePO.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.USER_DEFINED_EDITOR_VARIABLES)

### OPEN_MERGED_FILES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPEN_MERGED_FILES

Open the modified files after the merge operation is performed
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.OPEN_MERGED_FILES)

### SHOW_SAVE_AS_IN_NEW_DIALOG

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_SAVE_AS_IN_NEW_DIALOG

Show "Save As" capability in New wizard dialog. Returns a Boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SHOW_SAVE_AS_IN_NEW_DIALOG)

### CREATE_KEYS_ATTRIBUTE_FOR_TOPICREF_BASED_ON_FILENAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CREATE_KEYS_ATTRIBUTE_FOR_TOPICREF_BASED_ON_FILENAME

Option used to generate the "keys" attribute for topicrefs based on the filename (in DMM).
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CREATE_KEYS_ATTRIBUTE_FOR_TOPICREF_BASED_ON_FILENAME)

### AUTO_SYNCHRONIZE_UNMODIFIED_EDITORS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTO_SYNCHRONIZE_UNMODIFIED_EDITORS

Auto synch unmodified editors with file system. Returns a Boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTO_SYNCHRONIZE_UNMODIFIED_EDITORS)

### ENABLE_SYNCHRONIZE_UNMODIFIED_EDITORS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ENABLE_SYNCHRONIZE_UNMODIFIED_EDITORS

Enable update unmodified editors with file system. Returns a Boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.ENABLE_SYNCHRONIZE_UNMODIFIED_EDITORS)

### FILE_TYPES_ASSOCIATION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FILE_TYPES_ASSOCIATION

File type association. Returned as an array of "ro.sync.exml.editor.FileTypeAssociation"
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.FILE_TYPES_ASSOCIATION)

### ADDONS_UPDATE_SITES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDONS_UPDATE_SITES

Array of strings indicating the update sites list. Returns an array of java.lang.String.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.ADDONS_UPDATE_SITES)

### UI_VIEW_TABS_BORDER_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_VIEW_TABS_BORDER_COLOR

Color for view tabs border. Return a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_VIEW_TABS_BORDER_COLOR)

### UI_SCROLLBARS_CHEVRONS_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_SCROLLBARS_CHEVRONS_COLOR

Color for scroll bars, chevrons. Return a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_SCROLLBARS_CHEVRONS_COLOR)

### UI_STATUS_PANEL_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_STATUS_PANEL_BACKGROUND_COLOR

Background color for status panel. Return a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_STATUS_PANEL_BACKGROUND_COLOR)

### UI_STATUS_PANEL_FOREGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_STATUS_PANEL_FOREGROUND_COLOR

Foreground color for status panel. Return a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_STATUS_PANEL_FOREGROUND_COLOR)

### UI_VIEW_TITLES_FOREGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_VIEW_TITLES_FOREGROUND_COLOR

Foreground color for view titles. Return a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_VIEW_TITLES_FOREGROUND_COLOR)

### UI_VIEW_TITLES_FONT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_VIEW_TITLES_FONT

Font for view titles. Return a string containing the font properties with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_VIEW_TITLES_FONT)

### UI_MENUS_TOOLBARS_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_MENUS_TOOLBARS_BACKGROUND_COLOR

Background color for toolbars and menus. Return a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_MENUS_TOOLBARS_BACKGROUND_COLOR)

### UI_MENUS_TOOLBARS_SELECTION_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_MENUS_TOOLBARS_SELECTION_BACKGROUND_COLOR

Selection background color for toolbars and menus. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_MENUS_TOOLBARS_SELECTION_BACKGROUND_COLOR)

### UI_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_BACKGROUND_COLOR

Background color for user interface.Return a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_BACKGROUND_COLOR)

### UI_TEXT_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_TEXT_BACKGROUND_COLOR

Background color for text components, trees, tables.Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_TEXT_BACKGROUND_COLOR)

### UI_VIEW_TITLES_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_VIEW_TITLES_BACKGROUND_COLOR

View titles background color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_VIEW_TITLES_BACKGROUND_COLOR)

### UI_FOREGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_FOREGROUND_COLOR

Foreground color for user interface. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_FOREGROUND_COLOR)

### UI_DISABLED_FOREGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_DISABLED_FOREGROUND_COLOR

Disabled foreground color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_DISABLED_FOREGROUND_COLOR)

### UI_SELECTION_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_SELECTION_BACKGROUND_COLOR

Selection background color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_SELECTION_BACKGROUND_COLOR)

### UI_INACTIVE_SELECTION_BACKGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_INACTIVE_SELECTION_BACKGROUND_COLOR

Inactive selection background color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_INACTIVE_SELECTION_BACKGROUND_COLOR)

### UI_SELECTION_FOREGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_SELECTION_FOREGROUND_COLOR

Selection foreground color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_SELECTION_FOREGROUND_COLOR)

### UI_LINK_FOREGROUND_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_LINK_FOREGROUND_COLOR

Link foreground color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_LINK_FOREGROUND_COLOR)

### UI_BORDER_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_BORDER_COLOR

Border color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_BORDER_COLOR)

### UI_SEPARATOR_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_SEPARATOR_COLOR

Separator color. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_SEPARATOR_COLOR)

### UI_DARK_THEME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_DARK_THEME

true if the current theme is a dark one. Returns a boolean.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_DARK_THEME)

### UI_TEXT_COMPONENTS_BORDER_COLOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UI_TEXT_COMPONENTS_BORDER_COLOR

Border color for text components, trees, tables. Returns a string containing the color RGB with comma delimiters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.UI_TEXT_COMPONENTS_BORDER_COLOR)

### DITA_SHOW_CONSOLE_OUTPUT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_SHOW_CONSOLE_OUTPUT

Option regarding when to show the DITA transformation console output. Returns an integer property, one of the constants [APIOptionConstants.ALWAYS_SHOW_CONSOLE](APIOptionConstants.md#ALWAYS_SHOW_CONSOLE). [APIOptionConstants.SHOW_CONSOLE_WHEN_BUILD_FAILS](APIOptionConstants.md#SHOW_CONSOLE_WHEN_BUILD_FAILS)
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_SHOW_CONSOLE_OUTPUT)

### DITA_OT_DIRECTORY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_OT_DIRECTORY

DITA OT Directory. Returns a String representing the directory path to the default DITA OT directory.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_OT_DIRECTORY)

### TRACK_CHANGES_INITIAL_STATE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TRACK_CHANGES_INITIAL_STATE

Option for track changes initial state. Returns an integer value. One of the constants "APIOptionConstants.TRACK_CHANGES_\*".
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.TRACK_CHANGES_INITIAL_STATE)

### TRACK_CHANGES_INITIAL_DISPLAY_MODE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TRACK_CHANGES_INITIAL_DISPLAY_MODE

Option for track changes initial display mode (view changes/comments, view final, ...).
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.TRACK_CHANGES_INITIAL_DISPLAY_MODE)

### PROFILING_SHOW_ATTRIBUTES_COLORS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROFILING_SHOW_ATTRIBUTES_COLORS

Key used to store information about the profiling conditions colors. Returns an ProfilingAttributesPresentingColorsPO object.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PROFILING_SHOW_ATTRIBUTES_COLORS)

### PROFILING_CONDITIONS_SET_LIST

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROFILING_CONDITIONS_SET_LIST

Stores information about the profiling conditions sets. Returns an array of ProfileConditionsSetInfoPO objects.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PROFILING_CONDITIONS_SET_LIST)

### PROFILING_CONDITIONS_LIST

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROFILING_CONDITIONS_LIST

Stores information about the profiling conditions. Returns an array of ProfileConditionInfoPO objects. You can set these from a plugin like this:
```
    ProfileConditionInfoPO[] conditions = new ro.sync.ecss.conditions.ProfileConditionInfoPO[]{
        new ProfileConditionInfoPO("dummy", "Dummy", true, new ro.sync.ecss.conditions.ProfileConditionValuePO[]{
            new ProfileConditionValuePO("external", "External"),
            new ProfileConditionValuePO("guest", "Guest"),
            new ProfileConditionValuePO("internal", "Internal"),
        }, " ", "*DITA*")
    };
    PluginWorkspaceProvider.getPluginWorkspace().setGlobalObjectProperty("profiling.conditions.list", conditions);
```
The constructor of the ProfileConditionInfoPO persistent object looks like:
```

  public static ProfileConditionInfoPO createDefaultProfileConditionInfoPO(String attributeName, String attributeRenderName,
      boolean allowsMultipleValues, String[] allowedValues, String valuesSeparator, String documentTypePattern) {

```

  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PROFILING_CONDITIONS_LIST)

### PROFILING_STYLES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PROFILING_STYLES

Option key for profiling styles associated with a profiling attribute value. Returns an array of ProfilingAttributeStylePO objects. You can set these from a plugin like this:
```
    PluginWorkspaceProvider.getPluginWorkspace().setGlobalObjectProperty("author.profiling.styles", new ProfilingAttributeStylePO[]{
        new ProfilingAttributeStylePO("#DITA*", "dummy", "External", Color.BLUE.getRGB(), ProfilingAttributeStylePO.NO_COLOR, ProfilingAttributeStylePO.UNDERLINE, false, false),
        new ProfilingAttributeStylePO("#DITA*", "dummy", "Guest", Color.RED.getRGB(), ProfilingAttributeStylePO.NO_COLOR, ProfilingAttributeStylePO.DOUBLE_UNDERLINE, false, false),
    });
```
The constructor of the ProfilingAttributeStylePO looks like this:
```
public ProfilingAttributeStylePO(String framework, String attributeName,
      String attributeValue, int foreground, int background, String textDecoration,
      boolean bold, boolean italic)
```

  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PROFILING_STYLES)

### CAN_EDIT_READ_ONLY_FILES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CAN_EDIT_READ_ONLY_FILES

Option for editing read-only files. Returns a Boolean flag.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CAN_EDIT_READ_ONLY_FILES)

### CATALOGS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CATALOGS

The catalogs key. Returns an array of Strings, each string being an URL-like path to a catalog file. PLEASE DO NOT CHANGE THE KEY NAME, LOTS OF CUSTOMIZERS (IXIASOFT FOR EXAMPLE) USE THIS KEY TO IMPOSE CATALOGS.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CATALOGS)

### RECENTLY_USED_CHARACTERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RECENTLY_USED_CHARACTERS

Option for storing the recently used characters from CharacterMap. It's a Java String in which each char is one of the characters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.RECENTLY_USED_CHARACTERS)

### RECENTLY_USED_CHARACTERS_SIZE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RECENTLY_USED_CHARACTERS_SIZE

The number of recently used characters that must be stored. It is an integer property.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.RECENTLY_USED_CHARACTERS_SIZE)

### TAGS_DISPLAY_MODE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TAGS_DISPLAY_MODE

Tags display mode in tagless editor. It is an integer property, one of the constants in the ro.sync.exml.workspace.api.editor.page.author.DisplayModeConstants interface.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.TAGS_DISPLAY_MODE)

### AUTOMATICALLY_ACCEPT_CERTIFICATES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTOMATICALLY_ACCEPT_CERTIFICATES

Option that controls if oXygen will accept all HTTPS certificates.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTOMATICALLY_ACCEPT_CERTIFICATES)

### ADDITIONAL_FRAMEWORKS_DIRECTORIES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDITIONAL_FRAMEWORKS_DIRECTORIES

Array of strings indicating the additional frameworks directories. Returns an array of java.lang.String objects representing paths to the additional frameworks folders, paths which may also contain editor variables.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.ADDITIONAL_FRAMEWORKS_DIRECTORIES)

### FRAMEWORKS_DIRECTORY_URL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FRAMEWORKS_DIRECTORY_URL

The custom frameworks directory URL with editor variables, when a custom one is set. It has a string value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.FRAMEWORKS_DIRECTORY_URL)

### USE_CUSTOM_FRAMEWORKS_DIRECTORY_URL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) USE_CUSTOM_FRAMEWORKS_DIRECTORY_URL

Options that specifies if the custom frameworks directory is used or not. It has a boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.USE_CUSTOM_FRAMEWORKS_DIRECTORY_URL)

### SYNTAX_HIGHLIGHT_PROXY_MAP_COLORS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SYNTAX_HIGHLIGHT_PROXY_MAP_COLORS

Foreground colors for the "Editor / Syntax Highlight / Elements/Attributes by Prefix" preferences page. It takes a string containing color RGB values having the pattern: "R1,G1,B1;R2,G2,B2". Sample value for 3 colors: "10,10,20;20,20,30;30,31,32"
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SYNTAX_HIGHLIGHT_PROXY_MAP_COLORS)

### SYNTAX_HIGHLIGHT_PROXY_MAP_BG_COLORS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SYNTAX_HIGHLIGHT_PROXY_MAP_BG_COLORS

Background colors for the "Editor / Syntax Highlight / Elements/Attributes by Prefix" preferences page. It takes a string containing color RGB values having the pattern: "R1,G1,B1;R2,G2,B2". Sample value for 2 colors: "255,255,255;255,255,255"
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SYNTAX_HIGHLIGHT_PROXY_MAP_BG_COLORS)

### SYNTAX_HIGHLIGHT_PROXY_MAP_PROXIES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SYNTAX_HIGHLIGHT_PROXY_MAP_PROXIES

List of XML prefixes for which the syntax highlight will have various foreground/background colors. Its value is a String array like for example: new String[]{"p1", "p2", "p3"}. Example of how such option tags can be set:
```

    //Foreground colors
     pluginWorkspaceAccess.setGlobalObjectProperty("sh.proxy.map.colors.second", "10,10,20;20,20,30;30,31,32");
     //Background colors, same syntax, all white
     pluginWorkspaceAccess.setGlobalObjectProperty("sh.proxy.map.bg.colors.second", "255,255,255;255,255,255;255,255,255");
     //The set of prefixes...
     pluginWorkspaceAccess.setGlobalObjectProperty("sh.proxy.map.proxies", new String[]{"p1", "p2", "p3"});

```

  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SYNTAX_HIGHLIGHT_PROXY_MAP_PROXIES)

### XML_DTD_AUTOMATIC_QUICK_FIX_SUPPORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) XML_DTD_AUTOMATIC_QUICK_FIX_SUPPORT

Option that controls if the automatic quick fixes support is enabled or not for the XML validated with DTD.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.XML_DTD_AUTOMATIC_QUICK_FIX_SUPPORT)

### XML_RNG_AUTOMATIC_QUICK_FIX_SUPPORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) XML_RNG_AUTOMATIC_QUICK_FIX_SUPPORT

Option that controls if the automatic quick fixes support is enabled or not for the XML validated with RNG. It has a boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.XML_RNG_AUTOMATIC_QUICK_FIX_SUPPORT)

### XML_XSD_AUTOMATIC_QUICK_FIX_SUPPORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) XML_XSD_AUTOMATIC_QUICK_FIX_SUPPORT

Option that controls if the automatic quick fixes support is enabled or not for the XML validated with XSD. It has a boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.XML_XSD_AUTOMATIC_QUICK_FIX_SUPPORT)

### XSL_AUTOMATIC_QUICK_FIX_SUPPORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) XSL_AUTOMATIC_QUICK_FIX_SUPPORT

Option that controls if the automatic quick fixes support is enabled or not for XSLT. It has a boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.XSL_AUTOMATIC_QUICK_FIX_SUPPORT)

### SQF_QUICK_FIX_SUPPORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SQF_QUICK_FIX_SUPPORT

Option that controls if the schematron quick fixes support is enabled or not. It has a boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SQF_QUICK_FIX_SUPPORT)

### BULK_APPLY_ONLY_QUICK_FIXES_MARKED_VIA_DEFAULT_FIX_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) BULK_APPLY_ONLY_QUICK_FIXES_MARKED_VIA_DEFAULT_FIX_ATTRIBUTE

Option that controls whether only quick fixes marked via "default-fix" attribute are considered when applying in bulk. It has a boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.BULK_APPLY_ONLY_QUICK_FIXES_MARKED_VIA_DEFAULT_FIX_ATTRIBUTE)

### AUTHOR_FORMAT_COMPATIBILITY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTHOR_FORMAT_COMPATIBILITY

Option for controlling the compatibility of the document serialization from Author editing mode with other tools. Returns an integer property, one of the constants [AuthorFormatCompatibilityModeConstants.FORMAT_COMPATIBILITY_BREAKS_LINES_ONLY_BLOCKS_DO_NO_INDENT](../../ecss/dom/builder/AuthorFormatCompatibilityModeConstants.md#FORMAT_COMPATIBILITY_BREAKS_LINES_ONLY_BLOCKS_DO_NO_INDENT), [AuthorFormatCompatibilityModeConstants.FORMAT_COMPATIBILITY_DO_NOT_BREAK_LINES_DO_NO_INDENT](../../ecss/dom/builder/AuthorFormatCompatibilityModeConstants.md#FORMAT_COMPATIBILITY_DO_NOT_BREAK_LINES_DO_NO_INDENT), [AuthorFormatCompatibilityModeConstants.FORMAT_COMPATIBILITY_NONE](../../ecss/dom/builder/AuthorFormatCompatibilityModeConstants.md#FORMAT_COMPATIBILITY_NONE),
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTHOR_FORMAT_COMPATIBILITY)

### CODE_INSIGHT_SHOW_ANNOTATIONS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CODE_INSIGHT_SHOW_ANNOTATIONS

Show annotations (documentation) for each entry in the content completion window. Boolean option.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CODE_INSIGHT_SHOW_ANNOTATIONS)

### CODE_INSIGHT_SHOW_ANNOTATIONS_TOOLTIP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CODE_INSIGHT_SHOW_ANNOTATIONS_TOOLTIP

Show annotations (documentation) when hovering the mouse over various elements. Boolean option.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CODE_INSIGHT_SHOW_ANNOTATIONS_TOOLTIP)

### ARCHIVE_DESCRIPTORS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARCHIVE_DESCRIPTORS

All the extensions recognized as archives. Its value is an array of "ro.sync.exml.zip.ArchiveDescriptor" objects. You can set it to register your own custom archive extension like:
```
PluginWorkspaceProvider.getPluginWorkspace().setGlobalObjectProperty(ro.sync.exml.options.APIAccessibleOptionTags.ARCHIVE_DESCRIPTORS, new ArchiveDescriptor[]{new ArchiveDescriptor("EPX files", new String[]{"epx"}, ArchiveDescriptor.ARCHIVE_TYPE_ZIP)});
```

  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.ARCHIVE_DESCRIPTORS)

### SPELL_CHECK_OPTIONS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SPELL_CHECK_OPTIONS

Can be used to set and obtain a persistent object of type "ro.sync.azcheck.ui.SpellCheckOptions" which contains information about the current spell checker language, automatic spell check state and so on.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SPELL_CHECK_OPTIONS)

### PREFER_USING_KEYS_FOR_DITA_REUSE_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PREFER_USING_KEYS_FOR_DITA_REUSE_CONTENT

Boolean option. If true the "Reuse content" dialog will have the "Key" radio button selected.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PREFER_USING_KEYS_FOR_DITA_REUSE_CONTENT)

### PREFER_USING_KEYS_FOR_DITA_CROSS_REF

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PREFER_USING_KEYS_FOR_DITA_CROSS_REF

Boolean option. If true the "Cross reference" and "Related link to topic" dialogs will have the "Key" radio button selected.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PREFER_USING_KEYS_FOR_DITA_CROSS_REF)

### PREFER_USING_KEYS_FOR_DITA_PUSH_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PREFER_USING_KEYS_FOR_DITA_PUSH_CONTENT

Boolean option. If true the "Push content" dialog will have the "Key" radio button selected.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PREFER_USING_KEYS_FOR_DITA_PUSH_CONTENT)

### PREFER_USING_KEYS_FOR_DITA_INSERT_MEDIA

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PREFER_USING_KEYS_FOR_DITA_INSERT_MEDIA

Boolean option. If true the "Insert media" dialog will have the "Key" radio button selected.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PREFER_USING_KEYS_FOR_DITA_INSERT_MEDIA)

### PREFER_USING_KEYS_FOR_DITA_FILE_REFERENCE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PREFER_USING_KEYS_FOR_DITA_FILE_REFERENCE

Boolean option. If true the "File reference" and "Related link to file" dialogs will have the "Key" radio button selected.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PREFER_USING_KEYS_FOR_DITA_FILE_REFERENCE)

### PREFER_USING_KEYS_FOR_DITA_WEB_LINK

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PREFER_USING_KEYS_FOR_DITA_WEB_LINK

Boolean option. If true the "Web link" and "Related link to webpage" dialogs will have the "Key" radio button selected.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.PREFER_USING_KEYS_FOR_DITA_WEB_LINK)

### DITA_FILL_TOPICREF_FORMAT_ATTR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_FILL_TOPICREF_FORMAT_ATTR

Option that controls if the format attribute value will be automatically filled when inserting a topic reference.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_FILL_TOPICREF_FORMAT_ATTR)

### DITA_FILL_TOPICREF_SCOPE_ATTR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_FILL_TOPICREF_SCOPE_ATTR

Option that controls if the scope attribute value will be automatically filled when inserting a topic reference.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_FILL_TOPICREF_SCOPE_ATTR)

### DITA_FILL_TOPICREF_TYPE_ATTR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_FILL_TOPICREF_TYPE_ATTR

Option that controls if the type attribute value will be automatically filled when inserting a topic reference.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_FILL_TOPICREF_TYPE_ATTR)

### DITA_FILL_TOPICREF_NAVTITLE_ATTR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_FILL_TOPICREF_NAVTITLE_ATTR

Option that controls if the navigation title attribute value will be automatically filled when inserting a topic reference.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_FILL_TOPICREF_NAVTITLE_ATTR)

### DITA_FILL_LINK_FORMAT_ATTR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_FILL_LINK_FORMAT_ATTR

Option that controls if the format attribute value will be automatically filled when inserting a link reference.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_FILL_LINK_FORMAT_ATTR)

### DITA_FILL_LINK_SCOPE_ATTR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_FILL_LINK_SCOPE_ATTR

Option that controls if the scope attribute value will be automatically filled when inserting a link reference.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_FILL_LINK_SCOPE_ATTR)

### DITA_FILL_LINK_TYPE_ATTR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DITA_FILL_LINK_TYPE_ATTR

Option that controls if the type attribute value will be automatically filled when inserting a link reference.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DITA_FILL_LINK_TYPE_ATTR)

### EDITOR_SHOW_TAB_EOL_EOF

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_SHOW_TAB_EOL_EOF

Boolean property for displaying the characters TAB, END-OF-LINE and END-OF-FILE as special marks or not displaying them.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_SHOW_TAB_EOL_EOF)

### EDITOR_SHOW_SPACE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_SHOW_SPACE

Boolean property for displaying the SPACE characters as special marks or not displaying them in oXygen editors.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_SHOW_SPACE)

### SHOW_PROFILING_COLORS_AND_STYLES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_PROFILING_COLORS_AND_STYLES

"Show Profiling Colors and Styles" option. Returns a Boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SHOW_PROFILING_COLORS_AND_STYLES)

### SHOW_PROFILING_ATTRIBUTES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_PROFILING_ATTRIBUTES

"Show Profiling Attributes" option. Returns a Boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SHOW_PROFILING_ATTRIBUTES)

### SHOW_EXCLUDED_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_EXCLUDED_CONTENT

"Show Excluded Content" option. Returns a Boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.SHOW_EXCLUDED_CONTENT)

### CODE_TEMPLATES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CODE_TEMPLATES

Code-templates. Can be used to set or retrieve an array of "ro.sync.contentcompletion.CTItem".
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CODE_TEMPLATES)

### REPORT_INVALID_ATTR_VALS_FOUND_IN_DOC

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) REPORT_INVALID_ATTR_VALS_FOUND_IN_DOC

Boolean option from the Profiling and Conditional Text options page which when set to true will report warnings if the current validated file has profiling attributes with values which are not defined in the application preferences "Profiling and Conditional Text" page.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.REPORT_INVALID_ATTR_VALS_FOUND_IN_DOC)

### CHANGE_TRACKING_AUTHOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CHANGE_TRACKING_AUTHOR

The author for change tracking. Returns a String value and defaults to the user name set in the system.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CHANGE_TRACKING_AUTHOR)

### EDITOR_FONT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_FONT

A property with a string value of the form "name,style,size". For example: "MS Gothic,0,15" where "0" style means plain font, "1" means bold font and "2" means italic font. Keep the font used for displaying the documents in the editor panels.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_FONT)

### FONT_FOR_AUTHOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FONT_FOR_AUTHOR

The default font for the author editor. A property with a string value of the form "name,style,size". For example: "MS Gothic,0,15" where "0" style means plain font, "1" means bold font and "2" means italic font.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.FONT_FOR_AUTHOR)

### FONT_FOR_TEXT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FONT_FOR_TEXT

The font for the text controls. A property with a string value of the form "name,style,size". For example: "MS Gothic,0,15" where "0" style means plain font, "1" means bold font and "2" means italic font.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.FONT_FOR_TEXT)

### FONT_FOR_GUI

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FONT_FOR_GUI

The font for the GUI controls. A property with a string value of the form "name,style,size". For example: "MS Gothic,0,15" where "0" style means plain font, "1" means bold font and "2" means italic font.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.FONT_FOR_GUI)

### FONT_FOR_SCHEMA

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FONT_FOR_SCHEMA

The default font for the schema editor. A property with a string value of the form "name,style,size". For example: "MS Gothic,0,15" where "0" style means plain font, "1" means bold font and "2" means italic font.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.FONT_FOR_SCHEMA)

### KEYS_CONTEXT_MAP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) KEYS_CONTEXT_MAP

The keys context map. It's value is a string containing an URL-like path.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.KEYS_CONTEXT_MAP)

### EDITOR_LINE_WIDTH

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_LINE_WIDTH

The maximum length of any line when the Format and Indent (pretty-print) operation is applied. This value is superseded only if the property "Detect line width on open" is enabled. A property which accepts an integer value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_LINE_WIDTH)

### EDITOR_FORMAT_INDENT_INLINE_ELEMENTS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_FORMAT_INDENT_INLINE_ELEMENTS

Indent inline elements. Returns a Boolean value.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_FORMAT_INDENT_INLINE_ELEMENTS)

### EDITOR_DETECT_INDENT_ON_OPEN

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_DETECT_INDENT_ON_OPEN

Boolean property. If it is enabled the indenting of the document (use tabs or spaces, indent size) is discovered when the user opens the document for editing in an editor panel and it will be preserved when the user applies the Format and Indent (pretty-print) action.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_DETECT_INDENT_ON_OPEN)

### EDITOR_USE_TABS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_USE_TABS

If enabled the indentation will be made with tab characters, if disabled the indentation will be made with space characters.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_USE_TABS)

### EDITOR_INDENT_SIZE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDITOR_INDENT_SIZE

The number of space characters for one indentation level. -- Changed in v9.2 because the indent size must be greater than 0.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDITOR_INDENT_SIZE)

### AUTORECOVERY_LOCATION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTORECOVERY_LOCATION

A filepath string property defining the folder where the auto-recovery information for documents is stored. By default its value is:- **Windows Vista/7/8/10:** [user_home_directory]\AppData\Roaming\com.oxygenxml\autorecover- **Mac OS X:** [user_home_directory]/Library/Preferences/com.oxygenxml/autorecover- **Linux/Unix:** [user_home_directory]/.com.oxygenxml/autorecover
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTORECOVERY_LOCATION)

### AUTOCHECKVERSION_ENABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTOCHECKVERSION_ENABLE

Boolean property. If true the user wants to check automatically if a new version of oXygen was released.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTOCHECKVERSION_ENABLE)

### CHECK_FOR_NOTIFICATIONS_ENABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CHECK_FOR_NOTIFICATIONS_ENABLE

Boolean property. If true the user wants to check for notifications.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.CHECK_FOR_NOTIFICATIONS_ENABLE)

### ENABLE_DITA_2_X_SUPPORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ENABLE_DITA_2_X_SUPPORT

Enable the creation and editing of DITA 2.x documents.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.ENABLE_DITA_2_X_SUPPORT)

### AUTHOR_EDITING_MODE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTHOR_EDITING_MODE

Option controlling the author schema aware editing from the "Editor / Edit Modes / Author / Schema-Aware" Preferences page. Its values are objects of class "ro.sync.ecss.component.AuthorSchemaAwareOptions"
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTHOR_EDITING_MODE)

### EDIT_RESOLVED_REFERRED_CONTENT_IN_AUTHOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDIT_RESOLVED_REFERRED_CONTENT_IN_AUTHOR

Boolean option to allow in-place editing for referred content in Author page.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.EDIT_RESOLVED_REFERRED_CONTENT_IN_AUTHOR)

### RESTRICT_EDITING_REFERRED_CONTENT_TO_LOCAL_FILES_IN_AUTHOR

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RESTRICT_EDITING_REFERRED_CONTENT_TO_LOCAL_FILES_IN_AUTHOR

Boolean option to allow editing also referred remote files false to allow editing of referred remote files.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.RESTRICT_EDITING_REFERRED_CONTENT_TO_LOCAL_FILES_IN_AUTHOR)

### ASK_OPEN_DITA_MAP_IN_DITAMANAGER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ASK_OPEN_DITA_MAP_IN_DITAMANAGER

Remember if Oxygen should ask the user if the dita map will be opened in the dita maps manager.Possible integer values:ro.sync.exml.options.APIOptionConstants.ALWAYS_ASKro.sync.exml.options.APIOptionConstants.ALWAYS_NOro.sync.exml.options.APIOptionConstants.ALWAYS_YES
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.ASK_OPEN_DITA_MAP_IN_DITAMANAGER)

### DIFF_IGNORE_XPATH_EXPRESSION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DIFF_IGNORE_XPATH_EXPRESSION

Option used to store the XPath expression used to ignore nodes when files are compared. Its value is a string.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DIFF_IGNORE_XPATH_EXPRESSION)

### DIFF_INFO

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DIFF_INFO

The current diff info. Holds a ro.sync.diff.factory.DiffInfo object.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.DIFF_INFO)

### AUTO_APPLY_STYLES_DITAVAL_MAIN_FILES

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTO_APPLY_STYLES_DITAVAL_MAIN_FILES

Boolean value which controls applying styles defined in ditaval files placed in main files folder
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTO_APPLY_STYLES_DITAVAL_MAIN_FILES)

### AUTHOR_DISPLAY_REFERENCES_EXPANDED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) AUTHOR_DISPLAY_REFERENCES_EXPANDED

Key for display references expanded author option. Has boolean value, true by default.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.AUTHOR_DISPLAY_REFERENCES_EXPANDED)

### TAGS_COMPACT_MODE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) TAGS_COMPACT_MODE

Compact layout for tags. Has boolean value, true by default.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.exml.options.APIAccessibleOptionTags.TAGS_COMPACT_MODE)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
