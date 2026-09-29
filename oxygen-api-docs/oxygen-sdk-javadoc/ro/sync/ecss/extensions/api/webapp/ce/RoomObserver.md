Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface RoomObserver
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface RoomObserver
Observer for a [Room](Room.md), whose state can be used as a source of truth for the current state of the edited document.
  Since: 23
## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static interface  [RoomObserver.EditListener](RoomObserver.EditListener.md)
Listener called when an edit happened in the room.
  static interface  [RoomObserver.SyncListener](RoomObserver.SyncListener.md)
Listener called when a batch of changes are synchronized.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROOM_ID_HEADER](#ROOM_ID_HEADER)
The name of the header that contains the room ID in the [UserContext](../plugin/UserContext.md) of the observer.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addEditListener](#addEditListener(ro.sync.ecss.extensions.api.webapp.ce.RoomObserver.EditListener))([RoomObserver.EditListener](RoomObserver.EditListener.md) listener)
Register an edit listener.
  [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [createInputStream](#createInputStream())()

 [UnsavedContentReferenceManager](../../access/UnsavedContentReferenceManager.md) [getUnsavedContentReferenceManager](#getUnsavedContentReferenceManager())()
Get the manager that can be used to find (and save) the resources whose content has been modified in-place, by editing the expanded references.
  [UserContext](../plugin/UserContext.md) [getUserContext](#getUserContext())()
Sometimes, the room observer needs to open URL connections to fetch resourced referenced in the editor.
  void [removeEditListener](#removeEditListener(ro.sync.ecss.extensions.api.webapp.ce.RoomObserver.EditListener))([RoomObserver.EditListener](RoomObserver.EditListener.md) listener)
Unregister an edit listener.
  void [sync](#sync(ro.sync.ecss.extensions.api.webapp.ce.RoomObserver.SyncListener))([RoomObserver.SyncListener](RoomObserver.SyncListener.md) listener)
Synchronizes the Observer's state with the latest changes in the room.

## Field Details

### ROOM_ID_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROOM_ID_HEADER

The name of the header that contains the room ID in the [UserContext](../plugin/UserContext.md) of the observer.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.ce.RoomObserver.ROOM_ID_HEADER)

## Method Details

### sync

void sync([RoomObserver.SyncListener](RoomObserver.SyncListener.md) listener)

Synchronizes the Observer's state with the latest changes in the room. The observer synchronizes its state with changes from multiple users that changed the document since the last sync. The observer tries to batch together as many changes from the same user as possible (without breaking causality of changes). After synchronizing changes from a single user the listener is called.
  Parameters: listener - The listener to call after synchronizing changes from an user.
### createInputStream

[InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) createInputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Returns: The input stream over the current content of the observer. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the input stream cannot be created.
### getUnsavedContentReferenceManager

[UnsavedContentReferenceManager](../../access/UnsavedContentReferenceManager.md) getUnsavedContentReferenceManager()

Get the manager that can be used to find (and save) the resources whose content has been modified in-place, by editing the expanded references.
  Returns: The unsaved references manager, or null if editing in references is not enabled.
### getUserContext

[UserContext](../plugin/UserContext.md) getUserContext()

Sometimes, the room observer needs to open URL connections to fetch resourced referenced in the editor. When it opens such connections, the [URLStreamHandlerWithContext](../plugin/URLStreamHandlerWithContext.md) instance will receive this [UserContext](../plugin/UserContext.md). The [UserContext](../plugin/UserContext.md) has the "service account" flag set to true and a header [ROOM_ID_HEADER](#ROOM_ID_HEADER) that contains the ID of the room.
  Returns: the [UserContext](../plugin/UserContext.md) instance used when opening URL connections.
### addEditListener

void addEditListener([RoomObserver.EditListener](RoomObserver.EditListener.md) listener)

Register an edit listener.
  Parameters: listener - The edit listener to register.
### removeEditListener

void removeEditListener([RoomObserver.EditListener](RoomObserver.EditListener.md) listener)

Unregister an edit listener.
  Parameters: listener - The edit listener to register.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
