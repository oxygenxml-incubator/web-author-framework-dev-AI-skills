Package [ro.sync.diff.api](package-summary.md)

# Interface DiffProgressListener
    @API(type=EXTENDABLE, src=PUBLIC) public interface DiffProgressListener
Listener to the diff performer. It sends change events when the progress in the diff process is increased and a done event when the diff process is finished.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [finished](#finished())()
Event send by the diff process when is finished.
  void [start](#start())()
Called when the diff process is starting.
  void [update](#update(ro.sync.diff.api.DiffProgressEvent))([DiffProgressEvent](DiffProgressEvent.md) progressEvent)
Called when the progress in the diff process was increased.

## Method Details

### start

void start()

Called when the diff process is starting.

### update

void update([DiffProgressEvent](DiffProgressEvent.md) progressEvent)

Called when the progress in the diff process was increased.
  Parameters: progressEvent - The diff progress event. It contains information about the current progress in the diff process.
### finished

void finished()

Event send by the diff process when is finished.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
