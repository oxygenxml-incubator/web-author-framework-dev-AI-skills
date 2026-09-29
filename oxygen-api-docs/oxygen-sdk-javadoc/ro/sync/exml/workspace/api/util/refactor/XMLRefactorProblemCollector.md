Package [ro.sync.exml.workspace.api.util.refactor](package-summary.md)

# Interface XMLRefactorProblemCollector
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface XMLRefactorProblemCollector
Validation Utilities Problems Collector.
  Since: 28  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [problemsOccured](#problemsOccured(ro.sync.document.DocumentPositionedInfo%5B%5D))([DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md)[] problems)
Report that a set of problems occurred.

## Method Details

### problemsOccured

void problemsOccured([DocumentPositionedInfo](../../../../../document/DocumentPositionedInfo.md)[] problems)

Report that a set of problems occurred. May be called multiple times, usually for each validated file if problems are detected inside it.
  Parameters: problems - The DocumentPositionedInfo array containing possible problems.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
