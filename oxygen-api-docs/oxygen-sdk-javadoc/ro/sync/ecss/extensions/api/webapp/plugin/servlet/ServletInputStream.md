Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet](package-summary.md)

# Class ServletInputStream

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.io.InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html)
        * ro.sync.ecss.extensions.api.webapp.plugin.servlet.ServletInputStream
   All Implemented Interfaces: [Closeable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Closeable.html), [AutoCloseable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/AutoCloseable.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public abstract class ServletInputStream extends [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html)
ServletInputStream interface inspired from HTTP Servlet 5.0.
  Since: 26
## Constructor Summary
 Constructors
Modifier

Constructor

Description
 protected  [ServletInputStream](#%3Cinit%3E())()
Does nothing, because this is an abstract class.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 final int [readLine](#readLine(byte%5B%5D,int,int))(byte[] b, int off, int len)
Reads the input stream, one line at a time.

### Methods inherited from class java.io.[InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html)
 [available](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#available()), [close](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#close()), [mark](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#mark(int)), [markSupported](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#markSupported()), [nullInputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#nullInputStream()), [read](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#read()), [read](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#read(byte%5B%5D)), [read](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#read(byte%5B%5D,int,int)), [readAllBytes](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#readAllBytes()), [readNBytes](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#readNBytes(byte%5B%5D,int,int)), [readNBytes](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#readNBytes(int)), [reset](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#reset()), [skip](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#skip(long)), [skipNBytes](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#skipNBytes(long)), [transferTo](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html#transferTo(java.io.OutputStream))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ServletInputStream

protected ServletInputStream()

Does nothing, because this is an abstract class.

## Method Details

### readLine

public final int readLine(byte[] b, int off, int len)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Reads the input stream, one line at a time. Starting at an offset, reads bytes into an array, until it reads a certain number of bytes or reaches a newline character, which it reads into the array as well.
This method returns -1 if it reaches the end of the input stream before reading the maximum number of bytes.

  Parameters: b - an array of bytes into which data is read off - an integer specifying the character at which this method begins reading len - an integer specifying the maximum number of bytes to read Returns: an integer specifying the actual number of bytes read, or -1 if the end of the stream is reached Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an input or output exception has occurred
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
