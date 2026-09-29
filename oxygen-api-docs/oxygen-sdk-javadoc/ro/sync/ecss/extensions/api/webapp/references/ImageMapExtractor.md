Package [ro.sync.ecss.extensions.api.webapp.references](package-summary.md)

# Class ImageMapExtractor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.references.ImageMapExtractor
   All Implemented Interfaces: [ReferenceExtractor](../../../../../exml/workspace/api/references/ReferenceExtractor.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class ImageMapExtractor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ReferenceExtractor](../../../../../exml/workspace/api/references/ReferenceExtractor.md)
Returns an optional Reference with type Type.STATIC_CONTENT and the URL of the image map.

## Constructor Summary
 Constructors
Constructor

Description
 [ImageMapExtractor](#%3Cinit%3E(ro.sync.ecss.css.StyleSheet))(ro.sync.ecss.css.StyleSheet stylesheet)
Creates and extractor with the given stylesheet

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Reference](../../../../../exml/workspace/api/references/Reference.md)> [extract](#extract(ro.sync.ecss.dom.AuthorSentinelNode))(ro.sync.ecss.dom.AuthorSentinelNode node)
Returns a Reference for the external resource

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ImageMapExtractor

public ImageMapExtractor(ro.sync.ecss.css.StyleSheet stylesheet)

Creates and extractor with the given stylesheet
  Parameters: stylesheet -
## Method Details

### extract

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Reference](../../../../../exml/workspace/api/references/Reference.md)> extract(ro.sync.ecss.dom.AuthorSentinelNode node)
 Description copied from interface: [ReferenceExtractor](../../../../../exml/workspace/api/references/ReferenceExtractor.md#extract(ro.sync.ecss.dom.AuthorSentinelNode))
Returns a Reference for the external resource
  Specified by: [extract](../../../../../exml/workspace/api/references/ReferenceExtractor.md#extract(ro.sync.ecss.dom.AuthorSentinelNode)) in interface [ReferenceExtractor](../../../../../exml/workspace/api/references/ReferenceExtractor.md) Parameters: node - the document node Returns: reference data of the external resource associated with the node See Also:
        * [ReferenceExtractor.extract(ro.sync.ecss.dom.AuthorSentinelNode)](../../../../../exml/workspace/api/references/ReferenceExtractor.md#extract(ro.sync.ecss.dom.AuthorSentinelNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
