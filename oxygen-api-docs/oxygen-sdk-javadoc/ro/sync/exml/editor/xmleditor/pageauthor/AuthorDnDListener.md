Package [ro.sync.exml.editor.xmleditor.pageauthor](package-summary.md)

# Interface AuthorDnDListener
    All Superinterfaces: [AWTExtension](../../../../ecss/extensions/api/AWTExtension.md), [Extension](../../../../ecss/extensions/api/Extension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorDnDListenerextends [AWTExtension](../../../../ecss/extensions/api/AWTExtension.md)
Author Drag and Drop listener interface for the AWT implementation. The AuthorDnDListener interface is the callback interface used by the author editor page to provide notification of DnD operations that involve it.
Create a listener object by implementing the interface and then when the drag enters, moves over, or exits the author editor page, when the drop action changes, and when the drop occurs, the relevant method in the listener object is invoked, and the DropTargetEvent is passed to it.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [authorDragEnter](#authorDragEnter(java.awt.dnd.DropTargetDragEvent))([DropTargetDragEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDragEvent.html) event)
Called while a drag operation is ongoing, when the mouse pointer enters the author editor page where this listener is registered.
  boolean [authorDragExit](#authorDragExit(java.awt.dnd.DropTargetEvent))([DropTargetEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetEvent.html) event)
Called while a drag operation is ongoing, when the mouse pointer has exited the author editor page where this listener is registered.
  boolean [authorDragOver](#authorDragOver(java.awt.dnd.DropTargetDragEvent))([DropTargetDragEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDragEvent.html) event)
Called when a drag operation is ongoing, while the mouse pointer is still over the author editor page where this listener is registered.
  boolean [authorDrop](#authorDrop(java.awt.datatransfer.Transferable,java.awt.dnd.DropTargetDropEvent))([Transferable](https://docs.oracle.com/en/java/javase/17/docs/api/java.datatransfer/java/awt/datatransfer/Transferable.html) transferable, [DropTargetDropEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDropEvent.html) event)
Called when the drag operation has terminated with a drop on the author editor page where this listener is registered.
  boolean [authorSupportsFlavor](#authorSupportsFlavor(java.awt.datatransfer.DataFlavor))([DataFlavor](https://docs.oracle.com/en/java/javase/17/docs/api/java.datatransfer/java/awt/datatransfer/DataFlavor.html) flavor)
Check if the data flavor can be handled by the listener.
  void [init](#init(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)
Initialize the DnD listener.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../../../../ecss/extensions/api/Extension.md)
 [getDescription](../../../../ecss/extensions/api/Extension.md#getDescription())
## Method Details

### authorDragOver

boolean authorDragOver([DropTargetDragEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDragEvent.html) event)

Called when a drag operation is ongoing, while the mouse pointer is still over the author editor page where this listener is registered.
  Parameters: event - The [DropTargetDropEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDropEvent.html) event. Returns: true if the listener handled the event.
### authorDrop

boolean authorDrop([Transferable](https://docs.oracle.com/en/java/javase/17/docs/api/java.datatransfer/java/awt/datatransfer/Transferable.html) transferable, [DropTargetDropEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDropEvent.html) event)

Called when the drag operation has terminated with a drop on the author editor page where this listener is registered.
This method is responsible for undertaking the transfer of the data associated with the gesture. The DropTargetDropEvent provides a means to obtain a Transferableobject that represents the data object(s) to be transfered.

  Parameters: transferable - The [Transferable](https://docs.oracle.com/en/java/javase/17/docs/api/java.datatransfer/java/awt/datatransfer/Transferable.html) object. event - The [DropTargetDragEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDragEvent.html) event. Returns: true if the listener handled the event.
### authorSupportsFlavor

boolean authorSupportsFlavor([DataFlavor](https://docs.oracle.com/en/java/javase/17/docs/api/java.datatransfer/java/awt/datatransfer/DataFlavor.html) flavor)

Check if the data flavor can be handled by the listener.
  Parameters: flavor - The [DataFlavor](https://docs.oracle.com/en/java/javase/17/docs/api/java.datatransfer/java/awt/datatransfer/DataFlavor.html) flavor. Returns: true if the flavor is supported.
### authorDragExit

boolean authorDragExit([DropTargetEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetEvent.html) event)

Called while a drag operation is ongoing, when the mouse pointer has exited the author editor page where this listener is registered.
  Parameters: event - The [DropTargetEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetEvent.html) event. Returns: true if the listener consumed the drag exit event.
### authorDragEnter

boolean authorDragEnter([DropTargetDragEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDragEvent.html) event)

Called while a drag operation is ongoing, when the mouse pointer enters the author editor page where this listener is registered.
  Parameters: event - The [DropTargetDragEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/dnd/DropTargetDragEvent.html) event. Returns: true if the listener consumed the drag enter event.
### init

void init([AuthorAccess](../../../../ecss/extensions/api/AuthorAccess.md) authorAccess)

Initialize the DnD listener.
  Parameters: authorAccess - The [AuthorAccess](../../../../ecss/extensions/api/AuthorAccess.md) providing access to specific components corresponding to editor, document, workspace, tables, change tracking and utility informations and actions.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
