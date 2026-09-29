Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class ProfilingConditionalTextProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.ProfilingConditionalTextProvider
   @API(type=EXTENDABLE, src=PUBLIC) public class ProfilingConditionalTextProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
**Profiling/Conditional Text** is a way to mark elements meant to appear in some renditions of the document, but not in others. It differs from one variant of the document to another, while unconditional elements appear in all document versions.  This class provides custom support for **Profiling/Conditional Text**.
  Since: 13.2
## Constructor Summary
 Constructors
Constructor

Description
 [ProfilingConditionalTextProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXMLFragmentForContentProfiling](#getXMLFragmentForContentProfiling(int,int,ro.sync.ecss.extensions.api.AuthorAccess))(int startOffset, int endOffset, [AuthorAccess](AuthorAccess.md) authorAccess)
This method is used when the document content between startOffset and endOffset must be profiled.
  boolean [shouldAddProfilingDirectlyOnElement](#shouldAddProfilingDirectlyOnElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](node/AuthorElement.md) element)
This method is used to decide if the profiling attributes will be set directly on the element.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProfilingConditionalTextProvider

public ProfilingConditionalTextProvider()

## Method Details

### getXMLFragmentForContentProfiling

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXMLFragmentForContentProfiling(int startOffset, int endOffset, [AuthorAccess](AuthorAccess.md) authorAccess)

This method is used when the document content between startOffset and endOffset must be profiled. The returned XML fragment is used to wrap the content included in the given offset interval. The first leaf of the XML fragment will be the destination of the text to surround. The profiling attributes will be set on the first element of the XML fragment.
  Parameters: startOffset - The start offset of the document content that must be profiled. endOffset - The end offset of the document content that must be profiled. authorAccess - Access class to the author functions. Returns: The XML fragment to wrap the profiled document content with. If this fragment is null the interval will not be profiled. Since: 13.2
### shouldAddProfilingDirectlyOnElement

public boolean shouldAddProfilingDirectlyOnElement([AuthorElement](node/AuthorElement.md) element)

This method is used to decide if the profiling attributes will be set directly on the element. If this method returns false, the selected contetn will be wrapped in an XML fragment given by [getXMLFragmentForContentProfiling(int, int, AuthorAccess)](#getXMLFragmentForContentProfiling(int,int,ro.sync.ecss.extensions.api.AuthorAccess)).
  Parameters: element - The element to be analyzed. Returns: true to set the profiling attributes directly on the element, false to set the profiling on an XML fragment that will wrap the content of the element. Since: 22
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
