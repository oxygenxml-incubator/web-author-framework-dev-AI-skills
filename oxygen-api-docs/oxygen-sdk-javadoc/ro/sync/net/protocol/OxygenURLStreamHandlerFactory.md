Package [ro.sync.net.protocol](package-summary.md)

# Class OxygenURLStreamHandlerFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.net.protocol.OxygenURLStreamHandlerFactory
   All Implemented Interfaces: [URLStreamHandlerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandlerFactory.html)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class OxygenURLStreamHandlerFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [URLStreamHandlerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandlerFactory.html)
The URLStreamHandlerFactory that handles all the protocols supported by Oxygen. It handles both builtin protocols and plugin-contributed ones.

## Constructor Summary
 Constructors
Constructor

Description
 [OxygenURLStreamHandlerFactory](#%3Cinit%3E())()
Constructor.
  [OxygenURLStreamHandlerFactory](#%3Cinit%3E(java.net.URLStreamHandlerFactory))([URLStreamHandlerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandlerFactory.html) extraFactory)
An extra factory which can be used to resolve extra protocols.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) [createURLStreamHandler](#createURLStreamHandler(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)

 static [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getBuiltinProtocols](#getBuiltinProtocols())()
Returns the list of built-in protocol names.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OxygenURLStreamHandlerFactory

public OxygenURLStreamHandlerFactory()

Constructor.

### OxygenURLStreamHandlerFactory

public OxygenURLStreamHandlerFactory([URLStreamHandlerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandlerFactory.html) extraFactory)

An extra factory which can be used to resolve extra protocols.
  Parameters: extraFactory - An extra factory which can be used to resolve extra protocols.
## Method Details

### getBuiltinProtocols

public static [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getBuiltinProtocols()

Returns the list of built-in protocol names.
  Returns: The list of built-in protocol names.
### createURLStreamHandler

public [URLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandler.html) createURLStreamHandler([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)
  Specified by: [createURLStreamHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandlerFactory.html#createURLStreamHandler(java.lang.String)) in interface [URLStreamHandlerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandlerFactory.html) See Also:
        * [URLStreamHandlerFactory.createURLStreamHandler(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLStreamHandlerFactory.html#createURLStreamHandler(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
