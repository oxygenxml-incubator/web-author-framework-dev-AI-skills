Package [ro.sync.exml.workspace.api.editor.validation](package-summary.md)

# Class ValidationProblemsFilter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.validation.ValidationProblemsFilter
   @API(type=EXTENDABLE, src=PUBLIC) public class ValidationProblemsFilter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Filter which can be used by the user to ignore (or add) to the list of validation problems found by the validation process (manual or automatic) for a certain file.
  Since: 13
## Constructor Summary
 Constructors
Constructor

Description
 [ValidationProblemsFilter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [filterValidationProblems](#filterValidationProblems(ro.sync.exml.workspace.api.editor.validation.ValidationProblems))([ValidationProblems](ValidationProblems.md) validationProblems)
Callback received before (automatic or manual) validation problems are reported by Oxygen in the GUI.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ValidationProblemsFilter

public ValidationProblemsFilter()

## Method Details

### filterValidationProblems

public void filterValidationProblems([ValidationProblems](ValidationProblems.md) validationProblems)

Callback received before (automatic or manual) validation problems are reported by Oxygen in the GUI.
  Parameters: validationProblems - The problems found by Oxygen.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
