# Package ro.sync.ecss.extensions.commons

package ro.sync.ecss.extensions.commons

Common implementations for Docbook, DITA, TEI and XHTML (Java source also available in the Author SDK).
     Related Packages
Package

Description
 [ro.sync.ecss.extensions](../package-summary.md)

 [ro.sync.ecss.extensions.commons.editor](editor/package-summary.md)

 [ro.sync.ecss.extensions.commons.id](id/package-summary.md)

 [ro.sync.ecss.extensions.commons.imagemap](imagemap/package-summary.md)

 [ro.sync.ecss.extensions.commons.operations](operations/package-summary.md)

 [ro.sync.ecss.extensions.commons.sort](sort/package-summary.md)

 [ro.sync.ecss.extensions.commons.ui](ui/package-summary.md)

     All Classes and InterfacesInterfacesClassesExceptions
Class

Description
 [AbstractDocumentTypeHelper](AbstractDocumentTypeHelper.md)
Abstract implementation of the document type helper.
  [CannotEditException](CannotEditException.md)
Deprecated.
 [DefaultElementLocatorProvider](DefaultElementLocatorProvider.md)
Default implementation for locating elements based on a given link.
  [ExtensionTags](ExtensionTags.md)
The collection of the extension messages.
  [IDElementLocator](IDElementLocator.md)
Implementation of an ElementLocator that locates elements based on a given link and checks if the attribute with the type ID matches the provided link.
  [ImageFileChooser](ImageFileChooser.md)
Choose an image file.
  [MediaFileChooser](MediaFileChooser.md)
Choose an media file.
  [MediaObjectsUtil](MediaObjectsUtil.md)
Utility methods for media objects.
  [ObjectChooser](ObjectChooser.md)
Base class for choosers dialogs.
  [PasteAsReferenceException](PasteAsReferenceException.md)
Exception for when pasting as reference doesn't work properly.
  [XMLNodeRendererCustomizerAdapter](XMLNodeRendererCustomizerAdapter.md)
Empty implementation for [XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md).
  [XPointerElementLocator](XPointerElementLocator.md)
Element locator for links that have the one of the following patterns: element(elementID) - locate the element with the same id element(/1/2/5) - A child sequence appearing alone identifies an element by means of stepwise navigation, which is directed by a sequence of integers separated by slashes (/); each integer n locates the nth child element of the previously located element.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
