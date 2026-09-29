Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface Room
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Room
A room is an abstraction for a set of document models created for the same document. Such models belong to different users and are edited concurrently and synchronized in real-time. An document model that is part in a room is called a "peer".
  Since: 23
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PEER_ID_ATTRIBUTE](#PEER_ID_ATTRIBUTE)
Editing Session Context attribute to store the peer ID which is unique inside this room.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROOM_CREATOR_ATTRIBUTE](#ROOM_CREATOR_ATTRIBUTE)
Editing Session Context attribute that mark the room creator with "true" value.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ROOM_ID_ATTRIBUTE](#ROOM_ID_ATTRIBUTE)
Editing Session Context attribute to store the room ID.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [close](#close())()
Close the room.
  [RoomObserver](RoomObserver.md) [getObserver](#getObserver())()
Returns the room observer, useful for saving changes made in the room by multiple users.
  [PeerContext](PeerContext.md) [getPeerContext](#getPeerContext(int))(int peerId)
Get the peer context for a given peer.

## Field Details

### PEER_ID_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PEER_ID_ATTRIBUTE

Editing Session Context attribute to store the peer ID which is unique inside this room.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.ce.Room.PEER_ID_ATTRIBUTE)

### ROOM_ID_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROOM_ID_ATTRIBUTE

Editing Session Context attribute to store the room ID.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.ce.Room.ROOM_ID_ATTRIBUTE)

### ROOM_CREATOR_ATTRIBUTE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ROOM_CREATOR_ATTRIBUTE

Editing Session Context attribute that mark the room creator with "true" value.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.ce.Room.ROOM_CREATOR_ATTRIBUTE)

## Method Details

### getPeerContext

[PeerContext](PeerContext.md) getPeerContext(int peerId)

Get the peer context for a given peer.
  Parameters: peerId - The peer ID. Returns: The peer context.
### getObserver

[RoomObserver](RoomObserver.md) getObserver()

Returns the room observer, useful for saving changes made in the room by multiple users. Note: The room observer needs to be requested when the room is created.
  Returns: The room observer - used to observe changes to the document made in the room.
### close

void close()

Close the room. Should do any necessary cleanup and should notify all peers.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
