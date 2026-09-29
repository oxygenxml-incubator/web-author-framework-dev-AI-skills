Package [ro.sync.ecss.extensions.api.webapp.formcontrols](package-summary.md)

# Class WebappFormControlRendererRegistry

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.formcontrols.WebappFormControlRendererRegistry
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class WebappFormControlRendererRegistry extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Registry for form control renderers used in the Author Reviewer Webapp.

## Constructor Summary
 Constructors
Constructor

Description
 [WebappFormControlRendererRegistry](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHTMLContentCss](#getHTMLContentCss(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) htmlDescriptionURL)
Used from the context of an oxy_htmlContent() form control.
  [WebappFormControlRenderer](WebappFormControlRenderer.md) [getRenderer](#getRenderer(ro.sync.ecss.extensions.api.editor.AuthorInplaceContext))([AuthorInplaceContext](../../editor/AuthorInplaceContext.md) context)
Returns the renderer for the specified type of control.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WebappFormControlRendererRegistry

public WebappFormControlRendererRegistry()

Constructor.

## Method Details

### getRenderer

public [WebappFormControlRenderer](WebappFormControlRenderer.md) getRenderer([AuthorInplaceContext](../../editor/AuthorInplaceContext.md) context)

Returns the renderer for the specified type of control.
  Parameters: context - The type of the form-control. Returns: the renderer for the specified type of control.
### getHTMLContentCss

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHTMLContentCss([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) htmlDescriptionURL)

Used from the context of an oxy_htmlContent() form control. It given the CSS needed to render a block of documentation.
  Parameters: htmlDescriptionURL - The URL of the documentation html. The resolved value of oxy_htmlContent's parameter [InplaceEditorCSSConstants.PROPERTY_HREF](../../editor/InplaceEditorCSSConstants.md#PROPERTY_HREF). Returns: The CSS as string.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
