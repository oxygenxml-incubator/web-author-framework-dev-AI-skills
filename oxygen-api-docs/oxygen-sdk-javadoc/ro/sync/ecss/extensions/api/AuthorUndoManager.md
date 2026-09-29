Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorUndoManager

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [javax.swing.undo.AbstractUndoableEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/AbstractUndoableEdit.html)
        * [javax.swing.undo.CompoundEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html)
            * [javax.swing.undo.UndoManager](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html)
                * ro.sync.ecss.extensions.api.AuthorUndoManager
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [EventListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/EventListener.html), [UndoableEditListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/UndoableEditListener.html), [UndoableEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoableEdit.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public abstract class AuthorUndoManager extends [UndoManager](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html)
Undo manager for Author edits. It allows to register listeners that are notified when undoable edits occur.
  Since: 23.1 See Also:
* [Serialized Form](../../../../../serialized-form.md#ro.sync.ecss.extensions.api.AuthorUndoManager)

## Field Summary

### Fields inherited from class javax.swing.undo.[CompoundEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html)
 [edits](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html#edits)
### Fields inherited from class javax.swing.undo.[AbstractUndoableEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/AbstractUndoableEdit.html)
 [RedoName](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/AbstractUndoableEdit.html#RedoName), [UndoName](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/AbstractUndoableEdit.html#UndoName)
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorUndoManager](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract void [addUndoableEditListener](#addUndoableEditListener(javax.swing.event.UndoableEditListener))([UndoableEditListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/UndoableEditListener.html) listener)
Registers an UndoableEditListener.
  abstract void [removeUndoableEditListener](#removeUndoableEditListener(javax.swing.event.UndoableEditListener))([UndoableEditListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/UndoableEditListener.html) listener)
Remove a listener for undoable edits.

### Methods inherited from class javax.swing.undo.[UndoManager](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html)
 [addEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#addEdit(javax.swing.undo.UndoableEdit)), [canRedo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#canRedo()), [canUndo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#canUndo()), [canUndoOrRedo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#canUndoOrRedo()), [discardAllEdits](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#discardAllEdits()), [editToBeRedone](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#editToBeRedone()), [editToBeUndone](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#editToBeUndone()), [end](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#end()), [getLimit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#getLimit()), [getRedoPresentationName](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#getRedoPresentationName()), [getUndoOrRedoPresentationName](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#getUndoOrRedoPresentationName()), [getUndoPresentationName](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#getUndoPresentationName()), [redo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#redo()), [redoTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#redoTo(javax.swing.undo.UndoableEdit)), [setLimit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#setLimit(int)), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#toString()), [trimEdits](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#trimEdits(int,int)), [trimForLimit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#trimForLimit()), [undo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#undo()), [undoableEditHappened](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#undoableEditHappened(javax.swing.event.UndoableEditEvent)), [undoOrRedo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#undoOrRedo()), [undoTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html#undoTo(javax.swing.undo.UndoableEdit))
### Methods inherited from class javax.swing.undo.[CompoundEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html)
 [die](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html#die()), [getPresentationName](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html#getPresentationName()), [isInProgress](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html#isInProgress()), [isSignificant](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html#isSignificant()), [lastEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html#lastEdit())
### Methods inherited from class javax.swing.undo.[AbstractUndoableEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/AbstractUndoableEdit.html)
 [replaceEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/AbstractUndoableEdit.html#replaceEdit(javax.swing.undo.UndoableEdit))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorUndoManager

public AuthorUndoManager()

## Method Details

### addUndoableEditListener

public abstract void addUndoableEditListener([UndoableEditListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/UndoableEditListener.html) listener)

Registers an UndoableEditListener. The listener is notified when an edit occurs, with the **previous** undoable edit.
  Parameters: listener - The listener to be added
### removeUndoableEditListener

public abstract void removeUndoableEditListener([UndoableEditListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/UndoableEditListener.html) listener)

Remove a listener for undoable edits.
  Parameters: listener - The listener to be removed
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
