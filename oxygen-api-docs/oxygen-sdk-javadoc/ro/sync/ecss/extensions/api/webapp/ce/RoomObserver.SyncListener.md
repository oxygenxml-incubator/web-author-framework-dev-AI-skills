Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface RoomObserver.SyncListener
    Enclosing interface: [RoomObserver](RoomObserver.md)   public static interface RoomObserver.SyncListener
Listener called when a batch of changes are synchronized.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [changesSynchronized](#changesSynchronized(int))(int peerId)
Invoked after changes made by an user were synchronized with the observer's state.

## Method Details

### changesSynchronized

void changesSynchronized(int peerId)

Invoked after changes made by an user were synchronized with the observer's state.
  Parameters: peerId - The peer ID of that user. This ID can be used as a parameter for [Room.getPeerContext(int)](Room.md#getPeerContext(int)) implementation to obtain contextual details about the user.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
