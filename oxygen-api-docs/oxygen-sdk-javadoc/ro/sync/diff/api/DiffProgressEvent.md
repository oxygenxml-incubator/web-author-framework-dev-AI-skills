Package [ro.sync.diff.api](package-summary.md)

# Interface DiffProgressEvent
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DiffProgressEvent
Event used by the [DiffProgressListener](DiffProgressListener.md) to signal when the diff progress is incremented.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getCount](#getCount())()

## Method Details

### getCount

int getCount()
  Returns: The current progress of the diff process, between 1 and 100.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
