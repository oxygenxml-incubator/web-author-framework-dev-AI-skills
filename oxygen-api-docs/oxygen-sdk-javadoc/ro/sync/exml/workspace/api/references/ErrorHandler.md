Package [ro.sync.exml.workspace.api.references](package-summary.md)

# Interface ErrorHandler
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ErrorHandler
ErrorHandler is an interface that the ReferenceCollectorimplementation can call when reporting errors that happens while collecting the references
  Since: 21.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [handleError](#handleError(ro.sync.exml.workspace.api.references.CollectingError))([CollectingError](CollectingError.md) error)
This method is called on the error handler when an error occurs.

## Method Details

### handleError

void handleError([CollectingError](CollectingError.md) error)

This method is called on the error handler when an error occurs.
  Parameters: error - the error to be handled
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
