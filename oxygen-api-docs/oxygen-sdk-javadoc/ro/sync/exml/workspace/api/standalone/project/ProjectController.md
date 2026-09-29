Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Interface ProjectController
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ProjectController
API to access the Project view.
  Since: 19.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addLinksToFoldersInProjectRoot](#addLinksToFoldersInProjectRoot(java.io.File%5B%5D))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] folders)
Add links to existing folders in the project root references list.
  void [addPopUpMenuCustomizer](#addPopUpMenuCustomizer(ro.sync.exml.workspace.api.standalone.project.ProjectPopupMenuCustomizer))([ProjectPopupMenuCustomizer](ProjectPopupMenuCustomizer.md) popUpCustomizer)
Add the given pop-up menu customizer which can be used to customize the Project pop-up menu.
  void [addProjectChangeListener](#addProjectChangeListener(ro.sync.exml.workspace.api.standalone.project.ProjectChangeListener))([ProjectChangeListener](ProjectChangeListener.md) projectChangeListener)
Add a listener that gets notified **after** another project is loaded.
  void [addRendererCustomizer](#addRendererCustomizer(ro.sync.exml.workspace.api.standalone.project.ProjectRendererCustomizer))([ProjectRendererCustomizer](ProjectRendererCustomizer.md) rendererCustomizer)
Add the given renderer customizer which can be used to customize the Project rendering for various displayed resources.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md)> [findInFiles](#findInFiles(ro.sync.exml.workspace.api.standalone.project.SearchParams))([SearchParams](SearchParams.md) findParams)
Find in files.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getCurrentProjectURL](#getCurrentProjectURL())()
Get the URL of the current project.
  [Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> [getMainFileResourcesIterator](#getMainFileResourcesIterator())()
Get an iterator over the entire list of main file resources referenced in the Project "Main Files" folder.
  ro.sync.exml.workspace.api.standalone.project.ProjectIndexer [getProjectIndexer](#getProjectIndexer())()
Gives access to text search operations over resources indexed for the current project.
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] [getSelectedFiles](#getSelectedFiles())()
Gets the selected files or folders.
  void [loadProject](#loadProject(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) project)
Load the given project file.
  [MoveRenameResult](MoveRenameResult.md) [moveRename](#moveRename(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceFilePath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) destinationFilePath)
Move or rename a file or folder to a destination.
  void [refreshFolders](#refreshFolders(java.io.File%5B%5D))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] folders)
Refresh the given folders referenced in the project.
  void [removePopUpMenuCustomizer](#removePopUpMenuCustomizer(ro.sync.exml.workspace.api.standalone.project.ProjectPopupMenuCustomizer))([ProjectPopupMenuCustomizer](ProjectPopupMenuCustomizer.md) popUpCustomizer)
Remove the given pop-up menu customizer.
  void [removeProjectChangeListener](#removeProjectChangeListener(ro.sync.exml.workspace.api.standalone.project.ProjectChangeListener))([ProjectChangeListener](ProjectChangeListener.md) projectChangeListener)
Remove a listener that gets notified when another project is loaded.
  void [removeRendererCustomizer](#removeRendererCustomizer(ro.sync.exml.workspace.api.standalone.project.ProjectRendererCustomizer))([ProjectRendererCustomizer](ProjectRendererCustomizer.md) rendererCustomizer)
Remove the given renderer customizer.

## Method Details

### addProjectChangeListener

void addProjectChangeListener([ProjectChangeListener](ProjectChangeListener.md) projectChangeListener)

Add a listener that gets notified **after** another project is loaded.
  Parameters: projectChangeListener - The project listener to add. Since: 21.1
### removeProjectChangeListener

void removeProjectChangeListener([ProjectChangeListener](ProjectChangeListener.md) projectChangeListener)

Remove a listener that gets notified when another project is loaded.
  Parameters: projectChangeListener - The project listener to remove. Since: 21.1
### getCurrentProjectURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getCurrentProjectURL()

Get the URL of the current project.
  Returns: the project URL. Since: 21.1
### addPopUpMenuCustomizer

void addPopUpMenuCustomizer([ProjectPopupMenuCustomizer](ProjectPopupMenuCustomizer.md) popUpCustomizer)

Add the given pop-up menu customizer which can be used to customize the Project pop-up menu.
  Parameters: popUpCustomizer - the pop-up menu customizer to add.
### removePopUpMenuCustomizer

void removePopUpMenuCustomizer([ProjectPopupMenuCustomizer](ProjectPopupMenuCustomizer.md) popUpCustomizer)

Remove the given pop-up menu customizer.
  Parameters: popUpCustomizer - the pop-up menu customizer to remove.
### getSelectedFiles

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] getSelectedFiles()

Gets the selected files or folders. If both parent and child files/folders are selected, they are all returned.
  Returns: The array of Files value, can be empty if no selection or invalid selection.
### refreshFolders

void refreshFolders([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] folders)

Refresh the given folders referenced in the project.
  Parameters: folders - An array of folders to refresh.
### addLinksToFoldersInProjectRoot

void addLinksToFoldersInProjectRoot([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html)[] folders)

Add links to existing folders in the project root references list.
  Parameters: folders - The folders to refer. They should already be created on disk before calling this API which just links to it.
### addRendererCustomizer

void addRendererCustomizer([ProjectRendererCustomizer](ProjectRendererCustomizer.md) rendererCustomizer)

Add the given renderer customizer which can be used to customize the Project rendering for various displayed resources.
  Parameters: rendererCustomizer - the renderer customizer to add. Since: 20
### removeRendererCustomizer

void removeRendererCustomizer([ProjectRendererCustomizer](ProjectRendererCustomizer.md) rendererCustomizer)

Remove the given renderer customizer.
  Parameters: rendererCustomizer - the renderer customizer to remove. Since: 20
### loadProject

void loadProject([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) project)

Load the given project file.
  Parameters: project - The project file. Since: 22
### getProjectIndexer

ro.sync.exml.workspace.api.standalone.project.ProjectIndexer getProjectIndexer()

Gives access to text search operations over resources indexed for the current project.
  Returns: The indexer, never null. Since: 24.1
### getMainFileResourcesIterator

[Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> getMainFileResourcesIterator()

Get an iterator over the entire list of main file resources referenced in the Project "Main Files" folder. If the "Main files" support is disabled, an empty iterator will be returned, even if it contains referenced resources.
  Returns: An iterator over the list with configured main files. Never null. Since: 25
### findInFiles

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md)> findInFiles([SearchParams](SearchParams.md) findParams)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Find in files.
  Parameters: findParams - The find parameters. Returns: the list of matches. The list can be null if no matches are found. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If there are fatal errors during the search. Since: 28  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

### moveRename

[MoveRenameResult](MoveRenameResult.md) moveRename([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sourceFilePath, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) destinationFilePath)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Move or rename a file or folder to a destination.
  Parameters: sourceFilePath - Source file or folder destinationFilePath - Destination. Returns: a move rename result, never null. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) Since: 28.1  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
