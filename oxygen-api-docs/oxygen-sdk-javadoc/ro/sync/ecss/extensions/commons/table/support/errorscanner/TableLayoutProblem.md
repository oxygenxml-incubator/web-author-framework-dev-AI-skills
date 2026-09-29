Package [ro.sync.ecss.extensions.commons.table.support.errorscanner](package-summary.md)

# Interface TableLayoutProblem
    All Known Implementing Classes: [CALSAndHTMLTableLayoutProblem](CALSAndHTMLTableLayoutProblem.md)   @API(type=INTERNAL, src=PUBLIC) public interface TableLayoutProblem
Table layout problem
  Since: 18
## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md)
Problem severity

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage())()

 [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) [getSeverity](#getSeverity())()

## Method Details

### getSeverity

[TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) getSeverity()
  Returns: Returns the problem severity, one of [TableLayoutProblem.Severity](TableLayoutProblem.Severity.md) constants.
### getMessage

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage()
  Returns: Returns the problem message to be presented to the user.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
