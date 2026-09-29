Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface WebappExtensionsProvider
    @API(type=EXTENDABLE, src=PUBLIC) public interface WebappExtensionsProvider
Web Author specific extensions for a document type.
  Since: 21.1
## Method Summary
  All MethodsInstance MethodsDefault Methods
Modifier and Type

Method

Description
 default [ContentCompletionSortPriorityAssigner](webapp/cc/ContentCompletionSortPriorityAssigner.md) [getSortPriorityAssigner](#getSortPriorityAssigner())()
Used to specify an object that can modify the sort order of the content completion menu items.

## Method Details

### getSortPriorityAssigner

default [ContentCompletionSortPriorityAssigner](webapp/cc/ContentCompletionSortPriorityAssigner.md) getSortPriorityAssigner()

Used to specify an object that can modify the sort order of the content completion menu items.
  Returns: a sort priority assigner.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
