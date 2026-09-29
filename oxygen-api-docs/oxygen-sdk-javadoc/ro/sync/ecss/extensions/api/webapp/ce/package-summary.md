# Package ro.sync.ecss.extensions.api.webapp.ce

package ro.sync.ecss.extensions.api.webapp.ce
    Related Packages
Package

Description
 [ro.sync.ecss.extensions.api.webapp](../package-summary.md)

     All Classes and InterfacesInterfacesClassesExceptions
Class

Description
 [DefaultSaveStrategy](DefaultSaveStrategy.md)
Default save strategy used when no save strategy is explicitly specified when creating a room.
  [GroupChangesForMultiplePeersStrategy](GroupChangesForMultiplePeersStrategy.md)
Details required when saving a concurrently edited document.
  [GroupChangesForSinglePeerStrategy](GroupChangesForSinglePeerStrategy.md)
Details required when saving a concurrently edited document.
  [PeerContext](PeerContext.md)
Context information about a document model that is part of a [Room](Room.md).
  [Room](Room.md)
A room is an abstraction for a set of document models created for the same document.
  [RoomCreatedListener](RoomCreatedListener.md)
Listener called when a room was created.
  [RoomFactory](RoomFactory.md)
Factory for [Room](Room.md) objects.
  [RoomObserver](RoomObserver.md)
Observer for a [Room](Room.md), whose state can be used as a source of truth for the current state of the edited document.
  [RoomObserver.EditListener](RoomObserver.EditListener.md)
Listener called when an edit happened in the room.
  [RoomObserver.SyncListener](RoomObserver.SyncListener.md)
Listener called when a batch of changes are synchronized.
  [RoomProxyCouldNotBeCreatedException](RoomProxyCouldNotBeCreatedException.md)
Exception to be thrown when the creation of a proxy room failed.
  [RoomsManager](RoomsManager.md)
Class that manages the creation of instances concurrent editing [Room](Room.md).
  [SaveStrategy](SaveStrategy.md)
Details required when saving a concurrently edited document.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
