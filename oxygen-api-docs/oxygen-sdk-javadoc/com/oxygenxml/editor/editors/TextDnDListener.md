Package [com.oxygenxml.editor.editors](package-summary.md)

# Interface TextDnDListener
    All Superinterfaces: [Extension](../../../../ro/sync/ecss/extensions/api/Extension.md), [SWTExtension](../../../../ro/sync/ecss/extensions/api/SWTExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface TextDnDListenerextends [SWTExtension](../../../../ro/sync/ecss/extensions/api/SWTExtension.md)
Text Drag and Drop listener interface for the SWT implementation. The TextDnDListener class provides event notification to the Oxygen extension for DropTarget events occurring in the Text page.
As the user moves the cursor into, over and out of the text editor page, events indicate what operation can be performed and what data can be transferred if a drop where to occur at that point. The listener can respond to these events and change the type of data that will be dropped by modifying event.currentDataType, or change the operation that will be performed by modifying the event.detail field or stop any drop from happening on the current target by setting the event.detail field to DND_DROP_NONE.

When the user causes a drop to happen by releasing the mouse over the text editor page, the listener has one last chance to change the data type of the drop through the DropAccept event. If the drop is still allowed, the DropAccept event is immediately followed by the Drop event. In the Drop event, the listener can still change the operation that is performed but the data type is fixed.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 org.eclipse.swt.dnd.Transfer[] [getTextTransfers](#getTextTransfers())()
Get the data transfers of interest for the listener.
  void [init](#init(org.eclipse.swt.custom.StyledText,org.eclipse.jface.text.IDocument,java.lang.String))(org.eclipse.swt.custom.StyledText text, org.eclipse.jface.text.IDocument document, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)
Initialize the DnD listener.
  boolean [isTextEventOfInterest](#isTextEventOfInterest(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
Returns true if the DropTargetEvent is relevant for the listener and its information will be used in the other methods of this listener.
  void [textDragEnter](#textDragEnter(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The cursor has entered the text editor page boundaries while dragging.
  void [textDragLeave](#textDragLeave(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The cursor has leaved the text editor page boundaries while dragging.
  void [textDragOperationChanged](#textDragOperationChanged(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The drag operation being performed has changed (usually due to the user changing the selected modifier key(s) while dragging).
  void [textDragOver](#textDragOver(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The cursor is moving over the text editor page while dragging.
  void [textDrop](#textDrop(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The data is being dropped in the text editor page.
  void [textDropAccept](#textDropAccept(org.eclipse.swt.dnd.DropTargetEvent))(org.eclipse.swt.dnd.DropTargetEvent event)
The drop is about to be performed.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../../ro/sync/ecss/extensions/api/Extension.md)
 [getDescription](../../../../ro/sync/ecss/extensions/api/Extension.md#getDescription())
## Method Details

### isTextEventOfInterest

boolean isTextEventOfInterest(org.eclipse.swt.dnd.DropTargetEvent event)

Returns true if the DropTargetEvent is relevant for the listener and its information will be used in the other methods of this listener.
  Parameters: event - The DropTargetEvent to check Returns: true if the given event is of interest for the listener.
### getTextTransfers

org.eclipse.swt.dnd.Transfer[] getTextTransfers()

Get the data transfers of interest for the listener.
  Returns: An array of Transfer objects representing the data transfers this listener is interested in.
### textDragEnter

void textDragEnter(org.eclipse.swt.dnd.DropTargetEvent event)

The cursor has entered the text editor page boundaries while dragging. For more details see DropTargetListener.dragEnter(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag enter event.
### textDragLeave

void textDragLeave(org.eclipse.swt.dnd.DropTargetEvent event)

The cursor has leaved the text editor page boundaries while dragging. For more details see DropTargetListener.dragLeave(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag leave event.
### textDragOperationChanged

void textDragOperationChanged(org.eclipse.swt.dnd.DropTargetEvent event)

The drag operation being performed has changed (usually due to the user changing the selected modifier key(s) while dragging). For more details see DropTargetListener.dragOperationChanged(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag operation changed event.
### textDragOver

void textDragOver(org.eclipse.swt.dnd.DropTargetEvent event)

The cursor is moving over the text editor page while dragging. For more details see DropTargetListener.dragOver(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drag over event.
### textDrop

void textDrop(org.eclipse.swt.dnd.DropTargetEvent event)

The data is being dropped in the text editor page. The data field contains java format of the data being dropped. To determine the type of the data object, refer to the documentation for the Transfer subclass specified in event.currentDataType. For more details see DropTargetListener.drop(DropTargetEvent) and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drop event.
### textDropAccept

void textDropAccept(org.eclipse.swt.dnd.DropTargetEvent event)

The drop is about to be performed. The listener is given a last chance to change the nature of the drop. For more details see DropTargetListener.dropAccept(DropTargetEvent)and DropTargetEvent javadoc.
  Parameters: event - The information associated with the drop accept event.
### init

void init(org.eclipse.swt.custom.StyledText text, org.eclipse.jface.text.IDocument document, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)

Initialize the DnD listener.
  Parameters: text - The text component from the text editor page. document - The document from the text editor page. systemID - The system ID of the document.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
