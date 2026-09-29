Package [com.oxygenxml.editor.editors.author](package-summary.md)

# Interface AuthorDnDListener
    All Superinterfaces: [Extension](../../../../../ro/sync/ecss/extensions/api/Extension.md), [SWTExtension](../../../../../ro/sync/ecss/extensions/api/SWTExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorDnDListenerextends [SWTExtension](../../../../../ro/sync/ecss/extensions/api/SWTExtension.md)
Author Drag and Drop listener interface for the SWT implementation. The AuthorDnDListener class provides event notification to the author extension for DropTarget events.
As the user moves the cursor into, over and out of the author editor page, events indicate what operation can be performed and what data can be transferred if a drop where to occur at that point. The listener can respond to these events and change the type of data that will be dropped by modifying event.currentDataType, or change the operation that will be performed by modifying the event.detail field or stop any drop from happening on the current target by setting the event.detail field to DND_DROP_NONE.

When the user causes a drop to happen by releasing the mouse over the author editor page, the listener has one last chance to change the data type of the drop through the DropAccept event. If the drop is still allowed, the DropAccept event is immediately followed by the Drop event. In the Drop event, the listener can still change the operation that is performed but the data type is fixed.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [authorDragEnter](#authorDragEnter(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The cursor has entered the author editor page boundaries while dragging.
  void [authorDragLeave](#authorDragLeave(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The cursor has leaved the author editor page boundaries while dragging.
  void [authorDragOperationChanged](#authorDragOperationChanged(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The drag operation being performed has changed (usually due to the user changing the selected modifier key(s) while dragging).
  void [authorDragOver](#authorDragOver(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The cursor is moving over the author editor page while dragging.
  void [authorDrop](#authorDrop(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The data is being dropped in the author editor page.
  void [authorDropAccept](#authorDropAccept(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The drop is about to be performed.
  org.eclipse.swt.dnd.Transfer[] [getAuthorTransfers](#getAuthorTransfers())()
Get the data transfers of interest for the listener.
  void [init](#init(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) access)
Initialize the DnD listener.
  boolean [isAuthorEventOfInterest](#isAuthorEventOfInterest(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
Returns true if the DropTargetEvent is relevant for the listener and its information will be used in the other methods of this listener.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../../../ro/sync/ecss/extensions/api/Extension.md)
 [getDescription](../../../../../ro/sync/ecss/extensions/api/Extension.md#getDescription())
## Method Details

### isAuthorEventOfInterest

boolean isAuthorEventOfInterest(org.eclipse.swt.dnd.DropTargetEvent event)

Returns true if the DropTargetEvent is relevant for the listener and its information will be used in the other methods of this listener.
  Parameters: event - The DropTargetEvent to check. Returns: true if the given event is of interest for the listener.
### getAuthorTransfers

org.eclipse.swt.dnd.Transfer[] getAuthorTransfers()

Get the data transfers of interest for the listener.
  Returns: An array of Transfer objects representing the data transfers this listener is interested in.
### authorDragEnter

void authorDragEnter(org.eclipse.swt.dnd.DropTargetEvent event)

The cursor has entered the author editor page boundaries while dragging. For more details see DropTargetListener.dragEnter(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag enter event.
### authorDragLeave

void authorDragLeave(org.eclipse.swt.dnd.DropTargetEvent event)

The cursor has leaved the author editor page boundaries while dragging. For more details see DropTargetListener.dragLeave(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag leave event.
### authorDragOperationChanged

void authorDragOperationChanged(org.eclipse.swt.dnd.DropTargetEvent event)

The drag operation being performed has changed (usually due to the user changing the selected modifier key(s) while dragging). For more details see DropTargetListener.dragOperationChanged(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag operation changed event.
### authorDragOver

void authorDragOver(org.eclipse.swt.dnd.DropTargetEvent event)

The cursor is moving over the author editor page while dragging. For more details see DropTargetListener.dragOver(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag over event.
### authorDrop

void authorDrop(org.eclipse.swt.dnd.DropTargetEvent event)

The data is being dropped in the author editor page. The data field contains java format of the data being dropped. To determine the type of the data object, refer to the documentation for the Transfer subclass specified in event.currentDataType. For more details see DropTargetListener.drop(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drop event.
### authorDropAccept

void authorDropAccept(org.eclipse.swt.dnd.DropTargetEvent event)

The drop is about to be performed. The listener is given a last chance to change the nature of the drop. For more details see DropTargetListener.dropAccept(DropTargetEvent)and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drop accept event.
### init

void init([AuthorAccess](../../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) access)

Initialize the DnD listener. The [AuthorAccess](../../../../../ro/sync/ecss/extensions/api/AuthorAccess.md) can be used to access specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o.
  Parameters: access - The author access.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
