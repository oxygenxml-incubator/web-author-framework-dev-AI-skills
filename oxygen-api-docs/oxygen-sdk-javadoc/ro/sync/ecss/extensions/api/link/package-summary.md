# Package ro.sync.ecss.extensions.api.link

package ro.sync.ecss.extensions.api.link

Used for implementing navigation between links and their targets.
     Related Packages
Package

Description
 [ro.sync.ecss.extensions.api](../package-summary.md)
Main API package used for controlling the Author page (making modifications, adding listeners).
      All Classes and InterfacesInterfacesClassesEnum ClassesExceptions
Class

Description
 [Attr](Attr.md)
Contains informations about an attribute.
  [CannotRecognizeIDException](CannotRecognizeIDException.md)
Exception that is thrown when an ID cannot be recognized in the current context.
  [DefaultIDTypeIdentifier](DefaultIDTypeIdentifier.md)
Default implementation for [IDTypeIdentifier](IDTypeIdentifier.md).
  [ElementLocator](ElementLocator.md)
Base class for custom elements locators used to locate an element based on a link.
  [ElementLocatorException](ElementLocatorException.md)
Exception thrown when an element locator fails.
  [ElementLocatorProvider](ElementLocatorProvider.md)
This class is able to provide an implementation of an [ElementLocator](ElementLocator.md) based on the structure of a link.
  [ExtensionUtil](ExtensionUtil.md)
Utility methods.
  [IDTypeIdentifier](IDTypeIdentifier.md)
Identifier for an ID declaration or reference.
  [IDTypeRecognizer](IDTypeRecognizer.md)
Recognizer for ID declaration and references in attribute values.
  [IDTypeVerifier](IDTypeVerifier.md)
Interface used to check if an attribute has the ID type.
  [InvalidLinkException](InvalidLinkException.md)
Signals a link that cannot be resolved.
  [LinkTextResolver](LinkTextResolver.md)
Resolves a link and obtains a text representation.
  [Severity](Severity.md)
A hint about the severity of the exception.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
