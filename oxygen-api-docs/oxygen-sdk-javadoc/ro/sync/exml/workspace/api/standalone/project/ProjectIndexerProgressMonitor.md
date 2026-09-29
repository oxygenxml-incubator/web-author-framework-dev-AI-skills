Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Interface ProjectIndexerProgressMonitor
    @API(type=EXTENDABLE, src=PUBLIC) public interface ProjectIndexerProgressMonitor
Listener for indexing progress events.
  Since: 24.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [cancel](#cancel())()
Event sent when the re-index process was cancelled.
  void [endIndexing](#endIndexing())()
Event sent when the re-index process finished.
  boolean [isCanceled](#isCanceled())()
Probing the implementation to check if the indexing should stop.
  void [startIndexing](#startIndexing())()
Event sent when the re-index process has begun.
  void [updateDetailsMessage](#updateDetailsMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) detailsMessage)
Event that signals the status of the indexer has changed.
  void [updateIndexedResourcesCount](#updateIndexedResourcesCount(int))(int count)
Event that signals the number of indexed resources has increased.

## Method Details

### startIndexing

void startIndexing()

Event sent when the re-index process has begun.

### endIndexing

void endIndexing()

Event sent when the re-index process finished.

### cancel

void cancel()

Event sent when the re-index process was cancelled.

### updateDetailsMessage

void updateDetailsMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) detailsMessage)

Event that signals the status of the indexer has changed.
  Parameters: detailsMessage - The message that show the state of the indexer.
### updateIndexedResourcesCount

void updateIndexedResourcesCount(int count)

Event that signals the number of indexed resources has increased. Emmited between a [startIndexing()](#startIndexing()) and a [endIndexing()](#endIndexing()).
  Parameters: count - The new count.
### isCanceled

boolean isCanceled()

Probing the implementation to check if the indexing should stop.
  Returns: true if the indexing operation was canceled by the user and it should stop.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
