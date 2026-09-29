Package [ro.sync.exml.workspace.api.results](package-summary.md)

# Interface ResultsTabEventHandler
    @API(type=EXTENDABLE, src=PUBLIC) public interface ResultsTabEventHandler
Handles the event triggered inside a results tab.
  Since: 19.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [handle](#handle(ro.sync.exml.workspace.api.results.ResultsTabEvent))([ResultsTabEvent](ResultsTabEvent.md) event)
Handle the given event.

## Method Details

### handle

boolean handle([ResultsTabEvent](ResultsTabEvent.md) event)

Handle the given event.
  Parameters: event - The event to handle. Returns: true if the event was handled by this handler. In this case, the oXygen's default behaviour will not be performed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
