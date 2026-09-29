Package [ro.sync.exml.workspace.api.results](package-summary.md)

# Interface ResultsManager
    @API(type=EXTENDABLE, src=PUBLIC) public interface ResultsManager
Manages the results of various operations. For example, the results can be presented in a new or an already existing view/tab.Available for the stand-alone and Eclipse plugin versions of oXygen. The results manager can be retrieved from an instance of [PluginWorkspace](../PluginWorkspace.md) (see method getResultsManager()).
  Since: 19.0
## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [ResultsManager.ResultType](ResultsManager.ResultType.md)
The type of the result.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addEventHandler](#addEventHandler(java.lang.String,ro.sync.exml.workspace.api.results.ResultsTabEventHandler))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabEventHandler](ResultsTabEventHandler.md) handler)
Add a handler for events from a results tab, such as clicks, double-clicks, pressing Enter on an entry, and others.
  void [addPopUpMenuCustomizer](#addPopUpMenuCustomizer(java.lang.String,ro.sync.exml.workspace.api.results.ResultsTabPopUpMenuCustomizer))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabPopUpMenuCustomizer](ResultsTabPopUpMenuCustomizer.md) customizer)
Add a pop-up menu customizer for a specific results tab.
  void [addResult](#addResult(java.lang.String,ro.sync.document.DocumentPositionedInfo,ro.sync.exml.workspace.api.results.ResultsManager.ResultType,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) result, [ResultsManager.ResultType](ResultsManager.ResultType.md) resultType, boolean selectTab, boolean selectResult)
Add a result to the view identified by the given key.
  void [addResults](#addResults(java.lang.String,java.util.List,ro.sync.exml.workspace.api.results.ResultsManager.ResultType,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> results, [ResultsManager.ResultType](ResultsManager.ResultType.md) resultsType, boolean selectTab)
Append a list of results to the view identified by the given key.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> [getAllResults](#getAllResults(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey)
Get all the results from a tab.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> [getSelectedResults](#getSelectedResults(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey)
Get the results that are selected in a certain tab.
  void [removeEventHandler](#removeEventHandler(java.lang.String,ro.sync.exml.workspace.api.results.ResultsTabEventHandler))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabEventHandler](ResultsTabEventHandler.md) handler)
Remove the handler from the tab identified by the given key.
  void [removePopUpMenuCustomizer](#removePopUpMenuCustomizer(java.lang.String,ro.sync.exml.workspace.api.results.ResultsTabPopUpMenuCustomizer))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabPopUpMenuCustomizer](ResultsTabPopUpMenuCustomizer.md) customizer)
Remove a pop-up menu customizer from a specific results tab.
  void [removeResult](#removeResult(java.lang.String,ro.sync.document.DocumentPositionedInfo))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) result)
Remove the given result from the tab identified by the given key.
  void [selectResult](#selectResult(java.lang.String,ro.sync.document.DocumentPositionedInfo))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) result)
Select the given result from the tab identified by the given key.
  void [setResults](#setResults(java.lang.String,java.util.List,ro.sync.exml.workspace.api.results.ResultsManager.ResultType))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> results, [ResultsManager.ResultType](ResultsManager.ResultType.md) resultsType)
Set a new list of results in the view identified by the given key.

## Method Details

### setResults

void setResults([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> results, [ResultsManager.ResultType](ResultsManager.ResultType.md) resultsType)

Set a new list of results in the view identified by the given key. If a results view does not exist for the given key, a new one is created. The view is selected automatically when setting a list of results in it.
  Parameters: tabKey - The key identifying the view. It is set as the view's name. results - The list of new results. If null, the associated view is removed. resultsType - The type of the results. One of [ResultsManager.ResultType.PROBLEM](ResultsManager.ResultType.md#PROBLEM) or [ResultsManager.ResultType.GENERIC](ResultsManager.ResultType.md#GENERIC). It the type is [ResultsManager.ResultType.PROBLEM](ResultsManager.ResultType.md#PROBLEM), the results tab will display an icon corresponding to the severity of the results, otherwise it will not.
### addResult

void addResult([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) result, [ResultsManager.ResultType](ResultsManager.ResultType.md) resultType, boolean selectTab, boolean selectResult)

Add a result to the view identified by the given key. If a results view does not exist for the given key, a new one is created.
  Parameters: tabKey - The key identifying the view. It is set as the view's name. result - The result to add. If null, nothing happens. resultType - The type of the result. One of [ResultsManager.ResultType.PROBLEM](ResultsManager.ResultType.md#PROBLEM) or [ResultsManager.ResultType.GENERIC](ResultsManager.ResultType.md#GENERIC). It the type is [ResultsManager.ResultType.PROBLEM](ResultsManager.ResultType.md#PROBLEM), the results tab will display an icon corresponding to the severity of the results, otherwise it will not. If for the current call of this method the tab key is the same as for the previous, but the result type changes, the tab will first be cleared, before adding the current result. selectTab - true to select the tab when adding a result. selectResult - true to scroll to the added result and select it, if the results tab was not already focused.
### addResults

void addResults([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> results, [ResultsManager.ResultType](ResultsManager.ResultType.md) resultsType, boolean selectTab)

Append a list of results to the view identified by the given key. If a results view does not exist for the given key, a new one is created.
  Parameters: tabKey - The key identifying the view. It is set as the view's name. results - The list of results to append. If null, nothing happens. resultsType - The type of the results. One of [ResultsManager.ResultType.PROBLEM](ResultsManager.ResultType.md#PROBLEM) or [ResultsManager.ResultType.GENERIC](ResultsManager.ResultType.md#GENERIC). It the type is [ResultsManager.ResultType.PROBLEM](ResultsManager.ResultType.md#PROBLEM), the results tab will display an icon corresponding to the severity of the results, otherwise it will not. If for the current call of this method the tab key is the same as for the previous, but the result type changes, the tab will first be cleared, before adding the current results. selectTab - true to select the tab when adding the results.
### getAllResults

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> getAllResults([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey)

Get all the results from a tab.
  Parameters: tabKey - The key identifying the tab from which the results are to be retrieved. Returns: all the results or an empty list if the tab is empty or does not exist.
### getSelectedResults

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> getSelectedResults([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey)

Get the results that are selected in a certain tab.
  Parameters: tabKey - The key identifying the tab from which the selected results are to be retrieved. Returns: the selected results or an empty list if there are no results selected.
### addEventHandler

void addEventHandler([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabEventHandler](ResultsTabEventHandler.md) handler)

Add a handler for events from a results tab, such as clicks, double-clicks, pressing Enter on an entry, and others.
  Parameters: tabKey - The key identifying the tab on which the handler is added. handler - The handler.
### removeEventHandler

void removeEventHandler([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabEventHandler](ResultsTabEventHandler.md) handler)

Remove the handler from the tab identified by the given key.
  Parameters: tabKey - The key identifying the tab from which the handler is removed. handler - The handler.
### selectResult

void selectResult([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) result)

Select the given result from the tab identified by the given key. The tab is also selected.
  Parameters: tabKey - The key identifying the tab. result - The result to be selected.
### removeResult

void removeResult([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) result)

Remove the given result from the tab identified by the given key.
  Parameters: tabKey - The key identifying the tab. result - The result to be removed.
### addPopUpMenuCustomizer

void addPopUpMenuCustomizer([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabPopUpMenuCustomizer](ResultsTabPopUpMenuCustomizer.md) customizer)

Add a pop-up menu customizer for a specific results tab.
  Parameters: tabKey - The key identifying the tab for which the menu customizer is added. customizer - The customizer to add.
### removePopUpMenuCustomizer

void removePopUpMenuCustomizer([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey, [ResultsTabPopUpMenuCustomizer](ResultsTabPopUpMenuCustomizer.md) customizer)

Remove a pop-up menu customizer from a specific results tab.
  Parameters: tabKey - The key identifying the tab from which the menu customizer is removed. customizer - The customizer to remove.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
