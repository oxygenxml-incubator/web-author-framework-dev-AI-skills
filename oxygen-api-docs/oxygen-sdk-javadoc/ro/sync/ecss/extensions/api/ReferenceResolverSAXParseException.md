Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class ReferenceResolverSAXParseException

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
        * [java.lang.Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
            * [org.xml.sax.SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
                * [org.xml.sax.SAXParseException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html)
                    * ro.sync.ecss.extensions.api.ReferenceResolverSAXParseException
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(type=EXTENDABLE, src=PUBLIC) public class ReferenceResolverSAXParseException extends [SAXParseException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html)
Exception thrown if the reference resolver could not resolve a target.
  See Also:
* [Serialized Form](../../../../../serialized-form.md#ro.sync.ecss.extensions.api.ReferenceResolverSAXParseException)

## Constructor Summary
 Constructors
Constructor

Description
 [ReferenceResolverSAXParseException](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Constructor.
  [ReferenceResolverSAXParseException](#%3Cinit%3E(java.lang.String,org.xml.sax.Locator))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [Locator](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Locator.html) locator)
Constructor.

## Method Summary

### Methods inherited from class org.xml.sax.[SAXParseException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html)
 [getColumnNumber](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html#getColumnNumber()), [getLineNumber](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html#getLineNumber()), [getPublicId](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html#getPublicId()), [getSystemId](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html#getSystemId()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html#toString())
### Methods inherited from class org.xml.sax.[SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
 [getCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html#getCause()), [getException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html#getException()), [getMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html#getMessage())
### Methods inherited from class java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
 [addSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#addSuppressed(java.lang.Throwable)), [fillInStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#fillInStackTrace()), [getLocalizedMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getLocalizedMessage()), [getStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getStackTrace()), [getSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getSuppressed()), [initCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#initCause(java.lang.Throwable)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace()), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintStream)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintWriter)), [setStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#setStackTrace(java.lang.StackTraceElement%5B%5D))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ReferenceResolverSAXParseException

public ReferenceResolverSAXParseException([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Constructor.
  Parameters: message - The error or warning message.
### ReferenceResolverSAXParseException

public ReferenceResolverSAXParseException([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [Locator](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Locator.html) locator)

Constructor.
  Parameters: message - The error or warning message. locator - The locator object for the error or warning (may be null).
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
