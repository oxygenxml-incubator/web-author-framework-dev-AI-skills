Package [com.oxygenxml.editor.editors](package-summary.md)

# Class StylesFilterContributor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * com.oxygenxml.editor.editors.StylesFilterContributor
   @API(type=EXTENDABLE, src=PUBLIC) public class StylesFilterContributor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provider for an author styles filter.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [StylesFilterContributor](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [StylesFilter](../../../../ro/sync/ecss/extensions/api/StylesFilter.md) [createStylesFilter](#createStylesFilter(java.net.URL,ro.sync.exml.workspace.api.editor.documenttype.DocumentTypeInformation))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resourceURL, [DocumentTypeInformation](../../../../ro/sync/exml/workspace/api/editor/documenttype/DocumentTypeInformation.md) documentTypeInfo)
Returns a styles filter for the current resource.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### StylesFilterContributor

public StylesFilterContributor()

## Method Details

### createStylesFilter

public [StylesFilter](../../../../ro/sync/ecss/extensions/api/StylesFilter.md) createStylesFilter([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resourceURL, [DocumentTypeInformation](../../../../ro/sync/exml/workspace/api/editor/documenttype/DocumentTypeInformation.md) documentTypeInfo)

Returns a styles filter for the current resource.
  Parameters: resourceURL - The URL of the open resource. documentTypeInfo - Provides information about the document type configuration which was loaded for the current editor. Returns: A styles filter implementation.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
