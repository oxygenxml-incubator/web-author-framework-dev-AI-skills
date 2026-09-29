Package [ro.sync.exml.workspace.api.references](package-summary.md)

# Interface CollectingError
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface CollectingError
CollectingError is an interface that describes an error that happens while collecting references
  Since: 21.1
## Nested Class Summary
 Nested Classes
Modifier and Type

Interface

Description
 static enum  [CollectingError.Severity](CollectingError.Severity.md)
The severity of the error

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage())()

 [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) [getRelatedException](#getRelatedException())()
The exception related to the error if any.
  [CollectingError.Severity](CollectingError.Severity.md) [getSeverity](#getSeverity())()

## Method Details

### getMessage

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage()
  Returns: the message associated with this error
### getSeverity

[CollectingError.Severity](CollectingError.Severity.md) getSeverity()
  Returns: the severity of this error
### getRelatedException

[Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) getRelatedException()

The exception related to the error if any.
  Returns: the exception
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
