Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Class RoomsManager

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.ce.RoomsManager
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class RoomsManager extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class that manages the creation of instances concurrent editing [Room](Room.md).
  Since: 23
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [SaveStrategy](SaveStrategy.md) [DEFAULT_SAVE_STRATEGY](#DEFAULT_SAVE_STRATEGY)
Default save strategy used when no save strategy is explicitly specified when creating a room.
  static final [RoomsManager](RoomsManager.md) [INSTANCE](#INSTANCE)
Singleton instance.

## Constructor Summary
 Constructors
Constructor

Description
 [RoomsManager](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addRoomCreatedListener](#addRoomCreatedListener(ro.sync.ecss.extensions.api.webapp.ce.RoomCreatedListener))([RoomCreatedListener](RoomCreatedListener.md) listener)
Adds a listener to be called when a room is created.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createRoomFromDocument](#createRoomFromDocument(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([AuthorDocumentModel](../AuthorDocumentModel.md) model)
Create a room with a single document with default save strategy ([DefaultSaveStrategy](DefaultSaveStrategy.md)).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [createRoomFromDocument](#createRoomFromDocument(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel,ro.sync.ecss.extensions.api.webapp.ce.SaveStrategy))([AuthorDocumentModel](../AuthorDocumentModel.md) model, [SaveStrategy](SaveStrategy.md) saveStrategy)
Create a room with a single document.
  [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Room](Room.md)> [getRoom](#getRoom(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)
Return the room of a given document model.
  [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Room](Room.md)> [getRoomTryCreateProxy](#getRoomTryCreateProxy(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)
Return the room of a given document model.
  boolean [isEnabled](#isEnabled())()
The rooms manager is enabled when the Concurrent Editing plugin is installed.
  void [removeRoomCreatedListener](#removeRoomCreatedListener(ro.sync.ecss.extensions.api.webapp.ce.RoomCreatedListener))([RoomCreatedListener](RoomCreatedListener.md) listener)
Removes a listener.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### INSTANCE

public static final [RoomsManager](RoomsManager.md) INSTANCE

Singleton instance.

### DEFAULT_SAVE_STRATEGY

public static final [SaveStrategy](SaveStrategy.md) DEFAULT_SAVE_STRATEGY

Default save strategy used when no save strategy is explicitly specified when creating a room. Saves all changes at once, as the user who triggered the save.

## Constructor Details

### RoomsManager

public RoomsManager()

## Method Details

### createRoomFromDocument

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createRoomFromDocument([AuthorDocumentModel](../AuthorDocumentModel.md) model)

Create a room with a single document with default save strategy ([DefaultSaveStrategy](DefaultSaveStrategy.md)).
  Parameters: model - The document model. Returns: The room id.
### createRoomFromDocument

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) createRoomFromDocument([AuthorDocumentModel](../AuthorDocumentModel.md) model, [SaveStrategy](SaveStrategy.md) saveStrategy)

Create a room with a single document.
  Parameters: model - The document model. saveStrategy - The save details. Returns: The room id.
### getRoom

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Room](Room.md)> getRoom([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)

Return the room of a given document model.
  Parameters: roomId - The room ID. Returns: The document model.
### getRoomTryCreateProxy

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Room](Room.md)> getRoomTryCreateProxy([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) roomId)throws [RoomProxyCouldNotBeCreatedException](RoomProxyCouldNotBeCreatedException.md)

Return the room of a given document model. Tries to create a proxy room if the room doesn't exist on this server.
  Parameters: roomId - The room ID. Returns: The room instance for the given ID. Throws: [RoomProxyCouldNotBeCreatedException](RoomProxyCouldNotBeCreatedException.md) - If the instantiation of a proxy room fails.
### isEnabled

public boolean isEnabled()

The rooms manager is enabled when the Concurrent Editing plugin is installed.
  Returns: true if the concurrent editing support is enabled.
### addRoomCreatedListener

public void addRoomCreatedListener([RoomCreatedListener](RoomCreatedListener.md) listener)

Adds a listener to be called when a room is created.
  Parameters: listener - The listener to add Since: 26
### removeRoomCreatedListener

public void removeRoomCreatedListener([RoomCreatedListener](RoomCreatedListener.md) listener)

Removes a listener.
  Parameters: listener - The listener to remove. Since: 26
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
