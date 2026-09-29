Package [ro.sync.ecss.extensions.xhtml.imagemap](package-summary.md)

# Class XHTMLWebappImageMapSupportFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.xhtml.imagemap.XHTMLWebappImageMapSupportFactory
   All Implemented Interfaces: [Extension](../../api/Extension.md), [WebappImageMapSupportFactory](../../api/webapp/imagemap/WebappImageMapSupportFactory.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLWebappImageMapSupportFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [WebappImageMapSupportFactory](../../api/webapp/imagemap/WebappImageMapSupportFactory.md)
Creates image map support objects for "map" elements.

## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLWebappImageMapSupportFactory](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [WebappImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupport.md) [createImageMapSupport](#createImageMapSupport(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)
Create an image map support.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLWebappImageMapSupportFactory

public XHTMLWebappImageMapSupportFactory()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### createImageMapSupport

public [WebappImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupport.md) createImageMapSupport([AuthorInplaceContext](../../api/editor/AuthorInplaceContext.md) context)throws [ImageMapFormatException](../../api/webapp/imagemap/ImageMapFormatException.md)
 Description copied from interface: [WebappImageMapSupportFactory](../../api/webapp/imagemap/WebappImageMapSupportFactory.md#createImageMapSupport(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))
Create an image map support.
  Specified by: [createImageMapSupport](../../api/webapp/imagemap/WebappImageMapSupportFactory.md#createImageMapSupport(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)) in interface [WebappImageMapSupportFactory](../../api/webapp/imagemap/WebappImageMapSupportFactory.md) Parameters: context - The context. Returns: The image map support. Throws: [ImageMapFormatException](../../api/webapp/imagemap/ImageMapFormatException.md) - When the image map cannot be parsed from the given context. See Also:
        * [WebappImageMapSupportFactory.createImageMapSupport(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext)](../../api/webapp/imagemap/WebappImageMapSupportFactory.md#createImageMapSupport(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
