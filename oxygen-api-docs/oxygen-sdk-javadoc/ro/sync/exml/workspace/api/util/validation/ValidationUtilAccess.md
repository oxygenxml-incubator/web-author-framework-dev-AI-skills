Package [ro.sync.exml.workspace.api.util.validation](package-summary.md)

# Interface ValidationUtilAccess
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ValidationUtilAccess
Validation Utilities.
  Since: 25
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [validateResources](#validateResources(java.util.Iterator,boolean,ro.sync.exml.workspace.api.util.validation.ValidatorProblemCollector))([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, boolean validateOnlyXMLResources, [ValidatorProblemCollector](ValidatorProblemCollector.md) problemsCollector)
Validate a set of resources.
  void [validateResources](#validateResources(java.util.Iterator,java.util.function.Function,boolean,ro.sync.exml.workspace.api.util.validation.ValidatorProblemCollector))([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, boolean validateOnlyXMLResources, [ValidatorProblemCollector](ValidatorProblemCollector.md) problemsCollector)
Validate a set of resources.
  void [validateResources](#validateResources(java.util.Iterator,java.util.function.Function,boolean,ro.sync.exml.workspace.api.util.validation.ValidatorProblemCollector,java.util.Map))([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, boolean validateOnlyXMLResources, [ValidatorProblemCollector](ValidatorProblemCollector.md) problemsCollector, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> extraContext)
Validate a set of resources.

## Method Details

### validateResources

void validateResources([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, boolean validateOnlyXMLResources, [ValidatorProblemCollector](ValidatorProblemCollector.md) problemsCollector)

Validate a set of resources.
  Parameters: resourcesIterator - Iterator over the resources which need to be validated. Never null. validateOnlyXMLResources - true to validate only XML resources. problemsCollector - The problems collector. Never null.
### validateResources

void validateResources([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, boolean validateOnlyXMLResources, [ValidatorProblemCollector](ValidatorProblemCollector.md) problemsCollector)

Validate a set of resources.
  Parameters: resourcesIterator - Iterator over the resources which need to be validated. Never null. contentProvider - Provides content to validate for a certain URL. validateOnlyXMLResources - true to validate only XML resources. problemsCollector - The problems collector. Never null. Since: 27.0
### validateResources

void validateResources([Iterator](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Iterator.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> resourcesIterator, [Function](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Function.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> contentProvider, boolean validateOnlyXMLResources, [ValidatorProblemCollector](ValidatorProblemCollector.md) problemsCollector, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> extraContext)

Validate a set of resources.
  Parameters: resourcesIterator - Iterator over the resources which need to be validated. Never null. contentProvider - Provides content to validate for a certain URL. validateOnlyXMLResources - true to validate only XML resources. problemsCollector - The problems collector. Never null. extraContext - A map containing additional application context or information needed by the function. When called from WebAuthor, it will contain an "author_document_model" key with the [AuthorDocumentModel](../../../../../ecss/extensions/api/webapp/AuthorDocumentModel.md) of the current editor. It will also contain a "session_id" key with a unique identifier assigned to the execution request session. Since: 28.1 \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
