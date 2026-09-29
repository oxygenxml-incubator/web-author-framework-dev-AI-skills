Package [ro.sync.exml.workspace.api.references](package-summary.md)

# Interface ReferenceCollector
    All Known Implementing Classes: [DocumentModelReferenceCollector](../../../../ecss/extensions/api/webapp/references/DocumentModelReferenceCollector.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ReferenceCollector
Implementations of this interface are used to collect the references to external resources (images, audio, video, XInclude, etc.). Errors and exceptions during the collect operation are handled by the ErrorHandler
  Since: 21.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Reference](Reference.md)> [collectReferences](#collectReferences())()
Collects the references in a document
  [ErrorHandler](ErrorHandler.md) [getErrorHandler](#getErrorHandler())()

 void [setErrorHandler](#setErrorHandler(ro.sync.exml.workspace.api.references.ErrorHandler))([ErrorHandler](ErrorHandler.md) errorHandler)
Specialized error handlers can be set using this method.

## Method Details

### setErrorHandler

void setErrorHandler([ErrorHandler](ErrorHandler.md) errorHandler)

Specialized error handlers can be set using this method.
  Parameters: errorHandler -
### getErrorHandler

[ErrorHandler](ErrorHandler.md) getErrorHandler()
  Returns: the error handler
### collectReferences

[Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Reference](Reference.md)> collectReferences()

Collects the references in a document
  Returns: a set of references
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
