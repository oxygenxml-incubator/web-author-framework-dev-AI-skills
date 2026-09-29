Package [ro.sync.exml.plugin.document](package-summary.md)

# Class DocumentPluginResultImpl

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.plugin.document.DocumentPluginResultImpl
   All Implemented Interfaces: [DocumentPluginResult](DocumentPluginResult.md)   @API(type=EXTENDABLE, src=PUBLIC) public class DocumentPluginResultImpl extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [DocumentPluginResult](DocumentPluginResult.md)
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) [document](#document)
The processed document.

## Constructor Summary
 Constructors
Constructor

Description
 [DocumentPluginResultImpl](#%3Cinit%3E())()
Creates an PluginResult with no document.
  [DocumentPluginResultImpl](#%3Cinit%3E(javax.swing.text.Document))([Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) document)
Constructor for the PluginResult.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) [getProcessedDocument](#getProcessedDocument())()
Get the current document.
  void [setProcessedDocument](#setProcessedDocument(javax.swing.text.Document))([Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) document)
Sets the current document.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### document

protected [Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) document

The processed document.

## Constructor Details

### DocumentPluginResultImpl

public DocumentPluginResultImpl()

Creates an PluginResult with no document.

### DocumentPluginResultImpl

public DocumentPluginResultImpl([Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) document)

Constructor for the PluginResult.
  Parameters: document - The processed document.
## Method Details

### setProcessedDocument

public void setProcessedDocument([Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) document)

Sets the current document.
  Parameters: document - The current document.
### getProcessedDocument

public [Document](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Document.html) getProcessedDocument()

Get the current document.
  Specified by: [getProcessedDocument](DocumentPluginResult.md#getProcessedDocument()) in interface [DocumentPluginResult](DocumentPluginResult.md) Returns: The current document.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
