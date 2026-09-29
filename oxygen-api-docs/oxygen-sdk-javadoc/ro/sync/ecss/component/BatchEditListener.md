Package [ro.sync.ecss.component](package-summary.md)

# Interface BatchEditListener
    All Known Subinterfaces: [RenderingInfoChangedListener](RenderingInfoChangedListener.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface BatchEditListener
The edit events sometimes come in batches, for example when an undo is executed. One may choose to update the UI only at the end of such a batch. This interface is notified when a batch of events starts and ends.
  Since: 16
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [beginEdit](#beginEdit())()
Method to be called before a batch of events.
  void [endEdit](#endEdit())()
Method to be called at the end of a batch of events.

## Method Details

### beginEdit

void beginEdit()

Method to be called before a batch of events. beginEdit and endEdit can't be nested. If beginEdit is called more than once before an endEdit then events will be lost.

### endEdit

void endEdit()

Method to be called at the end of a batch of events.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
