Package [ro.sync.ecss.dita.mapeditor.actions.export.helper](package-summary.md)

# Interface ExportProgressUpdater
    All Superinterfaces: [ProgressUpdater](../ProgressUpdater.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ExportProgressUpdaterextends [ProgressUpdater](../ProgressUpdater.md)
Interface used to update the progress component.
  Since: 18.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [done](#done())()
The operation progress is done.
  boolean [isCanceled](#isCanceled())()
Check if the progress is cancelled.
  void [start](#start())()
The operation progress is started.

### Methods inherited from interface ro.sync.ecss.dita.mapeditor.actions.export.[ProgressUpdater](../ProgressUpdater.md)
 [cancel](../ProgressUpdater.md#cancel()), [updateProgressStatus](../ProgressUpdater.md#updateProgressStatus(java.lang.String))
## Method Details

### start

void start()

The operation progress is started.

### isCanceled

boolean isCanceled()

Check if the progress is cancelled.
  Returns: true if the progress is canceled
### done

void done()

The operation progress is done.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
