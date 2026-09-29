Package [ro.sync.exml.workspace.api.results](package-summary.md)

# Interface ResultsTabEvent
    @API(type=EXTENDABLE, src=PUBLIC) public interface ResultsTabEvent
An event triggered inside a results tab.
  Since: 19.0
## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [ResultsTabEvent.ResultsTabEventType](ResultsTabEvent.ResultsTabEventType.md)
The type of the event from the results tab.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [ResultsTabEvent.ResultsTabEventType](ResultsTabEvent.ResultsTabEventType.md) [getEventType](#getEventType())()
Gets the event type.
  [DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) [getResultItem](#getResultItem())()
Gets the result from the results tab for which the event was triggered.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTabKey](#getTabKey())()
Gets the key identifying the tab where the event was triggered.

## Method Details

### getTabKey

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTabKey()

Gets the key identifying the tab where the event was triggered.
  Returns: Returns the key identifying the tab where the event was triggered.
### getResultItem

[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md) getResultItem()

Gets the result from the results tab for which the event was triggered.
  Returns: Returns the result for which the event was triggered.
### getEventType

[ResultsTabEvent.ResultsTabEventType](ResultsTabEvent.ResultsTabEventType.md) getEventType()

Gets the event type. One of the values defined in [ResultsTabEvent.ResultsTabEventType](ResultsTabEvent.ResultsTabEventType.md).
  Returns: Returns the event type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
