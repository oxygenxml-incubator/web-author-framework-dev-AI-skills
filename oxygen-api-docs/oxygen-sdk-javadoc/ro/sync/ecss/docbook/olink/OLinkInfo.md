Package [ro.sync.ecss.docbook.olink](package-summary.md)

# Class OLinkInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.docbook.olink.OLinkInfo
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class OLinkInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
OLink information.

## Constructor Summary
 Constructors
Constructor

Description
 [OLinkInfo](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetDoc, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetPtr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xrefText)
The OLink Information
  [OLinkInfo](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetDoc, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetPtr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xrefText, boolean insertXreftext)
The OLink Information

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTargetDoc](#getTargetDoc())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTargetPtr](#getTargetPtr())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXrefText](#getXrefText())()

 boolean [isInsertXreftext](#isInsertXreftext())()

 void [setTargetDoc](#setTargetDoc(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetDoc)

 void [setTargetPtr](#setTargetPtr(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetPtr)

 void [setXrefText](#setXrefText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xrefText)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OLinkInfo

public OLinkInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetDoc, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetPtr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xrefText)

The OLink Information
  Parameters: targetDoc - The target document. targetPtr - The target pointer. xrefText - The XREF text.
### OLinkInfo

public OLinkInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetDoc, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetPtr, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xrefText, boolean insertXreftext)

The OLink Information
  Parameters: targetDoc - The target document. targetPtr - The target pointer. xrefText - The XREF text. insertXreftext - true if the xreftext should be inserted.
## Method Details

### getTargetDoc

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTargetDoc()
  Returns: Returns the targetDoc.
### setTargetDoc

public void setTargetDoc([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetDoc)
  Parameters: targetDoc - The targetDoc to set.
### getTargetPtr

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTargetPtr()
  Returns: Returns the targetPtr.
### isInsertXreftext

public boolean isInsertXreftext()
  Returns: true if should insert xreftext.
### setTargetPtr

public void setTargetPtr([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) targetPtr)
  Parameters: targetPtr - The targetPtr to set.
### getXrefText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXrefText()
  Returns: Returns the xrefText. Might be null.
### setXrefText

public void setXrefText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xrefText)
  Parameters: xrefText - The xrefText to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
