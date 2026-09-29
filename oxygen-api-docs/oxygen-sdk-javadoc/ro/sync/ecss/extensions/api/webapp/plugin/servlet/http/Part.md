Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet.http](package-summary.md)

# Interface Part
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Part
Part interface inspired from HTTP Servlet 5.0.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [delete](#delete())()
Deletes the underlying storage for a file item, including deleting any associated temporary disk file.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentType](#getContentType())()
Gets the content type of this part.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHeader](#getHeader(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the value of the specified mime header as a String.
  [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getHeaderNames](#getHeaderNames())()
Gets the header names of this Part.
  [Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getHeaders](#getHeaders(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Gets the values of the Part header with the given name.
  [InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) [getInputStream](#getInputStream())()
Gets the content of this part as an InputStream
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Gets the name of this part
  long [getSize](#getSize())()
Returns the size of this fille.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSubmittedFileName](#getSubmittedFileName())()
Gets the file name specified by the client
  void [write](#write(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileName)
A convenience method to write this uploaded item to disk.

## Method Details

### getInputStream

[InputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/InputStream.html) getInputStream() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Gets the content of this part as an InputStream
  Returns: The content of this part as an InputStream Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If an error occurs in retrieving the content as an InputStream
### getContentType

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentType()

Gets the content type of this part.
  Returns: The content type of this part.
### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Gets the name of this part
  Returns: The name of this part as a String
### getSubmittedFileName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSubmittedFileName()

Gets the file name specified by the client
  Returns: the submitted file name
### getSize

long getSize()

Returns the size of this fille.
  Returns: a long specifying the size of this part, in bytes.
### write

void write([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileName)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

A convenience method to write this uploaded item to disk.
This method is not guaranteed to succeed if called more than once for the same part. This allows a particular implementation to use, for example, file renaming, where possible, rather than copying all of the underlying data, thus gaining a significant performance benefit.

  Parameters: fileName - The location into which the uploaded part should be stored. Relative paths are relative to MultipartConfigElement#getLocation(). Absolute paths are used as provided. Note: that this is a system dependent string and URI notation may not be acceptable on all systems. For portability, this string should be generated with the File or Path APIs. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an error occurs.
### delete

void delete() throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Deletes the underlying storage for a file item, including deleting any associated temporary disk file.
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - if an error occurs.
### getHeader

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHeader([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the value of the specified mime header as a String. If the Part did not include a header of the specified name, this method returns null. If there are multiple headers with the same name, this method returns the first header in the part. The header name is case insensitive. You can use this method with any request header.
  Parameters: name - a String specifying the header name Returns: a String containing the value of the requested header, or null if the part does not have a header of that name
### getHeaders

[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getHeaders([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Gets the values of the Part header with the given name.
Any changes to the returned Collection must not affect this Part.

Part header names are case insensitive.

  Parameters: name - the header name whose values to return Returns: a (possibly empty) Collection of the values of the header with the given name
### getHeaderNames

[Collection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getHeaderNames()

Gets the header names of this Part.
Some servlet containers do not allow servlets to access headers using this method, in which case this method returns null

Any changes to the returned Collection must not affect this Part.

  Returns: a (possibly empty) Collection of the header names of this Part
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
