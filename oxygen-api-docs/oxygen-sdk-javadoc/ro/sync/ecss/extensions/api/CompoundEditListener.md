Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface CompoundEditListener
    All Known Subinterfaces: [AuthorListener](AuthorListener.md)   All Known Implementing Classes: [AuthorListenerAdapter](AuthorListenerAdapter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface CompoundEditListener
Listener notified when compound edits are started and ended.
  Since: 23
## Method Summary
  All MethodsInstance MethodsDefault Methods
Modifier and Type

Method

Description
 default void [beforeCompoundEditCancelled](#beforeCompoundEditCancelled())()
Called before a compound edit is cancelled.
  default void [compoundEditCancelled](#compoundEditCancelled())()
Called when a compound edit was cancelled.
  default void [compoundEditEnded](#compoundEditEnded())()
Called when a compound edit was ended.
  default void [compoundEditStarted](#compoundEditStarted())()
Called when a compound edit was started.

## Method Details

### compoundEditStarted

default void compoundEditStarted()

Called when a compound edit was started. A compound edit can be started by calling [AuthorDocumentController.beginCompoundEdit()](AuthorDocumentController.md#beginCompoundEdit()). Note that this callback will not be invoked for nested calls of [AuthorDocumentController.beginCompoundEdit()](AuthorDocumentController.md#beginCompoundEdit()), but only for the first one.

### compoundEditEnded

default void compoundEditEnded()

Called when a compound edit was ended. A compound edit can be ended by calling [AuthorDocumentController.endCompoundEdit()](AuthorDocumentController.md#endCompoundEdit()). Note that this callback will not be invoked for nested calls of [AuthorDocumentController.endCompoundEdit()](AuthorDocumentController.md#endCompoundEdit()), but only for the last one.

### compoundEditCancelled

default void compoundEditCancelled()

Called when a compound edit was cancelled. A compound edit can be cancelled by calling [AuthorDocumentController.cancelCompoundEdit()](AuthorDocumentController.md#cancelCompoundEdit()). When a compound edit is cancelled, the edits performed so far are automatically undone before this callback is invoked. After that, an [compoundEditEnded()](#compoundEditEnded()) call is also received.

### beforeCompoundEditCancelled

default void beforeCompoundEditCancelled()

Called before a compound edit is cancelled. A compound edit can be cancelled by calling [AuthorDocumentController.cancelCompoundEdit()](AuthorDocumentController.md#cancelCompoundEdit()). When a compound edit is cancelled, the edits performed so far are automatically undone before this callback is invoked. After that, an [compoundEditEnded()](#compoundEditEnded()) call is also received.
  Since: 23.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
