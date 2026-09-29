Package [ro.sync.ecss.extensions.api.webapp.references](package-summary.md)

# Class DocumentModelReferenceCollector

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.references.DocumentModelReferenceCollector
   All Implemented Interfaces: [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class DocumentModelReferenceCollector extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md)
Instances of this class are used to collect the references to external resources (images, audio, video, XInclude, etc.) from an AuthorDocumentModelTo be used when the document has been already parsed and its structure is already known See URLCollectingReader for collecting references from a document specified by a URL

## Constructor Summary
 Constructors
Constructor

Description
 [DocumentModelReferenceCollector](#%3Cinit%3E(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel,ro.sync.exml.workspace.impl.references.CollectingStrategy))([AuthorDocumentModel](../AuthorDocumentModel.md) model, ro.sync.exml.workspace.impl.references.CollectingStrategy collector)
Creates a new DocumentModelReferenceCollector with a given model and collecting strategy

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Reference](../../../../../exml/workspace/api/references/Reference.md)> [collectReferences](#collectReferences())()
Returns a set of references collected from the document model
  [ErrorHandler](../../../../../exml/workspace/api/references/ErrorHandler.md) [getErrorHandler](#getErrorHandler())()
The error handler returned by this collector will always be null.
  void [setErrorHandler](#setErrorHandler(ro.sync.exml.workspace.api.references.ErrorHandler))([ErrorHandler](../../../../../exml/workspace/api/references/ErrorHandler.md) errorHandler)
Setting an error handler for this reference collector has no effect.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocumentModelReferenceCollector

public DocumentModelReferenceCollector([AuthorDocumentModel](../AuthorDocumentModel.md) model, ro.sync.exml.workspace.impl.references.CollectingStrategy collector)

Creates a new DocumentModelReferenceCollector with a given model and collecting strategy
  Parameters: model - the document model collector - the collecting strategy
## Method Details

### collectReferences

public [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[Reference](../../../../../exml/workspace/api/references/Reference.md)> collectReferences()

Returns a set of references collected from the document model
  Specified by: [collectReferences](../../../../../exml/workspace/api/references/ReferenceCollector.md#collectReferences()) in interface [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md) Returns: a set of references See Also:
        * [ReferenceCollector.collectReferences()](../../../../../exml/workspace/api/references/ReferenceCollector.md#collectReferences())

### setErrorHandler

public void setErrorHandler([ErrorHandler](../../../../../exml/workspace/api/references/ErrorHandler.md) errorHandler)

Setting an error handler for this reference collector has no effect. Any errors during the extractions of the references are only logged
  Specified by: [setErrorHandler](../../../../../exml/workspace/api/references/ReferenceCollector.md#setErrorHandler(ro.sync.exml.workspace.api.references.ErrorHandler)) in interface [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md)
### getErrorHandler

public [ErrorHandler](../../../../../exml/workspace/api/references/ErrorHandler.md) getErrorHandler()

The error handler returned by this collector will always be null. The metod is implemented to maintain backward compatibility with the API
  Specified by: [getErrorHandler](../../../../../exml/workspace/api/references/ReferenceCollector.md#getErrorHandler()) in interface [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md) Returns: the error handler - always null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
