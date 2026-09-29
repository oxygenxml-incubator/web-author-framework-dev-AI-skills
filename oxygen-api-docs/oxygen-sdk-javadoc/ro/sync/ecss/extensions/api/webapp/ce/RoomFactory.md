Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface RoomFactory
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface RoomFactory
Factory for [Room](Room.md) objects.
  Since: 23
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addCommonEditingContextAttribute](#addCommonEditingContextAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)
Register an [EditingSessionContext](../../access/EditingSessionContext.md) attribute that is propagated from the first [AuthorDocumentModel](../AuthorDocumentModel.md) of a [Room](Room.md), to new [AuthorDocumentModel](../AuthorDocumentModel.md)s that are created inside that [Room](Room.md).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createRoom](#createRoom(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([AuthorDocumentModel](../AuthorDocumentModel.md) model)
Creates a room on this server starting from the given document model.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createRoom](#createRoom(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel,ro.sync.ecss.extensions.api.webapp.ce.SaveStrategy))([AuthorDocumentModel](../AuthorDocumentModel.md) model, [SaveStrategy](SaveStrategy.md) saveStrategy)
Creates a room on this server starting from the given document model.
  [Room](Room.md) [getRoom](#getRoom(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)
Returns the room with the given ID.
  [Room](Room.md) [getRoomTryCreateProxy](#getRoomTryCreateProxy(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)
Returns the room with the given ID.

## Method Details

### createRoom

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createRoom([AuthorDocumentModel](../AuthorDocumentModel.md) model)

Creates a room on this server starting from the given document model.
  Parameters: model - The document model. Returns: The room ID.
### createRoom

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createRoom([AuthorDocumentModel](../AuthorDocumentModel.md) model, [SaveStrategy](SaveStrategy.md) saveStrategy)

Creates a room on this server starting from the given document model.
  Parameters: model - The document model. saveStrategy - Details required for save. Returns: The room ID.
### getRoom

[Room](Room.md) getRoom([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)

Returns the room with the given ID.
  Parameters: roomId - The ID of the room. Returns: The room instance for a given ID, or null.
### getRoomTryCreateProxy

[Room](Room.md) getRoomTryCreateProxy([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)throws [RoomProxyCouldNotBeCreatedException](RoomProxyCouldNotBeCreatedException.md)

Returns the room with the given ID. Tries to create a proxy room if the room doesn't exist on this server.
  Parameters: roomId - The ID of the room. Returns: The room instance for a given ID, or null. Throws: [RoomProxyCouldNotBeCreatedException](RoomProxyCouldNotBeCreatedException.md) - If the instantiation of a proxy room fails.
### addCommonEditingContextAttribute

void addCommonEditingContextAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeName)

Register an [EditingSessionContext](../../access/EditingSessionContext.md) attribute that is propagated from the first [AuthorDocumentModel](../AuthorDocumentModel.md) of a [Room](Room.md), to new [AuthorDocumentModel](../AuthorDocumentModel.md)s that are created inside that [Room](Room.md).
  Parameters: attributeName - the common attribute name.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
