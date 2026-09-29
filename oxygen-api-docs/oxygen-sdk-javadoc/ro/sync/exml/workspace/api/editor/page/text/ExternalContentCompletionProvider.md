Package [ro.sync.exml.workspace.api.editor.page.text](package-summary.md)

# Class ExternalContentCompletionProvider

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.text.ExternalContentCompletionProvider
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ExternalContentCompletionProvider extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
An external content completion provider. Can be used to display a custom content completion list, and insert content in the document. This provider is invoked if no built-in proposals are available for the current context.
  Since: 22.1
## Constructor Summary
 Constructors
Constructor

Description
 [ExternalContentCompletionProvider](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [startExternalContentCompletion](#startExternalContentCompletion(ro.sync.exml.workspace.api.editor.page.text.IExternalContentCompletionContext))([IExternalContentCompletionContext](IExternalContentCompletionContext.md) context)
Start an external content completion support.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ExternalContentCompletionProvider

public ExternalContentCompletionProvider()

## Method Details

### startExternalContentCompletion

public boolean startExternalContentCompletion([IExternalContentCompletionContext](IExternalContentCompletionContext.md) context)

Start an external content completion support.
  Parameters: context - The current content completion context, such as the position and the text from the caret. Returns: true if the event was consumed, and no other registered plugin should be notified to start the external content completion. false if the event was not consumed and other plugins can be notified to start the external content completion. Since: 22.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
