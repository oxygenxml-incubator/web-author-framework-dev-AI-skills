Package [ro.sync.exml.workspace.api.images.handlers](package-summary.md)

# Class XMLImageHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.exml.workspace.api.images.handlers.ImageHandler](ImageHandler.md)
        * [ro.sync.exml.workspace.api.images.handlers.EditImageHandler](EditImageHandler.md)
            * ro.sync.exml.workspace.api.images.handlers.XMLImageHandler
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class XMLImageHandler extends [EditImageHandler](EditImageHandler.md)
Special handler for editing images defined as XML (SVG, MathML, etc). The image is either embedded in the XML content or referenced from it...
  Since: 18
## Constructor Summary
 Constructors
Constructor

Description
 [XMLImageHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 abstract boolean [canHandle](#canHandle(java.lang.String,java.lang.String,org.xml.sax.Attributes))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)
Check if can handle this XML fragment having a certain root name, namespace and attributes.
  abstract boolean [canHandleNamespace](#canHandleNamespace(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Checks if the element is recognized as an embedded image.
  boolean [canHandleNodeContext](#canHandleNodeContext(ro.sync.exml.workspace.api.node.NodeContext))([NodeContext](../../node/NodeContext.md) nodeContext)
Checks if the element is recognized as an embedded image.
  boolean [canHandleVectorialImages](#canHandleVectorialImages())()
Checks if current handler handles vectorial images (like SVG).

### Methods inherited from class ro.sync.exml.workspace.api.images.handlers.[EditImageHandler](EditImageHandler.md)
 [editImage](EditImageHandler.md#editImage(java.net.URL)), [editImage](EditImageHandler.md#editImage(ro.sync.exml.workspace.api.images.handlers.providers.EmbeddedImageContentProvider))
### Methods inherited from class ro.sync.exml.workspace.api.images.handlers.[ImageHandler](ImageHandler.md)
 [canHandleFileType](ImageHandler.md#canHandleFileType(java.lang.String)), [clearCache](ImageHandler.md#clearCache()), [getImage](ImageHandler.md#getImage(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext)), [getImageLayoutInformation](ImageHandler.md#getImageLayoutInformation(ro.sync.exml.workspace.api.images.handlers.providers.ImageContentProvider,ro.sync.exml.workspace.api.images.handlers.ImageRenderingContext))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XMLImageHandler

public XMLImageHandler()

## Method Details

### canHandleNamespace

public abstract boolean canHandleNamespace([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)

Checks if the element is recognized as an embedded image. For instance if the element is from the MathML namespace, then a MathML handler would return true, and it can be used to generate an image from it.
  Parameters: namespace - The namespace of the element from the document. Returns: True if the element was recognized by the handler - an image can be generated for it.
### canHandleNodeContext

public boolean canHandleNodeContext([NodeContext](../../node/NodeContext.md) nodeContext)

Checks if the element is recognized as an embedded image. For instance if the element is from the MathML namespace, then a MathML handler would return true, and it can be used to generate an image from it.
  Parameters: nodeContext - The context for an element. Returns: True if the element was recognized by the handler - an image can be generated for it.
### canHandle

public abstract boolean canHandle([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)

Check if can handle this XML fragment having a certain root name, namespace and attributes.
  Parameters: rootNamespace - The root namespace. rootLocalName - The root local name. rootAttributes - The root attributes. Returns: true if can handle this document.
### canHandleVectorialImages

public boolean canHandleVectorialImages()

Checks if current handler handles vectorial images (like SVG).
  Returns: true if current handler is for vectorial images. Since: 24.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
