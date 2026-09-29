Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Class FilterURLConnection

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.net.URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html)
        * ro.sync.ecss.extensions.api.webapp.plugin.FilterURLConnection
   All Implemented Interfaces: [FileBrowsingConnection](../../../../../net/protocol/FileBrowsingConnection.md)   @API(src=PUBLIC, type=EXTENDABLE) public class FilterURLConnection extends [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html)implements [FileBrowsingConnection](../../../../../net/protocol/FileBrowsingConnection.md)
URLConnection that delegates all methods to the connection given as a parameter.
  Since: 17
## Field Summary
 Fields
Modifier and Type

Field

Description
 protected [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) [delegateConnection](#delegateConnection)
The underlying connection.

### Fields inherited from class java.net.[URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html)
 [allowUserInteraction](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#allowUserInteraction), [connected](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#connected), [doInput](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#doInput), [doOutput](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#doOutput), [ifModifiedSince](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#ifModifiedSince), [url](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#url), [useCaches](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#useCaches)
## Constructor Summary
 Constructors
Constructor

Description
 [FilterURLConnection](#%3Cinit%3E(java.net.URLConnection))([URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) delegateConnection)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addRequestProperty](#addRequestProperty(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

 void [connect](#connect())()

 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 boolean [getAllowUserInteraction](#getAllowUserInteraction())()

 int [getConnectTimeout](#getConnectTimeout())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getContent](#getContent())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getContent](#getContent(java.lang.Class%5B%5D))([Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html)[] classes)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentEncoding](#getContentEncoding())()

 int [getContentLength](#getContentLength())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentType](#getContentType())()

 long [getDate](#getDate())()

 boolean [getDefaultUseCaches](#getDefaultUseCaches())()

 boolean [getDoInput](#getDoInput())()

 boolean [getDoOutput](#getDoOutput())()

 long [getExpiration](#getExpiration())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHeaderField](#getHeaderField(int))(int n)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHeaderField](#getHeaderField(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

 long [getHeaderFieldDate](#getHeaderFieldDate(java.lang.String,long))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, long Default)

 int [getHeaderFieldInt](#getHeaderFieldInt(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int Default)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHeaderFieldKey](#getHeaderFieldKey(int))(int n)

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> [getHeaderFields](#getHeaderFields())()

 long [getIfModifiedSince](#getIfModifiedSince())()

 [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [getInputStream](#getInputStream())()

 long [getLastModified](#getLastModified())()

 [OutputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/OutputStream.html) [getOutputStream](#getOutputStream())()

 [Permission](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/security/Permission.html) [getPermission](#getPermission())()

 int [getReadTimeout](#getReadTimeout())()

 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> [getRequestProperties](#getRequestProperties())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRequestProperty](#getRequestProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getURL](#getURL())()

 boolean [getUseCaches](#getUseCaches())()

 int [hashCode](#hashCode())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[FolderEntryDescriptor](../../../../../net/protocol/FolderEntryDescriptor.md)> [listFolder](#listFolder())()
Retrieves all children of the directory identified by the URL on which this connection is made.
  void [setAllowUserInteraction](#setAllowUserInteraction(boolean))(boolean allowuserinteraction)

 void [setConnectTimeout](#setConnectTimeout(int))(int timeout)

 void [setDefaultUseCaches](#setDefaultUseCaches(boolean))(boolean defaultusecaches)

 void [setDoInput](#setDoInput(boolean))(boolean doinput)

 void [setDoOutput](#setDoOutput(boolean))(boolean dooutput)

 void [setIfModifiedSince](#setIfModifiedSince(long))(long ifmodifiedsince)

 void [setReadTimeout](#setReadTimeout(int))(int timeout)

 void [setRequestProperty](#setRequestProperty(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

 void [setUseCaches](#setUseCaches(boolean))(boolean usecaches)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.net.[URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html)
 [getContentLengthLong](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContentLengthLong()), [getDefaultAllowUserInteraction](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDefaultAllowUserInteraction()), [getDefaultRequestProperty](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDefaultRequestProperty(java.lang.String)), [getDefaultUseCaches](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDefaultUseCaches(java.lang.String)), [getFileNameMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getFileNameMap()), [getHeaderFieldLong](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFieldLong(java.lang.String,long)), [guessContentTypeFromName](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#guessContentTypeFromName(java.lang.String)), [guessContentTypeFromStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#guessContentTypeFromStream(java.io.InputStream)), [setContentHandlerFactory](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setContentHandlerFactory(java.net.ContentHandlerFactory)), [setDefaultAllowUserInteraction](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDefaultAllowUserInteraction(boolean)), [setDefaultRequestProperty](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDefaultRequestProperty(java.lang.String,java.lang.String)), [setDefaultUseCaches](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDefaultUseCaches(java.lang.String,boolean)), [setFileNameMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setFileNameMap(java.net.FileNameMap))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### delegateConnection

protected [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) delegateConnection

The underlying connection.

## Constructor Details

### FilterURLConnection

public FilterURLConnection([URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) delegateConnection)

Constructor.
  Parameters: delegateConnection - The underlying connection.
## Method Details

### getInputStream

public [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) getInputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Overrides: [getInputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getInputStream()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLConnection.getInputStream()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getInputStream())

### getOutputStream

public [OutputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/OutputStream.html) getOutputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Overrides: [getOutputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getOutputStream()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLConnection.getOutputStream()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getOutputStream())

### connect

public void connect() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Specified by: [connect](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#connect()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLConnection.connect()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#connect())

### addRequestProperty

public void addRequestProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
  Overrides: [addRequestProperty](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#addRequestProperty(java.lang.String,java.lang.String)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.addRequestProperty(java.lang.String, java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#addRequestProperty(java.lang.String,java.lang.String))

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### getAllowUserInteraction

public boolean getAllowUserInteraction()
  Overrides: [getAllowUserInteraction](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getAllowUserInteraction()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getAllowUserInteraction()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getAllowUserInteraction())

### getConnectTimeout

public int getConnectTimeout()
  Overrides: [getConnectTimeout](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getConnectTimeout()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getConnectTimeout()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getConnectTimeout())

### getContent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getContent() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Overrides: [getContent](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContent()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLConnection.getContent()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContent())

### getContent

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getContent([Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html)[] classes)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Overrides: [getContent](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContent(java.lang.Class%5B%5D)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLConnection.getContent(java.lang.Class[])](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContent(java.lang.Class%5B%5D))

### getContentEncoding

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentEncoding()
  Overrides: [getContentEncoding](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContentEncoding()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getContentEncoding()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContentEncoding())

### getContentLength

public int getContentLength()
  Overrides: [getContentLength](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContentLength()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getContentLength()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContentLength())

### getContentType

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentType()
  Overrides: [getContentType](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContentType()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getContentType()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getContentType())

### getDate

public long getDate()
  Overrides: [getDate](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDate()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getDate()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDate())

### getDefaultUseCaches

public boolean getDefaultUseCaches()
  Overrides: [getDefaultUseCaches](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDefaultUseCaches()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getDefaultUseCaches()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDefaultUseCaches())

### getDoInput

public boolean getDoInput()
  Overrides: [getDoInput](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDoInput()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getDoInput()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDoInput())

### getDoOutput

public boolean getDoOutput()
  Overrides: [getDoOutput](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDoOutput()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getDoOutput()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getDoOutput())

### getExpiration

public long getExpiration()
  Overrides: [getExpiration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getExpiration()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getExpiration()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getExpiration())

### getHeaderField

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHeaderField(int n)
  Overrides: [getHeaderField](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderField(int)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getHeaderField(int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderField(int))

### getHeaderField

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHeaderField([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
  Overrides: [getHeaderField](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderField(java.lang.String)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getHeaderField(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderField(java.lang.String))

### getHeaderFieldDate

public long getHeaderFieldDate([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, long Default)
  Overrides: [getHeaderFieldDate](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFieldDate(java.lang.String,long)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getHeaderFieldDate(java.lang.String, long)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFieldDate(java.lang.String,long))

### getHeaderFieldInt

public int getHeaderFieldInt([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int Default)
  Overrides: [getHeaderFieldInt](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFieldInt(java.lang.String,int)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getHeaderFieldInt(java.lang.String, int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFieldInt(java.lang.String,int))

### getHeaderFieldKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHeaderFieldKey(int n)
  Overrides: [getHeaderFieldKey](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFieldKey(int)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getHeaderFieldKey(int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFieldKey(int))

### getHeaderFields

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> getHeaderFields()
  Overrides: [getHeaderFields](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFields()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getHeaderFields()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getHeaderFields())

### getIfModifiedSince

public long getIfModifiedSince()
  Overrides: [getIfModifiedSince](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getIfModifiedSince()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getIfModifiedSince()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getIfModifiedSince())

### getLastModified

public long getLastModified()
  Overrides: [getLastModified](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getLastModified()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getLastModified()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getLastModified())

### getPermission

public [Permission](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/security/Permission.html) getPermission() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Overrides: [getPermission](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getPermission()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) See Also:
        * [URLConnection.getPermission()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getPermission())

### getReadTimeout

public int getReadTimeout()
  Overrides: [getReadTimeout](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getReadTimeout()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getReadTimeout()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getReadTimeout())

### getRequestProperties

public [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> getRequestProperties()
  Overrides: [getRequestProperties](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getRequestProperties()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getRequestProperties()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getRequestProperties())

### getRequestProperty

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRequestProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
  Overrides: [getRequestProperty](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getRequestProperty(java.lang.String)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getRequestProperty(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getRequestProperty(java.lang.String))

### getURL

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getURL()
  Overrides: [getURL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getURL()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getURL()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getURL())

### getUseCaches

public boolean getUseCaches()
  Overrides: [getUseCaches](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getUseCaches()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.getUseCaches()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#getUseCaches())

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### setAllowUserInteraction

public void setAllowUserInteraction(boolean allowuserinteraction)
  Overrides: [setAllowUserInteraction](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setAllowUserInteraction(boolean)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setAllowUserInteraction(boolean)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setAllowUserInteraction(boolean))

### setConnectTimeout

public void setConnectTimeout(int timeout)
  Overrides: [setConnectTimeout](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setConnectTimeout(int)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setConnectTimeout(int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setConnectTimeout(int))

### setDefaultUseCaches

public void setDefaultUseCaches(boolean defaultusecaches)
  Overrides: [setDefaultUseCaches](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDefaultUseCaches(boolean)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setDefaultUseCaches(boolean)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDefaultUseCaches(boolean))

### setDoInput

public void setDoInput(boolean doinput)
  Overrides: [setDoInput](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDoInput(boolean)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setDoInput(boolean)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDoInput(boolean))

### setDoOutput

public void setDoOutput(boolean dooutput)
  Overrides: [setDoOutput](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDoOutput(boolean)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setDoOutput(boolean)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setDoOutput(boolean))

### setIfModifiedSince

public void setIfModifiedSince(long ifmodifiedsince)
  Overrides: [setIfModifiedSince](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setIfModifiedSince(long)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setIfModifiedSince(long)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setIfModifiedSince(long))

### setReadTimeout

public void setReadTimeout(int timeout)
  Overrides: [setReadTimeout](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setReadTimeout(int)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setReadTimeout(int)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setReadTimeout(int))

### setRequestProperty

public void setRequestProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
  Overrides: [setRequestProperty](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setRequestProperty(java.lang.String,java.lang.String)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setRequestProperty(java.lang.String, java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setRequestProperty(java.lang.String,java.lang.String))

### setUseCaches

public void setUseCaches(boolean usecaches)
  Overrides: [setUseCaches](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setUseCaches(boolean)) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.setUseCaches(boolean)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#setUseCaches(boolean))

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#toString()) in class [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) See Also:
        * [URLConnection.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html#toString())

### listFolder

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[FolderEntryDescriptor](../../../../../net/protocol/FolderEntryDescriptor.md)> listFolder() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Description copied from interface: [FileBrowsingConnection](../../../../../net/protocol/FileBrowsingConnection.md#listFolder())
Retrieves all children of the directory identified by the URL on which this connection is made.
  Specified by: [listFolder](../../../../../net/protocol/FileBrowsingConnection.md#listFolder()) in interface [FileBrowsingConnection](../../../../../net/protocol/FileBrowsingConnection.md) Returns: For list of descriptors for each folder entry. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If the remote server could not return a list of children. [UserActionRequiredException](UserActionRequiredException.md) - Whether the browsing requires user interaction, like login. See Also:
        * [FileBrowsingConnection.listFolder()](../../../../../net/protocol/FileBrowsingConnection.md#listFolder())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
