Package [ro.sync.ecss.dita](package-summary.md)

# Class HrefInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.dita.HrefInfo
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class HrefInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Contains the referenced URL + information whether this is a map or a topic
  Since: 18.1
## Constructor Summary
 Constructors
Constructor

Description
 [HrefInfo](#%3Cinit%3E(java.net.URL,java.lang.String,boolean,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, boolean isDITAMap, boolean isDITAReference)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHrefValue](#getHrefValue())()

 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getReferenceURL](#getReferenceURL())()

 boolean [isDITAMap](#isDITAMap())()

 boolean [isDITAReference](#isDITAReference())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### HrefInfo

public HrefInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) referenceURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, boolean isDITAMap, boolean isDITAReference)

Constructor.
  Parameters: referenceURL - The refered URL. hrefValue - The href value isDITAMap - True if DITA Map isDITAReference - true if this is a reference to a DITA resource.
## Method Details

### getReferenceURL

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getReferenceURL()
  Returns: The reference URL. May be null if the href points to an URL with a protocol unsupported by Oxygen. See EXM-49443
### getHrefValue

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHrefValue()
  Returns: The href value
### isDITAMap

public boolean isDITAMap()
  Returns: true if this is a DITA Map
### isDITAReference

public boolean isDITAReference()
  Returns: true if this is a reference to a DITA resource.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
