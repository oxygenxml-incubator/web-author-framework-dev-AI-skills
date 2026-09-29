Package [ro.sync.ecss.dita.mapeditor.actions.export](package-summary.md)

# Interface ProgressUpdater
    All Known Subinterfaces: [ExportProgressUpdater](helper/ExportProgressUpdater.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ProgressUpdater
Interface used to update the export progress dialog.
  Since: 18.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [cancel](#cancel())()
Cancels the progress dialog.
  void [updateProgressStatus](#updateProgressStatus(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) status)
Updates the status message of the progress dialog.

## Method Details

### updateProgressStatus

void updateProgressStatus([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) status)

Updates the status message of the progress dialog.
  Parameters: status - The status message.
### cancel

void cancel()

Cancels the progress dialog.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
