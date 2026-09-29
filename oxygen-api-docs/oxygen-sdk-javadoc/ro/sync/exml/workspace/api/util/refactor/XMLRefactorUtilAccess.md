Package [ro.sync.exml.workspace.api.util.refactor](package-summary.md)

# Interface XMLRefactorUtilAccess
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface XMLRefactorUtilAccess
XML Refactoring Utilities.
  Since: 28  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [listAllAvailableOperations](#listAllAvailableOperations())()
List all operations
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [listOperationParameters](#listOperationParameters(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationID)
List all parameters for an operation
  void [refactorXMLResources](#refactorXMLResources(java.util.Iterator,java.util.function.Function,java.util.function.BiConsumer,java.lang.String,java.util.Map,ro.sync.exml.workspace.api.util.refactor.XMLRefactorProblemCollector))([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, [BiConsumer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/BiConsumer.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentSaver, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationID, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> parameters, [XMLRefactorProblemCollector](XMLRefactorProblemCollector.md) problemsCollector)
XML refactor a set of resources.
  void [refactorXMLResources](#refactorXMLResources(java.util.Iterator,java.util.function.Function,java.util.function.BiConsumer,java.lang.String,ro.sync.exml.workspace.api.util.refactor.XMLRefactorProblemCollector))([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, [BiConsumer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/BiConsumer.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentSaver, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xsltStylesheetContent, [XMLRefactorProblemCollector](XMLRefactorProblemCollector.md) problemsCollector)
XML refactor a set of resources giving an XSLT stylesheet content.

## Method Details

### refactorXMLResources

void refactorXMLResources([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, [BiConsumer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/BiConsumer.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentSaver, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationID, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> parameters, [XMLRefactorProblemCollector](XMLRefactorProblemCollector.md) problemsCollector)

XML refactor a set of resources.
  Parameters: resourcesIterator - Iterator over the resources which need to be validated. Never null. contentProvider - Provides content to validate for a certain URL. Never null. contentSaver - Used to save the refactored content back. Never null. operationID - Operation ID. Never null. parameters - Parameters map. Can be null problemsCollector - The problems collector. Never null.
### refactorXMLResources

void refactorXMLResources([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, [BiConsumer](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/BiConsumer.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentSaver, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xsltStylesheetContent, [XMLRefactorProblemCollector](XMLRefactorProblemCollector.md) problemsCollector)

XML refactor a set of resources giving an XSLT stylesheet content.
  Parameters: resourcesIterator - Iterator over the resources which need to be validated. Never null. contentProvider - Provides content to validate for a certain URL. Never null. contentSaver - Used to save the refactored content back. Never null. xsltStylesheetContent - The XSLT stylesheet input source. Never null. problemsCollector - The problems collector. Never null.
### listAllAvailableOperations

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listAllAvailableOperations()

List all operations
  Returns: A JSON array with all available XML refactoring operation IDs and descriptions
### listOperationParameters

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listOperationParameters([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) operationID)

List all parameters for an operation
  Parameters: operationID - The operation ID Returns: A JSON array with all available parameters for a specific operation ID
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
