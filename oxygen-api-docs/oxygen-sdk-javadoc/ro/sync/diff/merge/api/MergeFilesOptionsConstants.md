Package [ro.sync.diff.merge.api](package-summary.md)

# Interface MergeFilesOptionsConstants
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface MergeFilesOptionsConstants
Constants used as keys in the **mergeOptions** map parameter from [DiffAndMergeTools.openMergeApplication(java.io.File, java.io.File, java.io.File, java.util.Map)](../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openMergeApplication(java.io.File,java.io.File,java.io.File,java.util.Map))

## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static interface  [MergeFilesOptionsConstants.FilterModeValues](MergeFilesOptionsConstants.FilterModeValues.md)
The values for filter mode option.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDED_BY_OTHERS](#ADDED_BY_OTHERS)
Merge status: added by others / added remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDED_BY_YOU](#ADDED_BY_YOU)
Merge status: added by you / added locally.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADDED_BY_YOU_AND_BY_OTHERS](#ADDED_BY_YOU_AND_BY_OTHERS)
Merge status: added by you and by others / added both locally and remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DELETED_BY_OTHERS](#DELETED_BY_OTHERS)
Merge status: deleted by others / deleted remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DELETED_BY_YOU](#DELETED_BY_YOU)
Merge status: deleted by you / deleted locally
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DELETED_BY_YOU_AND_BY_OTHERS](#DELETED_BY_YOU_AND_BY_OTHERS)
Merge status: deleted by you and by others / deleted both locally and remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DELETED_BY_YOU_AND_MODIFIED_BY_OTHERS](#DELETED_BY_YOU_AND_MODIFIED_BY_OTHERS)
Merge status: deleted by you and modified by others / deleted locally but modified remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FILTER_MODES_KEY](#FILTER_MODES_KEY)
This option controls the default state of the filter buttons from the merge dialog.Only one filter can be applied.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LEFT_DIFF_PANEL_DESCRIPTION](#LEFT_DIFF_PANEL_DESCRIPTION)
Label for the left diff panel description.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MERGE_DIALOG_TITLE](#MERGE_DIALOG_TITLE)
This option controls the title of the merge dialog.If this option is set, its value will be used as the title of the merge dialog.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MERGE_OPERATION_SUMMARY_CHANGE_MADE_BY_OTHERS_LABEL](#MERGE_OPERATION_SUMMARY_CHANGE_MADE_BY_OTHERS_LABEL)
A label that the merge operation summary explanatory text consists of.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MERGE_OPERATION_SUMMARY_CONFLICTS_LABEL](#MERGE_OPERATION_SUMMARY_CONFLICTS_LABEL)
A label that the merge operation summary explanatory text consists of.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MERGE_OPERATION_SUMMARY_NO_CHANGES_FOUND_LABEL](#MERGE_OPERATION_SUMMARY_NO_CHANGES_FOUND_LABEL)
A label that the merge operation summary explanatory text consists of.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MERGE_OPERATION_SUMMARY_YOUR_CHANGES_LABEL](#MERGE_OPERATION_SUMMARY_YOUR_CHANGES_LABEL)
A label that the merge operation summary explanatory text consists of.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MODIFIED_BY_OTHERS](#MODIFIED_BY_OTHERS)
Merge status: modified by others / modified remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MODIFIED_BY_YOU](#MODIFIED_BY_YOU)
Merge status: modified by you / modified locally.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MODIFIED_BY_YOU_AND_BY_OTHERS](#MODIFIED_BY_YOU_AND_BY_OTHERS)
Merge status: modified by you and by others / modified both locally and remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MODIFIED_BY_YOU_AND_BY_OTHERS_MERGEABLE](#MODIFIED_BY_YOU_AND_BY_OTHERS_MERGEABLE)
Merge status: modified by you and by others / modified both locally and remotely; can be merged automatically, no real conflicts.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [MODIFIED_BY_YOU_AND_DELETED_BY_OTHERS](#MODIFIED_BY_YOU_AND_DELETED_BY_OTHERS)
Merge status: modified by you and deleted by others / modified locally but deleted remotely.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [NOT_MODIFIED](#NOT_MODIFIED)
Merge status: not modified.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [RIGHT_DIFF_PANEL_DESCRIPTION](#RIGHT_DIFF_PANEL_DESCRIPTION)
Label for the right diff panel description.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_ALL_FILES_TOOLTIP](#SHOW_ALL_FILES_TOOLTIP)
Show all files filter button tooltip
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_ONLY_CONFLICTING_FILES_TOOLTIP](#SHOW_ONLY_CONFLICTING_FILES_TOOLTIP)
Show only conflicting files filter button tooltip
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_ONLY_FILES_MODIFIED_BY_OTHERS_TOOLTIP](#SHOW_ONLY_FILES_MODIFIED_BY_OTHERS_TOOLTIP)
Show only files modified by others filter button tooltip
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_ONLY_FILES_MODIFIED_BY_YOU_AND_OTHERS_TOOLTIP](#SHOW_ONLY_FILES_MODIFIED_BY_YOU_AND_OTHERS_TOOLTIP)
Show only files modified by you and others filter button tooltip
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SHOW_ONLY_FILES_MODIFIED_BY_YOU_TOOLTIP](#SHOW_ONLY_FILES_MODIFIED_BY_YOU_TOOLTIP)
Show only files modified by you filter button tooltip
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [VIRTUAL_PATH_FOR_PERSONAL_MODIFIED_FILES_DIRECTORY](#VIRTUAL_PATH_FOR_PERSONAL_MODIFIED_FILES_DIRECTORY)
If this option is set, its value will be used in the merge dialog to present all the file paths of the files that will be modified as a result of the merge operations.

## Field Details

### VIRTUAL_PATH_FOR_PERSONAL_MODIFIED_FILES_DIRECTORY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) VIRTUAL_PATH_FOR_PERSONAL_MODIFIED_FILES_DIRECTORY

If this option is set, its value will be used in the merge dialog to present all the file paths of the files that will be modified as a result of the merge operations. It can be useful if you plan to do the merging in a temporary directory, and copy all the changes when the dialog is closed. The dialog can use this option to hide the real temporary directory path from the user, using instead the value provided. This is actually a replacement for **personalModifiedFilesDir** (one of the parameters of [DiffAndMergeTools.openMergeApplication(java.io.File, java.io.File, java.io.File, java.util.Map)](../../../exml/workspace/api/standalone/DiffAndMergeTools.md#openMergeApplication(java.io.File,java.io.File,java.io.File,java.util.Map))) in the merge tool UI.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.VIRTUAL_PATH_FOR_PERSONAL_MODIFIED_FILES_DIRECTORY)

### FILTER_MODES_KEY

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FILTER_MODES_KEY

This option controls the default state of the filter buttons from the merge dialog.Only one filter can be applied. The possible values of this option can be found in [MergeFilesOptionsConstants.FilterModeValues](MergeFilesOptionsConstants.FilterModeValues.md).
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.FILTER_MODES_KEY)

### MERGE_DIALOG_TITLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MERGE_DIALOG_TITLE

This option controls the title of the merge dialog.If this option is set, its value will be used as the title of the merge dialog.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MERGE_DIALOG_TITLE)

### SHOW_ALL_FILES_TOOLTIP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_ALL_FILES_TOOLTIP

Show all files filter button tooltip
  Since: 22.1 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.SHOW_ALL_FILES_TOOLTIP)

### SHOW_ONLY_FILES_MODIFIED_BY_OTHERS_TOOLTIP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_ONLY_FILES_MODIFIED_BY_OTHERS_TOOLTIP

Show only files modified by others filter button tooltip
  Since: 22.1 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.SHOW_ONLY_FILES_MODIFIED_BY_OTHERS_TOOLTIP)

### SHOW_ONLY_FILES_MODIFIED_BY_YOU_AND_OTHERS_TOOLTIP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_ONLY_FILES_MODIFIED_BY_YOU_AND_OTHERS_TOOLTIP

Show only files modified by you and others filter button tooltip
  Since: 22.1 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.SHOW_ONLY_FILES_MODIFIED_BY_YOU_AND_OTHERS_TOOLTIP)

### SHOW_ONLY_FILES_MODIFIED_BY_YOU_TOOLTIP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_ONLY_FILES_MODIFIED_BY_YOU_TOOLTIP

Show only files modified by you filter button tooltip
  Since: 22.1 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.SHOW_ONLY_FILES_MODIFIED_BY_YOU_TOOLTIP)

### SHOW_ONLY_CONFLICTING_FILES_TOOLTIP

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SHOW_ONLY_CONFLICTING_FILES_TOOLTIP

Show only conflicting files filter button tooltip
  Since: 22.1 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.SHOW_ONLY_CONFLICTING_FILES_TOOLTIP)

### NOT_MODIFIED

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) NOT_MODIFIED

Merge status: not modified.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.NOT_MODIFIED)

### ADDED_BY_YOU

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDED_BY_YOU

Merge status: added by you / added locally.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.ADDED_BY_YOU)

### ADDED_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDED_BY_OTHERS

Merge status: added by others / added remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.ADDED_BY_OTHERS)

### DELETED_BY_YOU

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DELETED_BY_YOU

Merge status: deleted by you / deleted locally
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.DELETED_BY_YOU)

### DELETED_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DELETED_BY_OTHERS

Merge status: deleted by others / deleted remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.DELETED_BY_OTHERS)

### DELETED_BY_YOU_AND_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DELETED_BY_YOU_AND_BY_OTHERS

Merge status: deleted by you and by others / deleted both locally and remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.DELETED_BY_YOU_AND_BY_OTHERS)

### DELETED_BY_YOU_AND_MODIFIED_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DELETED_BY_YOU_AND_MODIFIED_BY_OTHERS

Merge status: deleted by you and modified by others / deleted locally but modified remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.DELETED_BY_YOU_AND_MODIFIED_BY_OTHERS)

### MODIFIED_BY_YOU

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MODIFIED_BY_YOU

Merge status: modified by you / modified locally.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MODIFIED_BY_YOU)

### MODIFIED_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MODIFIED_BY_OTHERS

Merge status: modified by others / modified remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MODIFIED_BY_OTHERS)

### MODIFIED_BY_YOU_AND_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MODIFIED_BY_YOU_AND_BY_OTHERS

Merge status: modified by you and by others / modified both locally and remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MODIFIED_BY_YOU_AND_BY_OTHERS)

### MODIFIED_BY_YOU_AND_DELETED_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MODIFIED_BY_YOU_AND_DELETED_BY_OTHERS

Merge status: modified by you and deleted by others / modified locally but deleted remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MODIFIED_BY_YOU_AND_DELETED_BY_OTHERS)

### ADDED_BY_YOU_AND_BY_OTHERS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADDED_BY_YOU_AND_BY_OTHERS

Merge status: added by you and by others / added both locally and remotely.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.ADDED_BY_YOU_AND_BY_OTHERS)

### MODIFIED_BY_YOU_AND_BY_OTHERS_MERGEABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MODIFIED_BY_YOU_AND_BY_OTHERS_MERGEABLE

Merge status: modified by you and by others / modified both locally and remotely; can be merged automatically, no real conflicts.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MODIFIED_BY_YOU_AND_BY_OTHERS_MERGEABLE)

### MERGE_OPERATION_SUMMARY_CHANGE_MADE_BY_OTHERS_LABEL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MERGE_OPERATION_SUMMARY_CHANGE_MADE_BY_OTHERS_LABEL

A label that the merge operation summary explanatory text consists of.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MERGE_OPERATION_SUMMARY_CHANGE_MADE_BY_OTHERS_LABEL)

### MERGE_OPERATION_SUMMARY_YOUR_CHANGES_LABEL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MERGE_OPERATION_SUMMARY_YOUR_CHANGES_LABEL

A label that the merge operation summary explanatory text consists of.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MERGE_OPERATION_SUMMARY_YOUR_CHANGES_LABEL)

### MERGE_OPERATION_SUMMARY_CONFLICTS_LABEL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MERGE_OPERATION_SUMMARY_CONFLICTS_LABEL

A label that the merge operation summary explanatory text consists of.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MERGE_OPERATION_SUMMARY_CONFLICTS_LABEL)

### MERGE_OPERATION_SUMMARY_NO_CHANGES_FOUND_LABEL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) MERGE_OPERATION_SUMMARY_NO_CHANGES_FOUND_LABEL

A label that the merge operation summary explanatory text consists of.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.MERGE_OPERATION_SUMMARY_NO_CHANGES_FOUND_LABEL)

### LEFT_DIFF_PANEL_DESCRIPTION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LEFT_DIFF_PANEL_DESCRIPTION

Label for the left diff panel description.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.LEFT_DIFF_PANEL_DESCRIPTION)

### RIGHT_DIFF_PANEL_DESCRIPTION

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) RIGHT_DIFF_PANEL_DESCRIPTION

Label for the right diff panel description.
  Since: 28.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.diff.merge.api.MergeFilesOptionsConstants.RIGHT_DIFF_PANEL_DESCRIPTION)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
