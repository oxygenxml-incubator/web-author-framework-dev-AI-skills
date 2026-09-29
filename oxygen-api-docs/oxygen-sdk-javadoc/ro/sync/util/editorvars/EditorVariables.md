Package [ro.sync.util.editorvars](package-summary.md)

# Class EditorVariables

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.util.editorvars.EditorVariablesBase](EditorVariablesBase.md)
        * ro.sync.util.editorvars.EditorVariables
   All Implemented Interfaces: [EditorVariablesConstants](EditorVariablesConstants.md)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class EditorVariables extends [EditorVariablesBase](EditorVariablesBase.md)
Holds constants representing all editor variables defined in Oxygen.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md)
Used to determine how framework variables should be expanded/rewritten.
  static interface  [EditorVariables.FunctionResolver](EditorVariables.FunctionResolver.md)
Resolves a function

## Field Summary

### Fields inherited from interface ro.sync.util.editorvars.[EditorVariablesConstants](EditorVariablesConstants.md)
 [ACTIVE_PROFILING_CONDITION_SET](EditorVariablesConstants.md#ACTIVE_PROFILING_CONDITION_SET), [ANCESTOR_FILE_TO_DIFF](EditorVariablesConstants.md#ANCESTOR_FILE_TO_DIFF), [ANSWER_PARAM_START](EditorVariablesConstants.md#ANSWER_PARAM_START), [ARCHIVE_FILE_DIRECTORY](EditorVariablesConstants.md#ARCHIVE_FILE_DIRECTORY), [ARCHIVE_FILE_DIRECTORY_URL](EditorVariablesConstants.md#ARCHIVE_FILE_DIRECTORY_URL), [ARCHIVE_NAME](EditorVariablesConstants.md#ARCHIVE_NAME), [ARCHIVE_NAME_WITH_EXTENSION](EditorVariablesConstants.md#ARCHIVE_NAME_WITH_EXTENSION), [ARCHIVE_PATH](EditorVariablesConstants.md#ARCHIVE_PATH), [ARCHIVE_PATH_URL](EditorVariablesConstants.md#ARCHIVE_PATH_URL), [ASK_PARAM_START](EditorVariablesConstants.md#ASK_PARAM_START), [ASK_PARAM_VALUE_TEMPLATE](EditorVariablesConstants.md#ASK_PARAM_VALUE_TEMPLATE), [AUTHOR_NAME](EditorVariablesConstants.md#AUTHOR_NAME), [BASE_FRAMEWORK_DIRECTORY](EditorVariablesConstants.md#BASE_FRAMEWORK_DIRECTORY), [BASE_FRAMEWORK_URL](EditorVariablesConstants.md#BASE_FRAMEWORK_URL), [CONFIGURED_DITA_OT_DIR](EditorVariablesConstants.md#CONFIGURED_DITA_OT_DIR), [CONFIGURED_DITA_OT_DIR_URL](EditorVariablesConstants.md#CONFIGURED_DITA_OT_DIR_URL), [CT_CARET_EDITOR_VARIABLE](EditorVariablesConstants.md#CT_CARET_EDITOR_VARIABLE), [CT_SELECTION_EDITOR_VARIABLE](EditorVariablesConstants.md#CT_SELECTION_EDITOR_VARIABLE), [CURRENT_FILE](EditorVariablesConstants.md#CURRENT_FILE), [CURRENT_FILE_DIRECTORY](EditorVariablesConstants.md#CURRENT_FILE_DIRECTORY), [CURRENT_FILE_DIRECTORY_URL](EditorVariablesConstants.md#CURRENT_FILE_DIRECTORY_URL), [CURRENT_FILE_URL](EditorVariablesConstants.md#CURRENT_FILE_URL), [CURRENT_FILE_URL_OLD](EditorVariablesConstants.md#CURRENT_FILE_URL_OLD), [CURRENT_FILENAME](EditorVariablesConstants.md#CURRENT_FILENAME), [CURRENT_FILENAME_WITH_EXTENSION](EditorVariablesConstants.md#CURRENT_FILENAME_WITH_EXTENSION), [DATE_FUNCTION_SAMPLE](EditorVariablesConstants.md#DATE_FUNCTION_SAMPLE), [DATE_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#DATE_FUNCTION_VARIABLE_PREFIX), [DEBUGGER_XML_SOURCE](EditorVariablesConstants.md#DEBUGGER_XML_SOURCE), [DEBUGGER_XSL_SOURCE](EditorVariablesConstants.md#DEBUGGER_XSL_SOURCE), [DETECTED_SCHEMA](EditorVariablesConstants.md#DETECTED_SCHEMA), [DETECTED_SCHEMA_URL](EditorVariablesConstants.md#DETECTED_SCHEMA_URL), [EDITOR_VARIABLES_PREFIX](EditorVariablesConstants.md#EDITOR_VARIABLES_PREFIX), [EDITOR_VARIABLES_SUFIX](EditorVariablesConstants.md#EDITOR_VARIABLES_SUFIX), [ENV_FUNCTION_SAMPLE](EditorVariablesConstants.md#ENV_FUNCTION_SAMPLE), [ENV_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#ENV_FUNCTION_VARIABLE_PREFIX), [ENV_VAR_NAME](EditorVariablesConstants.md#ENV_VAR_NAME), [FIRST_FILE_TO_DIFF](EditorVariablesConstants.md#FIRST_FILE_TO_DIFF), [FO_INPUT_FILE](EditorVariablesConstants.md#FO_INPUT_FILE), [FOP_AH_TRANSFORMATION_METHOD](EditorVariablesConstants.md#FOP_AH_TRANSFORMATION_METHOD), [FOP_TRANSFORMATION_METHOD](EditorVariablesConstants.md#FOP_TRANSFORMATION_METHOD), [FRAMEWORK_DIR_FUNCTION_TEMPLATE](EditorVariablesConstants.md#FRAMEWORK_DIR_FUNCTION_TEMPLATE), [FRAMEWORK_DIR_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#FRAMEWORK_DIR_FUNCTION_VARIABLE_PREFIX), [FRAMEWORK_DIRECTORY](EditorVariablesConstants.md#FRAMEWORK_DIRECTORY), [FRAMEWORK_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#FRAMEWORK_FUNCTION_VARIABLE_PREFIX), [FRAMEWORK_URL](EditorVariablesConstants.md#FRAMEWORK_URL), [FRAMEWORK_URL_FUNCTION_TEMPLATE](EditorVariablesConstants.md#FRAMEWORK_URL_FUNCTION_TEMPLATE), [FRAMEWORKS_DIRECTORY](EditorVariablesConstants.md#FRAMEWORKS_DIRECTORY), [FRAMEWORKS_DIRECTORY_URL](EditorVariablesConstants.md#FRAMEWORKS_DIRECTORY_URL), [FUNCTION_VARIABLE_SUFFIX](EditorVariablesConstants.md#FUNCTION_VARIABLE_SUFFIX), [ID](EditorVariablesConstants.md#ID), [MAKE_RELATIVE_FUNCTION_SAMPLE](EditorVariablesConstants.md#MAKE_RELATIVE_FUNCTION_SAMPLE), [MAKE_RELATIVE_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#MAKE_RELATIVE_FUNCTION_VARIABLE_PREFIX), [OUTPUT_FILE](EditorVariablesConstants.md#OUTPUT_FILE), [OUTPUT_FILE_URL](EditorVariablesConstants.md#OUTPUT_FILE_URL), [OXYGEN_HOME_URL](EditorVariablesConstants.md#OXYGEN_HOME_URL), [OXYGEN_INSTALL_DIR](EditorVariablesConstants.md#OXYGEN_INSTALL_DIR), [PATH_SEPARATOR](EditorVariablesConstants.md#PATH_SEPARATOR), [PLUGIN_DIR_FUNCTION_TEMPLATE](EditorVariablesConstants.md#PLUGIN_DIR_FUNCTION_TEMPLATE), [PLUGIN_DIR_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#PLUGIN_DIR_FUNCTION_VARIABLE_PREFIX), [PLUGIN_DIR_URL_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#PLUGIN_DIR_URL_FUNCTION_VARIABLE_PREFIX), [PLUGIN_URL_FUNCTION_TEMPLATE](EditorVariablesConstants.md#PLUGIN_URL_FUNCTION_TEMPLATE), [PROJECT_DIRECTORY](EditorVariablesConstants.md#PROJECT_DIRECTORY), [PROJECT_DIRECTORY_URL](EditorVariablesConstants.md#PROJECT_DIRECTORY_URL), [PROJECT_NAME](EditorVariablesConstants.md#PROJECT_NAME), [ROOT_MAP_DIR](EditorVariablesConstants.md#ROOT_MAP_DIR), [ROOT_MAP_DIR_URL](EditorVariablesConstants.md#ROOT_MAP_DIR_URL), [ROOT_MAP_FILE](EditorVariablesConstants.md#ROOT_MAP_FILE), [ROOT_MAP_URL](EditorVariablesConstants.md#ROOT_MAP_URL), [SAXON_CONFIG_FILE](EditorVariablesConstants.md#SAXON_CONFIG_FILE), [SECOND_FILE_TO_DIFF](EditorVariablesConstants.md#SECOND_FILE_TO_DIFF), [SQL](EditorVariablesConstants.md#SQL), [SQL_URL](EditorVariablesConstants.md#SQL_URL), [STATIC_XPATH_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#STATIC_XPATH_FUNCTION_VARIABLE_PREFIX), [SYSTEM_FUNCTION_SAMPLE](EditorVariablesConstants.md#SYSTEM_FUNCTION_SAMPLE), [SYSTEM_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#SYSTEM_FUNCTION_VARIABLE_PREFIX), [SYSTEM_VAR_NAME](EditorVariablesConstants.md#SYSTEM_VAR_NAME), [TIMESTAMP](EditorVariablesConstants.md#TIMESTAMP), [TRANSFORMATION_SAVED_FILE](EditorVariablesConstants.md#TRANSFORMATION_SAVED_FILE), [TRANSLATE_FUNCTION_VARIABLE_PREFIX](EditorVariablesConstants.md#TRANSLATE_FUNCTION_VARIABLE_PREFIX), [UNIQUE_CARET_MARKER_FOR_AUTHOR](EditorVariablesConstants.md#UNIQUE_CARET_MARKER_FOR_AUTHOR), [UNIQUE_CARET_MARKER_PI_NAME_FOR_AUTHOR](EditorVariablesConstants.md#UNIQUE_CARET_MARKER_PI_NAME_FOR_AUTHOR), [USER_HOME_DIR](EditorVariablesConstants.md#USER_HOME_DIR), [USER_HOME_URL](EditorVariablesConstants.md#USER_HOME_URL), [UUID](EditorVariablesConstants.md#UUID), [XML](EditorVariablesConstants.md#XML), [XML_CATALOG_FILES_LIST](EditorVariablesConstants.md#XML_CATALOG_FILES_LIST), [XML_URL](EditorVariablesConstants.md#XML_URL), [XPATH_FUNCTION_SAMPLE](EditorVariablesConstants.md#XPATH_FUNCTION_SAMPLE), [XPROC](EditorVariablesConstants.md#XPROC), [XPROC_URL](EditorVariablesConstants.md#XPROC_URL), [XQUERY](EditorVariablesConstants.md#XQUERY), [XQUERY_URL](EditorVariablesConstants.md#XQUERY_URL), [XSL](EditorVariablesConstants.md#XSL), [XSL_URL](EditorVariablesConstants.md#XSL_URL)
## Constructor Summary
 Constructors
Constructor

Description
 [EditorVariables](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static void [addCustomEditorVariablesResolver](#addCustomEditorVariablesResolver(ro.sync.exml.workspace.api.util.EditorVariablesResolver))([EditorVariablesResolver](../../exml/workspace/api/util/EditorVariablesResolver.md) resolver)
Add custom resolver.
  static boolean [containsEditorVariable](#containsEditorVariable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)
Checks if the given expression contains editor variables.
  static boolean [containsInteractiveVariable](#containsInteractiveVariable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)
Checks if the given expression contains at least an interactive editor variable ($ask, $answer).
  static boolean [containsXPathEvalEditorVariable](#containsXPathEvalEditorVariable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)
Checks if the given expression contains the xpath_eval editor variables.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandEditorVariables](#expandEditorVariables(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL)
Expand the editor variables in the output file name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandEditorVariables](#expandEditorVariables(java.lang.String,java.lang.String,java.util.Map,ro.sync.util.editorvars.expander.ErrorListener))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.util.editorvars.expander.EditorVariableResolver> additionalResolvers, ro.sync.util.editorvars.expander.ErrorListener errorListener)
Expand the editor variables in the output file name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandEditorVariablesAsFilePath](#expandEditorVariablesAsFilePath(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL)
Expand the editor variables.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [expandEditorVariablesAsURL](#expandEditorVariablesAsURL(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)
Expand the editor variables.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandFrameworksVariables](#expandFrameworksVariables(java.lang.String,java.lang.String,java.lang.String,ro.sync.util.editorvars.EditorVariables.FrameworkRewritePolicy))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkStoreLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseStoreLocation, [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) rewritePolicy)
Expand FRAMEWORKS_DIRECTORY_URL, FRAMEWORKS_DIRECTORY, FRAMEWORK_DIRECTORY and FRAMEWORK_URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandFrameworksVariables](#expandFrameworksVariables(java.lang.String,java.lang.String,ro.sync.util.editorvars.EditorVariables.FrameworkRewritePolicy))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkStoreLocation, [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) rewritePolicy)
Expand FRAMEWORKS_DIRECTORY_URL, FRAMEWORKS_DIRECTORY, FRAMEWORK_DIRECTORY and FRAMEWORK_URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandFrameworksVariables](#expandFrameworksVariables(java.lang.String,ro.sync.util.editorvars.EditorVariables.FrameworkRewritePolicy,java.io.File,java.net.URL,java.io.File,java.net.URL))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) rewritePolicy, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksDir, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) frameworksURL, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkDir, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) frameworkURL)
Expand FRAMEWORKS_DIRECTORY_URL, FRAMEWORKS_DIRECTORY, FRAMEWORK_DIRECTORY and FRAMEWORK_URL.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [generateUniqueID](#generateUniqueID())()

 static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] [getAdditionalFrameworksDirs](#getAdditionalFrameworksDirs())()
Get all the additional frameworks directories specified by user.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[EditorVariableDescription](../../exml/workspace/api/util/EditorVariableDescription.md)> [getAllCustomResolvedEditorVariables](#getAllCustomResolvedEditorVariables())()
Get a list with all custom resolved editor variables.
  static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] [getAllFrameworksDirs](#getAllFrameworksDirs())()
Get all the frameworks directories including default framework directory, user preferences directory and additional frameworks directories.
  static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getBaseUserFrameworksDir](#getBaseUserFrameworksDir())()
Get the base frameworks directory from the user preferences directory like: Users\\*\*\*\AppData\Roaming\com.oxygenxml\extensions\v14.0\frameworks Note: This is not the actual directory with frameworks but the directory which contains all frameworks directories.
  static ro.sync.util.editorvars.CatalogManagerUtilsAccess [getCatalogUtilsAccess](#getCatalogUtilsAccess())()
Get the catalog utils access.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCurrentArchiveURL](#getCurrentArchiveURL(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentFileSystemID)
Returns the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) of the current archive.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCurrentFrameworksURL](#getCurrentFrameworksURL())()
Get the current frameworks directory.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCurrentFrameworksURL](#getCurrentFrameworksURL(ro.sync.options.NotifyableMap))(ro.sync.options.NotifyableMap optionsMap)
Get the current frameworks directory.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCurrentProjectURL](#getCurrentProjectURL(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentFileSystemID)
Returns the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) of the current project.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getDefaultFrameworkURL](#getDefaultFrameworkURL())()
Get the default frameworks directory.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editorVariable)
Returns a description of the editor variable.
  static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getFrameworksDir](#getFrameworksDir())()
Get the [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) representing the "frameworks" directory.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getFrameworksUrl](#getFrameworksUrl())()
Get the "frameworks" directory [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSystemPathSeparator](#getSystemPathSeparator())()

 static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] [getUserFrameworksDirs](#getUserFrameworksDirs())()
Get the frameworks directories from the user preferences directory like: Users\\*\*\*\AppData\Roaming\com.oxygenxml\extensions\v14.0\frameworks\{update_site}.
  static ro.sync.util.editorvars.XPathEvaluator [getXpathEvaluator](#getXpathEvaluator())()
Gets the XPath evaluator.
  static boolean [isRelativizedToProject](#isRelativizedToProject(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Checks if URL is relative to project
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeFileRelative2DITAOTDir](#makeFileRelative2DITAOTDir(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileOrDir)
Make a file or directory relative to the configured DITA OT directory.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeFileRelative2Framework](#makeFileRelative2Framework(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkFilePath)
Make a file or directory relative to the $framework or $frameworks directory.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeFileRelative2Frameworks](#makeFileRelative2Frameworks(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileOrDir)
Make a file or directory relative to the "frameworks" directory.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeFileRelative2Project](#makeFileRelative2Project(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) projectFilePath)
Make a file or directory relative to the $pdudirectory.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeURLRelative2Framework](#makeURLRelative2Framework(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkFileURL)
Make an URL relative to $framework or that if not possible, to $frameworks (also if possible).
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeURLRelative2Frameworks](#makeURLRelative2Frameworks(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Make an URL relative to the "frameworks" directory.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeURLRelative2Project](#makeURLRelative2Project(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) projectFileURL)
Make an URL relative to $pdu if possible.
  static boolean [possiblyContainsEditorVariable](#possiblyContainsEditorVariable(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)
Checks if the given expression potentially contains editor variables.
  static void [removeCustomEditorVariablesResolver](#removeCustomEditorVariablesResolver(ro.sync.exml.workspace.api.util.EditorVariablesResolver))([EditorVariablesResolver](../../exml/workspace/api/util/EditorVariablesResolver.md) resolver)
Remove a custom resolver.
  static void [resetDefaultFrameworkURL](#resetDefaultFrameworkURL())()
Reset the cached value of the default frameworks directory property.
  static void [resetFrameworksDir](#resetFrameworksDir())()
Reset the computed value for the framework location.
  static void [setAdditionalFrameworksProvider](#setAdditionalFrameworksProvider(ro.sync.exml.options.AdditionalFrameworksProvider))(ro.sync.exml.options.AdditionalFrameworksProvider additionalFrameworksProvider)
Sets the referenced directory as additional framework directory.
  static void [setArchiveExtensionsRecognizer](#setArchiveExtensionsRecognizer(ro.sync.util.ArchiveExtensionsRecognizer))(ro.sync.util.ArchiveExtensionsRecognizer archiveExtensionsRecognizer)
Set an archive extensions recognizer
  static void [setArchiveURLProvider](#setArchiveURLProvider(ro.sync.util.ArchiveURLProvider))(ro.sync.util.ArchiveURLProvider archiveURLProvider)
Set the archive URL provider.
  static void [setCatalogUtilsAccess](#setCatalogUtilsAccess(ro.sync.util.editorvars.CatalogManagerUtilsAccess))(ro.sync.util.editorvars.CatalogManagerUtilsAccess catalogUtilsAccess)
Set the catalogs utils access.
  static void [setConditionSetNameResolver](#setConditionSetNameResolver(ro.sync.util.editorvars.ConditionSetNameResolver))(ro.sync.util.editorvars.ConditionSetNameResolver conditionSetNameResolver)
Set the provider for the profiling condition set name.
  static void [setFrameworkLocationResolver](#setFrameworkLocationResolver(ro.sync.util.editorvars.FrameworkLocationResolver))(ro.sync.util.editorvars.FrameworkLocationResolver frameworkLocationResolver)
Can locate a framework by using its name.
  static void [setFrameworksDirForTest](#setFrameworksDirForTest(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) fDir)
Set a frameworks dir so it will not be computed from the home url.
  static void [setFrameworksURLForTest](#setFrameworksURLForTest(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) fURL)
Set a frameworks url so it will not be computed from the home url.
  static void [setPluginLocationResolver](#setPluginLocationResolver(ro.sync.util.editorvars.PluginLocationResolver))(ro.sync.util.editorvars.PluginLocationResolver resolver)
Set the plugin location resolver.
  static void [setProjectURLProvider](#setProjectURLProvider(ro.sync.util.ProjectURLProvider))(ro.sync.util.ProjectURLProvider projectURLProvider)
Set the project URL provider.
  static void [setRootMapResolver](#setRootMapResolver(ro.sync.util.editorvars.DITARootMapProvider))(ro.sync.util.editorvars.DITARootMapProvider ditaRootMapProvider)
Obtain the provider that contains information about DITA root map.
  static void [setUserUploadedFrameworks](#setUserUploadedFrameworks(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) userFrameworksDir)
Sets directory where the user uploaded frameworks are stored.
  static void [setXpathEvaluator](#setXpathEvaluator(ro.sync.util.editorvars.XPathEvaluator))(ro.sync.util.editorvars.XPathEvaluator staticXpathEvaluator)
Set an XPath evaluator.

### Methods inherited from class ro.sync.util.editorvars.[EditorVariablesBase](EditorVariablesBase.md)
 [expandEnvAndSystem](EditorVariablesBase.md#expandEnvAndSystem(java.lang.String)), [fastEquals](EditorVariablesBase.md#fastEquals(java.lang.String,java.lang.String)), [getName](EditorVariablesBase.md#getName(java.lang.String)), [registerEnvAndSystemResolver](EditorVariablesBase.md#registerEnvAndSystemResolver(ro.sync.util.editorvars.expander.EditorVariableExpander)), [replaceFunctions](EditorVariablesBase.md#replaceFunctions(java.lang.String,java.lang.String,java.lang.String,ro.sync.util.editorvars.EditorVariables.FunctionResolver))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditorVariables

public EditorVariables()

## Method Details

### getDescription

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editorVariable)

Returns a description of the editor variable.
  Parameters: editorVariable - The editor variable to get description for. Returns: The description for the editor variable.
### possiblyContainsEditorVariable

public static boolean possiblyContainsEditorVariable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)

Checks if the given expression potentially contains editor variables. The method is very fast but it does not guarantee the expression actually contains editor variables which are understood by the application.
  Parameters: expression - The expression to check. Returns: true if the expression potentially contains editor variables.
### containsXPathEvalEditorVariable

public static boolean containsXPathEvalEditorVariable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)

Checks if the given expression contains the xpath_eval editor variables.
  Parameters: expression - The expression to check. Returns: true if the expression contains the xpath_eval editor variable.
### containsInteractiveVariable

public static boolean containsInteractiveVariable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)

Checks if the given expression contains at least an interactive editor variable ($ask, $answer).
  Parameters: expression - The expression to check. Returns: true if the expression contains at least an interactive editor variable.
### containsEditorVariable

public static boolean containsEditorVariable([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expression)

Checks if the given expression contains editor variables.
  Parameters: expression - The expression to check. Returns: true if the expression contains one of the available editor variables.
### expandEditorVariablesAsFilePath

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandEditorVariablesAsFilePath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL)

Expand the editor variables. The returned value will attempt to be a file path. So even if the editor variables expand to an URL, the file path will be returned. The currently known editor variables are declared in this class.
  Parameters: expr - The expresion containing editor variables. currentEditedFileURL - The full path of the current edited file, as an URI. Returns: The expresion with the editor variables expanded, possibly an URI.
### expandEditorVariablesAsURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) expandEditorVariablesAsURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)

Expand the editor variables. The returned value will be an URL, or null if it cannot be built.
  Parameters: path - the path to be resolved, may be relative to the baseSystemID baseSystemID - the system ID of the base file. Returns: the resolved path as URL, or null
### expandEditorVariables

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandEditorVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL)

Expand the editor variables in the output file name. The currently known editor variables are declared in this class.
  Parameters: expr - The expresion containing editor variables. currentEditedFileURL - The full path of the current edited file, as an URI. Returns: The expresion with the editor variables expanded, possibly an URI.
### expandEditorVariables

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandEditorVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),ro.sync.util.editorvars.expander.EditorVariableResolver> additionalResolvers, ro.sync.util.editorvars.expander.ErrorListener errorListener)throws ro.sync.util.editorvars.parser.ParseException, ro.sync.util.editorvars.expander.OperationCancelledException

Expand the editor variables in the output file name. The currently known editor variables are declared in this class.
  Parameters: expr - The expression containing editor variables. currentEditedFileURL - The full path of the current edited file, as an URI. additionalResolvers - Some additional variables resolvers. errorListener - Error listener. Returns: The expression with the editor variables expanded, possibly an URI. Throws: ro.sync.util.editorvars.expander.OperationCancelledException ro.sync.util.editorvars.parser.ParseException
### makeURLRelative2Frameworks

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeURLRelative2Frameworks([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Make an URL relative to the "frameworks" directory.
  Parameters: url - The original URL. Returns: The relative URL to the "frameworks" if possible, otherwise the original URL.
### makeFileRelative2DITAOTDir

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeFileRelative2DITAOTDir([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileOrDir)

Make a file or directory relative to the configured DITA OT directory.
  Parameters: fileOrDir - The original file or directory. Returns: The relative path to the configured DITA OT directory or null if could not make it relative.
### makeFileRelative2Frameworks

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeFileRelative2Frameworks([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileOrDir)

Make a file or directory relative to the "frameworks" directory.
  Parameters: fileOrDir - The original file or directory. Returns: The relative path to the "frameworks" if possible, otherwise the original file or directory path.
### setFrameworksURLForTest

public static void setFrameworksURLForTest([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) fURL)

Set a frameworks url so it will not be computed from the home url.
  Parameters: fURL - The url.
### getFrameworksUrl

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getFrameworksUrl() throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Get the "frameworks" directory [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  Returns: The "frameworks" directory [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html). Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the oxygen home URL is not set.
### resetFrameworksDir

public static void resetFrameworksDir()

Reset the computed value for the framework location. The next time it will be requested it will be recomputed.

### getCurrentFrameworksURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCurrentFrameworksURL() throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Get the current frameworks directory.
  Returns: The current frameworks URL. Can be a custom one if it was set in options, or the default one. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the oxygen home URL is not set.
### getCurrentFrameworksURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCurrentFrameworksURL(ro.sync.options.NotifyableMap optionsMap)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Get the current frameworks directory.
  Parameters: optionsMap - The Oxygen options. Returns: The current frameworks URL. Can be a custom one if it was set in options, or the default one. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the oxygen home URL is not set.
### getDefaultFrameworkURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getDefaultFrameworkURL() throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Get the default frameworks directory. It is relative to the oxygen installation directory.
  Returns: The default frameworks directory. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the oxygen home URL is not set.
### resetDefaultFrameworkURL

public static void resetDefaultFrameworkURL()

Reset the cached value of the default frameworks directory property.

### setFrameworksDirForTest

public static void setFrameworksDirForTest([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) fDir)

Set a frameworks dir so it will not be computed from the home url. Only from tests.
  Parameters: fDir -
### getFrameworksDir

public static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getFrameworksDir() throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Get the [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) representing the "frameworks" directory.
  Returns: The "frameworks" directory [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html). Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the oxygen home URL is not set.
### getBaseUserFrameworksDir

public static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getBaseUserFrameworksDir()

Get the base frameworks directory from the user preferences directory like: Users\\*\*\*\AppData\Roaming\com.oxygenxml\extensions\v14.0\frameworks Note: This is not the actual directory with frameworks but the directory which contains all frameworks directories. A directory for each update site: - extensions\v14.0\frameworks\{update_site_1} - extensions\v14.0\frameworks\{update_site_2}
  Returns: The user frameworks directory.
### getUserFrameworksDirs

public static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] getUserFrameworksDirs()

Get the frameworks directories from the user preferences directory like: Users\\*\*\*\AppData\Roaming\com.oxygenxml\extensions\v14.0\frameworks\{update_site}. A new level is inserted ({update_site}) to protect against add-ons conflicts (sort of like a namespace).
  Returns: The user frameworks directories or null if it doesn't exists.
### getAllFrameworksDirs

public static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] getAllFrameworksDirs()

Get all the frameworks directories including default framework directory, user preferences directory and additional frameworks directories.
  Returns: All the frameworks directories.
### getAdditionalFrameworksDirs

public static [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] getAdditionalFrameworksDirs()

Get all the additional frameworks directories specified by user.
  Returns: The additional frameworks directories.
### getCurrentProjectURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCurrentProjectURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentFileSystemID)

Returns the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) of the current project.
  Parameters: currentFileSystemID - The current file system ID. Returns: The current project [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) or null if it cannot be determined.
### getCurrentArchiveURL

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCurrentArchiveURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentFileSystemID)

Returns the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) of the current archive.
  Parameters: currentFileSystemID - The current file system ID. Returns: The current archive [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) or null if it cannot be determined.
### setProjectURLProvider

public static void setProjectURLProvider(ro.sync.util.ProjectURLProvider projectURLProvider)

Set the project URL provider.
  Parameters: projectURLProvider - The new project URL provider.
### setArchiveURLProvider

public static void setArchiveURLProvider(ro.sync.util.ArchiveURLProvider archiveURLProvider)

Set the archive URL provider.
  Parameters: archiveURLProvider - The new archive URL provider.
### setFrameworkLocationResolver

public static void setFrameworkLocationResolver(ro.sync.util.editorvars.FrameworkLocationResolver frameworkLocationResolver)

Can locate a framework by using its name.
  Parameters: frameworkLocationResolver - Can locate a framework by using its name.
### setPluginLocationResolver

public static void setPluginLocationResolver(ro.sync.util.editorvars.PluginLocationResolver resolver)

Set the plugin location resolver.
  Parameters: resolver - The plugin location resolver.
### setRootMapResolver

public static void setRootMapResolver(ro.sync.util.editorvars.DITARootMapProvider ditaRootMapProvider)

Obtain the provider that contains information about DITA root map.
  Parameters: ditaRootMapProvider - The provider for the DITA root map.
### setConditionSetNameResolver

public static void setConditionSetNameResolver(ro.sync.util.editorvars.ConditionSetNameResolver conditionSetNameResolver)

Set the provider for the profiling condition set name.
  Parameters: conditionSetNameResolver - Object which provides the profiling condition set name.
### setArchiveExtensionsRecognizer

public static void setArchiveExtensionsRecognizer(ro.sync.util.ArchiveExtensionsRecognizer archiveExtensionsRecognizer)

Set an archive extensions recognizer
  Parameters: archiveExtensionsRecognizer - The archiveExtensionsRecognizer.
### getSystemPathSeparator

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSystemPathSeparator()
  Returns: The system path separator. It is dependent on the platform.
### expandFrameworksVariables

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandFrameworksVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkStoreLocation, [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) rewritePolicy)

Expand FRAMEWORKS_DIRECTORY_URL, FRAMEWORKS_DIRECTORY, FRAMEWORK_DIRECTORY and FRAMEWORK_URL. All these variables are resolved relative to framework store location.
  Parameters: expr - Editor variables expression. frameworkStoreLocation - The framework store location as an file path. rewritePolicy - Rewrite FRAMEWORK_DIRECTORY and FRAMEWORK_URL using FRAMEWORKS_DIRECTORY_URL and FRAMEWORKS_DIRECTORY variables. Returns: The given expression with the framework variables expanded.
### expandFrameworksVariables

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandFrameworksVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkStoreLocation, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseStoreLocation, [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) rewritePolicy)

Expand FRAMEWORKS_DIRECTORY_URL, FRAMEWORKS_DIRECTORY, FRAMEWORK_DIRECTORY and FRAMEWORK_URL. All these variables are resolved relative to framework store location.
  Parameters: expr - Editor variables expression. frameworkStoreLocation - The framework store location as an file path. baseStoreLocation - The base store location rewritePolicy - Rewrite FRAMEWORK_DIRECTORY and FRAMEWORK_URL using FRAMEWORKS_DIRECTORY_URL and FRAMEWORKS_DIRECTORY variables. Returns: The given expression with the framework variables expanded.
### expandFrameworksVariables

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandFrameworksVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expr, [EditorVariables.FrameworkRewritePolicy](EditorVariables.FrameworkRewritePolicy.md) rewritePolicy, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworksDir, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) frameworksURL, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkDir, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) frameworkURL)

Expand FRAMEWORKS_DIRECTORY_URL, FRAMEWORKS_DIRECTORY, FRAMEWORK_DIRECTORY and FRAMEWORK_URL.
  Parameters: expr - Editor variables expression. rewritePolicy - Rewrite FRAMEWORK_DIRECTORY and FRAMEWORK_URL using FRAMEWORKS_DIRECTORY_URL and FRAMEWORKS_DIRECTORY variables. frameworksDir - The directory where all frameworks reside. frameworksURL - The URL of the directory where all frameworks reside. frameworkDir - The directory where the specific framework reside. frameworkURL - The URL of the directory where the specific framework reside. Returns: The given expression with the framework variables expanded.
### makeURLRelative2Framework

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeURLRelative2Framework([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkFileURL)

Make an URL relative to $framework or that if not possible, to $frameworks (also if possible). OBS: $frameworks is the frameworks directory of the given framework frameworkFileURL.
  Parameters: url - The URL. frameworkFileURL - The URL of the ".framework" file. Returns: The relative URL to the $framework or $frameworks if possible, otherwise the original URL.
### makeURLRelative2Project

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeURLRelative2Project([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) projectFileURL)

Make an URL relative to $pdu if possible.
  Parameters: url - The URL. projectFileURL - The URL of the ".prj" file. Returns: The relative URL to the $pdu if possible, otherwise the original URL.
### makeFileRelative2Framework

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeFileRelative2Framework([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) frameworkFilePath)

Make a file or directory relative to the $framework or $frameworks directory. The $frameworks directory is the frameworks directory of the given framework file, so it might differ from the default Oxygen frameworks directory.
  Parameters: path - The original file or directory. frameworkFilePath - The URL of the ".framework" file. Returns: The relative path to the $framework or $frameworks if possible, otherwise the original file or directory path.
### makeFileRelative2Project

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeFileRelative2Project([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) projectFilePath)

Make a file or directory relative to the $pdudirectory.
  Parameters: path - The original file or directory. projectFilePath - The URL of the ".pdu" file. Returns: The relative path to the $pdu if possible, otherwise the original file or directory path.
### setXpathEvaluator

public static void setXpathEvaluator(ro.sync.util.editorvars.XPathEvaluator staticXpathEvaluator)

Set an XPath evaluator.
  Parameters: staticXpathEvaluator - The static xpath evaluator interface.
### getXpathEvaluator

public static ro.sync.util.editorvars.XPathEvaluator getXpathEvaluator()

Gets the XPath evaluator.
  Returns: The static xpath evaluator interface. Can be null if not previously set.
### addCustomEditorVariablesResolver

public static void addCustomEditorVariablesResolver([EditorVariablesResolver](../../exml/workspace/api/util/EditorVariablesResolver.md) resolver)

Add custom resolver.
  Parameters: resolver - The custom resolver to add.
### removeCustomEditorVariablesResolver

public static void removeCustomEditorVariablesResolver([EditorVariablesResolver](../../exml/workspace/api/util/EditorVariablesResolver.md) resolver)

Remove a custom resolver.
  Parameters: resolver - The resolver to remove.
### getAllCustomResolvedEditorVariables

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[EditorVariableDescription](../../exml/workspace/api/util/EditorVariableDescription.md)> getAllCustomResolvedEditorVariables()

Get a list with all custom resolved editor variables.
  Returns: a list with all custom resolved editor variables.
### setAdditionalFrameworksProvider

public static void setAdditionalFrameworksProvider(ro.sync.exml.options.AdditionalFrameworksProvider additionalFrameworksProvider)

Sets the referenced directory as additional framework directory.
  Parameters: additionalFrameworksProvider - The additionalFrameworksProvider to set.
### setUserUploadedFrameworks

public static void setUserUploadedFrameworks([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) userFrameworksDir)

Sets directory where the user uploaded frameworks are stored.
  Parameters: userFrameworksDir - The location of frameworks uploaded by the user in WA.
### setCatalogUtilsAccess

public static void setCatalogUtilsAccess(ro.sync.util.editorvars.CatalogManagerUtilsAccess catalogUtilsAccess)

Set the catalogs utils access.
  Parameters: catalogUtilsAccess - The catalog Utils Access.
### getCatalogUtilsAccess

public static ro.sync.util.editorvars.CatalogManagerUtilsAccess getCatalogUtilsAccess()

Get the catalog utils access.
  Returns: Returns the catalog Utils Access.
### generateUniqueID

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) generateUniqueID()
  Returns: The generated Unique ID
### isRelativizedToProject

public static boolean isRelativizedToProject([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Checks if URL is relative to project
  Parameters: url - URL to check Returns: true if URL starts with ${pd}
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
