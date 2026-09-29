# Package ro.sync.ecss.extensions.api.webapp

package ro.sync.ecss.extensions.api.webapp
    Related Packages
Package

Description
 [ro.sync.ecss.extensions.api](../package-summary.md)
Main API package used for controlling the Author page (making modifications, adding listeners).
  [ro.sync.ecss.extensions.api.webapp.access](access/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.attributes](attributes/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.cc](cc/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.ce](ce/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.doctype](doctype/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.findreplace](findreplace/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.formcontrols](formcontrols/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.imagemap](imagemap/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.license](license/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.plugin](plugin/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.profiling](profiling/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.references](references/package-summary.md)

 [ro.sync.ecss.extensions.api.webapp.review](review/package-summary.md)

     All Classes and InterfacesInterfacesClassesEnum ClassesAnnotation Interfaces
Class

Description
 [AuthorDocumentModel](AuthorDocumentModel.md)
The model of an XML document to be edited.
  [AuthorDocumentModelContextManager](AuthorDocumentModelContextManager.md)
A helper class that handles the current editing context.

[AuthorIdIndex](AuthorIdIndex.md)<T>

An index that maps from IDs to objects and viceversa.
  [AuthorOperationWithResult](AuthorOperationWithResult.md)
Operation that returns a result when invoked from the Web Author JS API.
  [DPILocation](DPILocation.md)
DPI location information.
  [HTMLClasses](HTMLClasses.md)
HTML classes used to identify the role of HTML elements.
  [SafeAuthorOperation](SafeAuthorOperation.md)
Deprecated.
This interface is not used anymore as marker interface for operations that can be invoked via REST API with user supplied arguments.

 [SessionStore](SessionStore.md)
A per-session key value store (sessionId, key, value).
  [SpellcheckingEngine](SpellcheckingEngine.md)

 [WebappActionsManager](WebappActionsManager.md)
Helper object that provides access to extension actions, and provides support for invoking operations.
  [WebappAuthorDocumentFactory](WebappAuthorDocumentFactory.md)
Factory class that creates the document model to be used in the Web Reviewer.
  [WebappAuthorDocumentFactoryConstants](WebappAuthorDocumentFactoryConstants.md)
Constants for the webapp document factory.
  [WebappAuthorSchemaAwareActionsHandler](WebappAuthorSchemaAwareActionsHandler.md)
Handles schema aware actions like paste.
  [WebappDocumentValidator](WebappDocumentValidator.md)

 [WebappLockManager](WebappLockManager.md)
The lock manager associated with a document.
  [WebappMessage](WebappMessage.md)
Webapp server message that is presented on client side.
  [WebappMessagesProvider](WebappMessagesProvider.md)
Gets all the error messages reported by the application.
  [WebappRestSafe](WebappRestSafe.md)
Annotation that should be placed on AuthorOperations to indicate that they are safe to be invoked in Web Author via a REST API with user supplied arguments.
  [WebappSchematronPhaseChooser](WebappSchematronPhaseChooser.md)
Interface that is asked to provide the schematron phase to use.
  [WebappSpellchecker](WebappSpellchecker.md)

 [WebAuthorSpellcheckErrorTypes](WebAuthorSpellcheckErrorTypes.md)
Spellcheck error types used for Web Author.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
