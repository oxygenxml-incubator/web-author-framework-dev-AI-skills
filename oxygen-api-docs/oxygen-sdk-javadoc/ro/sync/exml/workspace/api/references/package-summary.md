# Package ro.sync.exml.workspace.api.references

package ro.sync.exml.workspace.api.references
    Related Packages
Package

Description
 [ro.sync.exml.workspace.api](../package-summary.md)
API for accessing the application workspace.
      All Classes and InterfacesInterfacesClassesEnum Classes
Class

Description
 [CollectingError](CollectingError.md)
CollectingError is an interface that describes an error that happens while collecting references
  [CollectingError.Severity](CollectingError.Severity.md)
The severity of the error
  [ErrorHandler](ErrorHandler.md)
ErrorHandler is an interface that the ReferenceCollectorimplementation can call when reporting errors that happens while collecting the references
  [Reference](Reference.md)
Simple bean class used to contain references.
  [Reference.Type](Reference.Type.md)
Constants enumerating the resource types.
  [ReferenceCollector](ReferenceCollector.md)
Implementations of this interface are used to collect the references to external resources (images, audio, video, XInclude, etc.).
  [ReferenceCollectorFactory](ReferenceCollectorFactory.md)
Factory that creates ReferenceCollector objects to collect references from an XML document at specified URL.
  [ReferenceExtractor](ReferenceExtractor.md)
Interface used to extract a Reference from a node

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
