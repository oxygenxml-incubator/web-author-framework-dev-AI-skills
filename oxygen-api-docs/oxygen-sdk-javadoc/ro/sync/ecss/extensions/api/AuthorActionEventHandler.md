Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorActionEventHandler
    All Superinterfaces: [Extension](Extension.md)   All Known Implementing Classes: [AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md), [DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md), [DITAAuthorActionEventHandler](DITAAuthorActionEventHandler.md), [DocbookAuthorActionEventHandler](DocbookAuthorActionEventHandler.md), [TEIAuthorActionEventHandler](TEIAuthorActionEventHandler.md), [XHTMLAuthorActionEventHandler](XHTMLAuthorActionEventHandler.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorActionEventHandlerextends [Extension](Extension.md)
Intercepts action events in the Author mode and can handle them in a special manner. Since 19.0 an AuthorActionEventHandlerBase extended API base has been added which can be extended to provide additional functionality.
  Since: 18
## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md)
Events that are delegated to this handler.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 default boolean [canHandleEvent](#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventDetails))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventDetails](AuthorActionEventDetails.md) eventDetails)
Check if an Author action event can be handled.
  boolean [canHandleEvent](#canHandleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)
Check if an Author action event can be handled.
  default [AuthorElement](node/AuthorElement.md) [getListItemAncestorToSplit](#getListItemAncestorToSplit(ro.sync.ecss.extensions.api.node.AuthorNode,ro.sync.ecss.extensions.api.AuthorAccess))([AuthorNode](node/AuthorNode.md) node, [AuthorAccess](AuthorAccess.md) access)
Return the list item ancestor of the current node that needs to be split on Enter.
  boolean [handleEvent](#handleEvent(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.AuthorActionEventHandler.AuthorActionEventType))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)
An event was generated.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### handleEvent

boolean handleEvent([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)

An event was generated.
  Parameters: authorAccess - Author access. eventType - The type of the generated event. Returns: true if the event was handled and the default operation should be skipped, false to let the default operation execute.
### canHandleEvent

boolean canHandleEvent([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md) eventType)

Check if an Author action event can be handled.
  Parameters: authorAccess - Access to the Author API. eventType - The type of event generated. Returns: true if the Author action event can be handled.
### canHandleEvent

default boolean canHandleEvent([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorActionEventDetails](AuthorActionEventDetails.md) eventDetails)

Check if an Author action event can be handled.
  Parameters: authorAccess - Access to the Author API. eventDetails - The details of the event generated. Returns: true if the Author action event can be handled.
### getListItemAncestorToSplit

default [AuthorElement](node/AuthorElement.md) getListItemAncestorToSplit([AuthorNode](node/AuthorNode.md) node, [AuthorAccess](AuthorAccess.md) access)

Return the list item ancestor of the current node that needs to be split on Enter.
  Parameters: node - The node. access - Access object to the Author API. Returns: the list item ancestor of the current node that needs to be split on Enter, or null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
