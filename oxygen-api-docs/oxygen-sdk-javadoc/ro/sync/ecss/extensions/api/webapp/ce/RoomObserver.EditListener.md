Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface RoomObserver.EditListener
    Enclosing interface: [RoomObserver](RoomObserver.md)   public static interface RoomObserver.EditListener
Listener called when an edit happened in the room. In this case, the [RoomObserver.sync(SyncListener)](RoomObserver.md#sync(ro.sync.ecss.extensions.api.webapp.ce.RoomObserver.SyncListener)) should be called to synchronize the observer.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [editHappened](#editHappened())()
Called when an edit was performed by one of the user in the concurrent editing room.

## Method Details

### editHappened

void editHappened()

Called when an edit was performed by one of the user in the concurrent editing room.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
