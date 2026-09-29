Package [ro.sync.diff.api](package-summary.md)

# Interface AuthorDiffDirectoriesChangeTrackingMerger
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorDiffDirectoriesChangeTrackingMerger
Merger based on 2-way mode directory comparison which saves the results in a specified directory. All pairs of modified XML files involved in the process are merged by saving the Author mode comparison results as documents with tracked changes that can be later reviewed and accepted / rejected. All the other situations detected are treated based on 2 options applicable to both XML and non-XML files, plus one option applicable to XML files only, plus another option applicable to non-XML files only.
  Since: 26.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [BACKUP_DIRECTORY_NAME_SUFFIX](#BACKUP_DIRECTORY_NAME_SUFFIX)
The suffix for the name of the directory that backups the base directory.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPERATION_REPORT_FILE_NAME](#OPERATION_REPORT_FILE_NAME)
The name (including file extension) of the report file to be created when the merge operation completes.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OPERATION_REPORT_SUBDIRECTORY_NAME](#OPERATION_REPORT_SUBDIRECTORY_NAME)
The name of the sub-directory to be created in the output directory for storing the merge operation report.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [mergeDirectoriesWithChangeTrackingHighlights](#mergeDirectoriesWithChangeTrackingHighlights(java.net.URL,java.net.URL,java.net.URL,ro.sync.diff.api.DiffOptions,boolean,boolean,boolean,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseDirectoryURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) directoryToMergeWithURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) outputDirectoryURL, [DiffOptions](DiffOptions.md) diffOptions, boolean addFilesOnlyPresentInDirectoryToMergeWith, boolean createChangeTrackingMarkersForAddedXMLFiles, boolean deleteFilesOnlyPresentInBaseDirectory, boolean updateNonXMLFilesFromBaseDirectoryToFileVersionsFromDirectoryToMergeWith)
Merges the directories specified by the first 2 URLs and saves the results to the output directory specified by the 3rd URL.

## Field Details

### OPERATION_REPORT_SUBDIRECTORY_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPERATION_REPORT_SUBDIRECTORY_NAME

The name of the sub-directory to be created in the output directory for storing the merge operation report.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.AuthorDiffDirectoriesChangeTrackingMerger.OPERATION_REPORT_SUBDIRECTORY_NAME)

### OPERATION_REPORT_FILE_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OPERATION_REPORT_FILE_NAME

The name (including file extension) of the report file to be created when the merge operation completes.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.AuthorDiffDirectoriesChangeTrackingMerger.OPERATION_REPORT_FILE_NAME)

### BACKUP_DIRECTORY_NAME_SUFFIX

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) BACKUP_DIRECTORY_NAME_SUFFIX

The suffix for the name of the directory that backups the base directory. The base directory is backed up either if the output directory is not specified or the base directory itself is also explicitly chosen/specified as the output directory. When the backup directory is no longer needed, it can be deleted using the URL of the base directory and this suffix to correctly identify it.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.AuthorDiffDirectoriesChangeTrackingMerger.BACKUP_DIRECTORY_NAME_SUFFIX)

## Method Details

### mergeDirectoriesWithChangeTrackingHighlights

void mergeDirectoriesWithChangeTrackingHighlights([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseDirectoryURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) directoryToMergeWithURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) outputDirectoryURL, [DiffOptions](DiffOptions.md) diffOptions, boolean addFilesOnlyPresentInDirectoryToMergeWith, boolean createChangeTrackingMarkersForAddedXMLFiles, boolean deleteFilesOnlyPresentInBaseDirectory, boolean updateNonXMLFilesFromBaseDirectoryToFileVersionsFromDirectoryToMergeWith)throws [DiffException](DiffException.md)

Merges the directories specified by the first 2 URLs and saves the results to the output directory specified by the 3rd URL. Only "file" protocol is supported for all 3 URLs provided. All pairs of modified XML files involved in the process are merged by saving the Author mode comparison results as documents with tracked changes that can be later reviewed and accepted / rejected. All the other situations detected are treated based on 2 options applicable to both XML and non-XML files, plus one option applicable to XML files only, plus another option applicable to non-XML files only. Once the merge operation succeeds, a report file is created. It is named [OPERATION_REPORT_FILE_NAME](#OPERATION_REPORT_FILE_NAME) and is placed in a sub-directory named [OPERATION_REPORT_SUBDIRECTORY_NAME](#OPERATION_REPORT_SUBDIRECTORY_NAME) in the output directory. Aside from the fact that the report provides an overview of the merge process, it also provides links to all the files in the resulting output directory. You can use the respective links to load these XML files in Author mode in Oxygen to review the tracked changes and accept or reject them.
  Parameters: baseDirectoryURL - The URL of the base directory. directoryToMergeWithURL - The URL of the directory to merge with. outputDirectoryURL - The URL of the output directory. Can be null, in which case the base directory is also considered the output directory. Another particular case is when the base directory is explicitly specified as output directory too. In both cases, the base directory is automatically backed up. The backup copy will have the same parent directory as the base directory and its name will be the name of the base directory suffixed by [BACKUP_DIRECTORY_NAME_SUFFIX](#BACKUP_DIRECTORY_NAME_SUFFIX). diffOptions - The [DiffOptions](DiffOptions.md) used to decide which comparing algorithm and which comparing options to use. Can be null in which case the comparison algorithm is chosen automatically and the default comparison options are used. addFilesOnlyPresentInDirectoryToMergeWith - If true, all the files only present in the directory to merge with will be added to the output directory. createChangeTrackingMarkersForAddedXMLFiles - If true, all XML files only present in the directory to merge with - that have to be added to the destination/output directory - will contain change tracking markers of type "added content". The option is not necessarily intended for the merge process itself, but it is useful if you want to apply various Oxygen transformation scenarios to the resulting output directory. deleteFilesOnlyPresentInBaseDirectory - If true, all the files only present in the base directory will not be added to the output directory. updateNonXMLFilesFromBaseDirectoryToFileVersionsFromDirectoryToMergeWith - If true, all non XML files from the base directory are updated to the versions from the directory to merge with. Throws: [DiffException](DiffException.md) - If something went wrong while comparing the directories and saving the results.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
