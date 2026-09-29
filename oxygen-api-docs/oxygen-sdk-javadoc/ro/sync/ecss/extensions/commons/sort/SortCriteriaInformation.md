Package [ro.sync.ecss.extensions.commons.sort](package-summary.md)

# Class SortCriteriaInformation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.sort.SortCriteriaInformation
   @API(type=INTERNAL, src=PUBLIC) public class SortCriteriaInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds information about the sort criteria and scope.

## Field Summary
 Fields
Modifier and Type

Field

Description
 final [CriterionInformation](CriterionInformation.md)[] [criteriaInfo](#criteriaInfo)
The criteria information array.
  final boolean [onlySelectedElements](#onlySelectedElements)
true when the sort scope is represented only by the selected elements.

## Constructor Summary
 Constructors
Constructor

Description
 [SortCriteriaInformation](#%3Cinit%3E(ro.sync.ecss.extensions.commons.sort.CriterionInformation%5B%5D,boolean))([CriterionInformation](CriterionInformation.md)[] info, boolean onlySelectedEntries)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### onlySelectedElements

public final boolean onlySelectedElements

true when the sort scope is represented only by the selected elements.

### criteriaInfo

public final [CriterionInformation](CriterionInformation.md)[] criteriaInfo

The criteria information array.

## Constructor Details

### SortCriteriaInformation

public SortCriteriaInformation([CriterionInformation](CriterionInformation.md)[] info, boolean onlySelectedEntries)

Constructor.
  Parameters: info - Array containing the [CriterionInformation](CriterionInformation.md)objects which will be used to sort the element. onlySelectedEntries - true if the scope of the sort is "Selected elements", false for "All elements".
## Method Details

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
