Package [ro.sync.ecss.extensions.api.component.listeners](package-summary.md)

# Class DITAMapTreeComponentListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.component.listeners.DITAMapTreeComponentListener
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class DITAMapTreeComponentListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
DITA Map tree component listener. Can be added to notify of global events which occur in the DITA Map Tree.
  Since: 14
## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapTreeComponentListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract void [documentTypeChanged](#documentTypeChanged())()
The editor document type changed (usually called after a document was loaded).
  abstract void [loadedDocumentChanged](#loadedDocumentChanged())()
The loaded document changed.
  abstract void [modifiedStateChanged](#modifiedStateChanged(boolean))(boolean modified)
The modified state of the component changed

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAMapTreeComponentListener

public DITAMapTreeComponentListener()

## Method Details

### modifiedStateChanged

public abstract void modifiedStateChanged(boolean modified)

The modified state of the component changed
  Parameters: modified - true if the edited text in the component is modified, false otherwise
### loadedDocumentChanged

public abstract void loadedDocumentChanged()

The loaded document changed. load(URL, Reader) was called

### documentTypeChanged

public abstract void documentTypeChanged()

The editor document type changed (usually called after a document was loaded).

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
