Package [ro.sync.exml.validate](package-summary.md)

# Interface IQuickFixableValidationProblem
    public interface IQuickFixableValidationProblem
Interface defining a validation problem that would be quick fixable.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addQuickFix](#addQuickFix(ro.sync.quickfix.IQuickFix))([IQuickFix](../../quickfix/IQuickFix.md) quickFix)
Adds a quick fix for this problem.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IQuickFix](../../quickfix/IQuickFix.md)> [getQuickFixes](#getQuickFixes())()

## Method Details

### addQuickFix

void addQuickFix([IQuickFix](../../quickfix/IQuickFix.md) quickFix)

Adds a quick fix for this problem.
  Parameters: quickFix - The quick fix to be added.
### getQuickFixes

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IQuickFix](../../quickfix/IQuickFix.md)> getQuickFixes()
  Returns: The list with available quick fixes for the current problem.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
