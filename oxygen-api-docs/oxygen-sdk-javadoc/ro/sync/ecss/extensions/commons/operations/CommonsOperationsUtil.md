Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class CommonsOperationsUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil
   @API(type=INTERNAL, src=PUBLIC) public final class CommonsOperationsUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Util methods for common Author operations.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static class  [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md)
Interface used to check the elements that will be converted in other elements (table cells or list entries)
  static class  [CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)
Class containing the new fragment and info about it.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [buildFreshPrefix](#buildFreshPrefix(ro.sync.ecss.extensions.api.node.NamespaceContext))([NamespaceContext](../../api/node/NamespaceContext.md) namespaceContext)
Generates a prefix that is not yet bound to a namespace.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [expandAndResolvePath](#expandAndResolvePath(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path)
Resolves a path relative to the framework directory.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)> [getFragmentsForConversions](#getFragmentsForConversions(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil.ConversionElementHelper,java.util.List))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) helper, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../api/ContentInterval.md)> intervals)
Get selected content fragments to be converted to cell or list entries fragments.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocalName](#getLocalName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)
Get the local name from an qualified element or attribute name.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPrefix](#getPrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)
Get the proxy from an qualified element or attribute name.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)> [getSelectedFragmentsForConversions](#getSelectedFragmentsForConversions(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.operations.CommonsOperationsUtil.ConversionElementHelper))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) helper)
Get selected content fragments to be converted to cell or list entries fragments.
  static boolean [isAllowedElement](#isAllowedElement(java.lang.String,int,ro.sync.ecss.extensions.api.AuthorSchemaManager))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementLocalName, int offset, [AuthorSchemaManager](../../api/AuthorSchemaManager.md) authorSchemaManager)
Check if an element with the given local name is allowed at the caret offset.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [locateResourceInClasspath](#locateResourceInClasspath(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourceFileName)
Locate a certain resource in the classpath using its file name.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [locateResourceInClasspathFolder](#locateResourceInClasspathFolder(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) folderName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourceFileName)
Locate a certain resource in the classpath using its file name.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> [removeCurrentSelection](#removeCurrentSelection(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Remove current selection from Author.
  static void [removeEmptyElements](#removeEmptyElements(ro.sync.ecss.extensions.api.AuthorAccess,java.util.Collection))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> emptyElementsPositions)
Remove empty elements.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> [removeIntervals](#removeIntervals(ro.sync.ecss.extensions.api.AuthorAccess,java.util.List))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../api/ContentInterval.md)> selectionIntervals)
Remove current selection from Author.
  static void [removeUnwantedAttributes](#removeUnwantedAttributes(java.lang.String%5B%5D,ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,ro.sync.ecss.extensions.api.AuthorDocumentController))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] skippedAttributes, [AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) fragment, [AuthorDocumentController](../../api/AuthorDocumentController.md) controller)
Remove unwanted attributes.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [serializeAttributes](#serializeAttributes(java.util.Map,java.util.Collection))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributesToSkip)
Serialize attributes with a space before.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [setAttributeValue](#setAttributeValue(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement,javax.xml.namespace.QName,java.lang.String,boolean))([AuthorDocumentController](../../api/AuthorDocumentController.md) ctrl, [AuthorElement](../../api/node/AuthorElement.md) targetElement, [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) attributeQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean removeIfEmpty)
Sets an attribute value.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [setAttributeValue](#setAttributeValue(ro.sync.ecss.extensions.api.AuthorDocumentController,ro.sync.ecss.extensions.api.node.AuthorElement,javax.xml.namespace.QName,java.lang.String,java.lang.String,boolean))([AuthorDocumentController](../../api/AuthorDocumentController.md) ctrl, [AuthorElement](../../api/node/AuthorElement.md) targetElement, [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) attributeQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) normalizedValue, boolean removeIfEmpty)
Sets an attribute value.
  static void [surroundWithFragment](#surroundWithFragment(ro.sync.ecss.extensions.api.AuthorAccess,boolean,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, boolean schemaAware, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment)
Surround selection with fragment.
  static int [surroundWithFragment](#surroundWithFragment(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,int,int))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int start, int end)
Surround the content between start and end offset with the given fragment.
  static void [unwrapTags](#unwrapTags(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) nodeToUnwrap)
Unwrap node tags.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### serializeAttributes

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) serializeAttributes([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributes, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> attributesToSkip)

Serialize attributes with a space before.
  Parameters: attributes - The attributes to serialize. attributesToSkip - The names of the attributes to skip. Returns: The serialization.
### unwrapTags

public static void unwrapTags([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [AuthorNode](../../api/node/AuthorNode.md) nodeToUnwrap)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Unwrap node tags.
  Parameters: authorAccess - The Author access. nodeToUnwrap - The node to unwrap. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### surroundWithFragment

public static void surroundWithFragment([AuthorAccess](../../api/AuthorAccess.md) authorAccess, boolean schemaAware, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Surround selection with fragment.
  Parameters: authorAccess - Author access. schemaAware - true for schema aware operation xmlFragment - The xml fragment Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### surroundWithFragment

public static int surroundWithFragment([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xmlFragment, int start, int end)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Surround the content between start and end offset with the given fragment.
  Parameters: authorAccess - Author access. xmlFragment - The xml fragment start - The start offset. Inclusive. end - The end offset. Inclusive. Returns: Insertion offset. Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### setAttributeValue

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) setAttributeValue([AuthorDocumentController](../../api/AuthorDocumentController.md) ctrl, [AuthorElement](../../api/node/AuthorElement.md) targetElement, [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) attributeQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, boolean removeIfEmpty)

Sets an attribute value. If the value is null the attribute will be removed from the element. If the value is the empty string and removeIfEmpty is true the attribute will also be removed.
  Parameters: ctrl - Attribute controller. targetElement - The target element. attributeQName - Attribute to edit. value - Current value. Illegal characters in the value WILL NOT be escaped. removeIfEmpty - true to remove the attribute when an empty value is set. Returns: The QName with which the attribute was committed. From the given attributeQName only the local name and namespace are taken into account.
### setAttributeValue

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) setAttributeValue([AuthorDocumentController](../../api/AuthorDocumentController.md) ctrl, [AuthorElement](../../api/node/AuthorElement.md) targetElement, [QName](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/namespace/QName.html) attributeQName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) normalizedValue, boolean removeIfEmpty)

Sets an attribute value. If the value is null the attribute will be removed from the element. If the value is the empty string and removeIfEmpty is true the attribute will also be removed.
  Parameters: ctrl - Attribute controller. targetElement - The target element. attributeQName - Attribute to edit. value - Current value. Illegal characters in the value WILL NOT be escaped. All entities must be already escaped in this value. For example:
```
ab"c&$
```
 normalizedValue - The value with normalized whitespaces and expanded entities. For example:
```
ab"c&$
```
 removeIfEmpty - true to remove the attribute when an empty value is set. Returns: The QName with which the attribute was committed. From the given attributeQName only the local name and namespace are taken into account.
### buildFreshPrefix

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) buildFreshPrefix([NamespaceContext](../../api/node/NamespaceContext.md) namespaceContext)

Generates a prefix that is not yet bound to a namespace.
  Parameters: namespaceContext - Namespace context. Returns: A prefix not bound in the given context.
### locateResourceInClasspath

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) locateResourceInClasspath([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourceFileName)

Locate a certain resource in the classpath using its file name.
  Parameters: authorAccess - Author access. resourceFileName - The resource file name. Returns: The URL of the resource or null.
### locateResourceInClasspathFolder

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) locateResourceInClasspathFolder([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) folderName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resourceFileName)

Locate a certain resource in the classpath using its file name.
  Parameters: authorAccess - Author access. folderName - The name of the folder. resourceFileName - The resource file name. Returns: The URL of the resource or null.
### expandAndResolvePath

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) expandAndResolvePath([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path)

Resolves a path relative to the framework directory. Editor variables are also accepted and expanded. The path is also passed through the catalog mappings.
  Parameters: authorAccess - Author access. path - The path to resolve. Can be a file path, an URL path or a path relative to the framework directory. Editor variables are also accepted. The path is also passed through the catalog mappings. Returns: An URL or null if unable to expand the path to an URL.
### getPrefix

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)

Get the proxy from an qualified element or attribute name.
  Parameters: qName - q name Returns: the proxy or an empty string. Null if the argument is null.
### getLocalName

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocalName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) qName)

Get the local name from an qualified element or attribute name.
  Parameters: qName - q name Returns: the local name, or null if the argument is null.
### removeUnwantedAttributes

public static void removeUnwantedAttributes([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] skippedAttributes, [AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) fragment, [AuthorDocumentController](../../api/AuthorDocumentController.md) controller)

Remove unwanted attributes.
  Parameters: skippedAttributes - The attributes to be deleted. fragment - The author document fragment to be cleared. controller - The author document controller.
### removeCurrentSelection

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> removeCurrentSelection([AuthorAccess](../../api/AuthorAccess.md) authorAccess)

Remove current selection from Author.
  Parameters: authorAccess - Author access. Returns: A list with start positions for empty elements (after remove is done).
### removeIntervals

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> removeIntervals([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../api/ContentInterval.md)> selectionIntervals)

Remove current selection from Author.
  Parameters: authorAccess - Author access. selectionIntervals - The intervals. Returns: A list with start positions for empty elements (after remove is done).
### getSelectedFragmentsForConversions

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)> getSelectedFragmentsForConversions([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) helper)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Get selected content fragments to be converted to cell or list entries fragments.
  Parameters: authorAccess - The author access. helper - Used to check if the elements from selection can be converted in other elements (table cells or list entries) Returns: The selected content fragments to be converted to cell fragments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### getFragmentsForConversions

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CommonsOperationsUtil.SelectedFragmentInfo](CommonsOperationsUtil.SelectedFragmentInfo.md)> getFragmentsForConversions([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [CommonsOperationsUtil.ConversionElementHelper](CommonsOperationsUtil.ConversionElementHelper.md) helper, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[ContentInterval](../../api/ContentInterval.md)> intervals)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html), [AuthorOperationException](../../api/AuthorOperationException.md)

Get selected content fragments to be converted to cell or list entries fragments.
  Parameters: authorAccess - The author access. helper - Used to check if the elements from selection can be converted in other elements (table cells or list entries) intervals - The intervals to convert. Returns: The selected content fragments to be converted to cell fragments. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) [AuthorOperationException](../../api/AuthorOperationException.md)
### removeEmptyElements

public static void removeEmptyElements([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)> emptyElementsPositions)

Remove empty elements.
  Parameters: authorAccess - The Author access. emptyElementsPositions - Positions for empty elements
### isAllowedElement

public static boolean isAllowedElement([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementLocalName, int offset, [AuthorSchemaManager](../../api/AuthorSchemaManager.md) authorSchemaManager)throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Check if an element with the given local name is allowed at the caret offset.
  Parameters: elementLocalName - the local name of the element whose allowance we check. offset - the offset where the allowance of the element is checked. authorSchemaManager - the Author schema manager. Returns: true if an element with the given local name is allowed at the caret offset, false otherwise. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - When the offset is below zero or greater than the content.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
