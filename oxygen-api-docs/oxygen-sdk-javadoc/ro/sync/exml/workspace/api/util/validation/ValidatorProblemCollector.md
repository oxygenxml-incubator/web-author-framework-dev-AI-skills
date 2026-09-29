Package [ro.sync.exml.workspace.api.util.validation](package-summary.md)

# Interface ValidatorProblemCollector
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ValidatorProblemCollector
Validation Utilities Problems Collector.
  Since: 25
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
