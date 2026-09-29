Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Interface SortCustomizer
    All Known Implementing Classes: [ECSortCustomizerDialog](ECSortCustomizerDialog.md), [SASortCustomizerDialog](SASortCustomizerDialog.md)   @API(type=INTERNAL, src=PUBLIC) public interface SortCustomizer
Used for customizing the sorting information, typically through user interaction.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [SortCriteriaInformation](SortCriteriaInformation.md) [getSortInformation](#getSortInformation(java.util.List,boolean,boolean))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criteriaInformation, boolean hasSelectedSortableElements, boolean cannotSortAllElements)
Obtain the sort information given some initial sort criteria.

## Method Details

### getSortInformation

[SortCriteriaInformation](SortCriteriaInformation.md) getSortInformation([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CriterionInformation](CriterionInformation.md)> criteriaInformation, boolean hasSelectedSortableElements, boolean cannotSortAllElements)

Obtain the sort information given some initial sort criteria.
  Parameters: criteriaInformation - The information about the available sorting criteria. hasSelectedSortableElements - true when elements selected in the document can be sorted. cannotSortAllElements - true when all the elements from the parent of the sort operation cannot be sorted. for example when the selected rows from a table can be sorted but the whole table cannot because it contains, outside the selected rows, some rows with multiple rowspan cells. Returns: The sort information, about criteria and the sort scope.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
