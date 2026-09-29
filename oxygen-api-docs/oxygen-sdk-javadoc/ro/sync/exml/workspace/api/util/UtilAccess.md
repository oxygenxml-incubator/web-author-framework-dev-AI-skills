Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface UtilAccess
    All Known Subinterfaces: [AuthorUtilAccess](../../../../ecss/extensions/api/access/AuthorUtilAccess.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface UtilAccess
Provides access to utility methods.
  Since: 11.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addCustomEditorVariablesResolver](#addCustomEditorVariablesResolver(ro.sync.exml.workspace.api.util.EditorVariablesResolver))([EditorVariablesResolver](EditorVariablesResolver.md) resolver)
Add a custom editor variables resolver.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [convertFileToURL](#convertFileToURL(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) file)
Converts the given file to an URL by converting not allowed characters to their escaped representation.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [correctURL](#correctURL(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Corrects the given URL by converting not allowed characters to their escaped representation.
  [BufferedImage](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/BufferedImage.html) [createImage](#createImage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imageUrl)
Create the image described by the URL.
  [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) [createReader](#createReader(java.net.URL,java.lang.String))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultEncoding)
Opens a connection for the given URL, examines its contents and decides what kind of encoding should be used.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [decrypt](#decrypt(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toDecrypt)
Decrypts a string using the Oxygen internal encryption system.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [encrypt](#encrypt(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEncrypt)
Encrypts a string using the Oxygen internal encryption system.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandEditorVariables](#expandEditorVariables(java.lang.String,java.net.URL))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pathWithEditorVariables, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditedURL)
Try to expand the editor variables in a path.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [expandEditorVariables](#expandEditorVariables(java.lang.String,java.net.URL,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pathWithEditorVariables, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditedURL, boolean expandAskEditorVariables)
Try to expand the editor variables in a path.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContentType](#getContentType(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)
Get the content type for the given URL.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getExtension](#getExtension(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Get the file extension for this URL.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFileName](#getFileName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) urlPath)
Get the file name from a file or URL path
  boolean [isSupportedImageURL](#isSupportedImageURL(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Check if this URL points to a supported image.
  boolean [isUnhandledBinaryResourceURL](#isUnhandledBinaryResourceURL(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Check if this URL points to a binary resource which is not handled by Oxygen in any way.
  [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [locateFile](#locateFile(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Locate the file on disk corresponding to the URL.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeRelative](#makeRelative(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) childURL)
Make the child URL relative to the base URL.
  [ImageHolder](ImageHolder.md) [optimizeImage](#optimizeImage(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) imageUrl)
Optimize an image to be consumed by a web browser.
  void [removeCustomEditorVariablesResolver](#removeCustomEditorVariablesResolver(ro.sync.exml.workspace.api.util.EditorVariablesResolver))([EditorVariablesResolver](EditorVariablesResolver.md) resolver)
Remove a custom editor variables resolver.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [removeUserCredentials](#removeUserCredentials(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Removes the user name and password from the URL if they are present.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [uncorrectURL](#uncorrectURL(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Un-corrects the given URL by converting the percent encoded characters back to the original characters.

## Method Details

### makeRelative

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeRelative([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) childURL)

Make the child URL relative to the base URL. The query and fragment identifier are preserved if the initial reference contains them.
The child URL is relatively expressed to the base URL. If it is not possible, the child URL is returned.

For example if the base URL is "file://c:/projects/exml/base.prx" and the child URL is "file://c:/projects/exml/test/someTest.xml" the result will be: "test/someTest.xml"

  Parameters: baseURL - The base URL. childURL - The child URL. Returns: The relative path or the childURL if a relative path cannot be computed.
### correctURL

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) correctURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Corrects the given URL by converting not allowed characters to their escaped representation. The URL correction takes an URL like:http://path to directory/file.xmland escapes illegal URL characters like spaces to:http://path%20to%20directory/file.xml
  Parameters: url - The URL to be corrected. Returns: The corrected URL. It does not return null.
### uncorrectURL

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) uncorrectURL([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Un-corrects the given URL by converting the percent encoded characters back to the original characters. The URL un-correction takes an URL like:http://path%20to%20directory/file.xmland unescapes it back to:http://path to directory/file.xml
  Parameters: url - The URL to be corrected. Returns: The corrected URL. It does not return null. Since: 20.1
### convertFileToURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) convertFileToURL([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) file)throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Converts the given file to an URL by converting not allowed characters to their escaped representation. The URL correction takes a File like:c:\path to directory\file.xmland escapes illegal URL characters like spaces to:http://path%20to%20directory/file.xml
  Parameters: file - The File to be corrected. Returns: The corrected URL. It does not return null. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - if it fails to perform the conversion. Since: 18
### removeUserCredentials

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) removeUserCredentials([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Removes the user name and password from the URL if they are present.
  Parameters: url - The URL from which the user credentials will be removed. Returns: The URL having the user credentials removed. Since: 12.1
### locateFile

[File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) locateFile([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Locate the file on disk corresponding to the URL.
  Parameters: url - The [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) to be checked. Returns: The corresponding [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) from the local file system or null if the URL is remote.
### getExtension

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getExtension([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Get the file extension for this URL. The extension is lower cased.
  Parameters: url - The URL to extract the extension for. Returns: the file extension for this URL. The extension is lower cased.
### getFileName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFileName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) urlPath)

Get the file name from a file or URL path
  Parameters: urlPath - An URL path Returns: the file name from a file or URL path
### isSupportedImageURL

boolean isSupportedImageURL([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Check if this URL points to a supported image. The image extension is used
  Parameters: url - The URL Returns: true if this URL points to a supported image. The image extension is used
### isUnhandledBinaryResourceURL

boolean isUnhandledBinaryResourceURL([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Check if this URL points to a binary resource which is not handled by Oxygen in any way. The resource file extension is checked against a list of binary file patterns configured in the Oxygen options. For example ZIP-like archives are handled by Oxygen although they are binary.
  Parameters: url - The URL Returns: true if this URL points to a binary resource. Since: 15
### expandEditorVariables

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandEditorVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pathWithEditorVariables, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditedURL)

Try to expand the editor variables in a path. If there's an external framework associated with the current editor, any $framework, $frameworks, $frameworkDir or $frameworksDir variable will be expanded in the context of that framework. "ask" and "answer" editor variables are not expanded by default.
  Parameters: pathWithEditorVariables - The path containing editor variables currentEditedURL - The current edited URL. Can be null but it may be necessary to expand editor variables like "${cfd}". Returns: The path with editor variables expanded. Since: 12.1
### expandEditorVariables

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) expandEditorVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pathWithEditorVariables, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditedURL, boolean expandAskEditorVariables)

Try to expand the editor variables in a path. If there's an external framework associated with the current editor, any $framework, $frameworks, $frameworkDir or $frameworksDir variable will be expanded in the context of that framework.
  Parameters: pathWithEditorVariables - The path containing editor variables currentEditedURL - The current edited URL. Can be null but it may be necessary to expand editor variables like "${cfd}". expandAskEditorVariables - true to also expand "ask" and "answer" editor variables. Returns: The path with editor variables expanded. Will return the original string if there are "ask" editor variables in the content and the end user chose to cancel the prompt dialogs. Since: 22
### encrypt

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) encrypt([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEncrypt)

Encrypts a string using the Oxygen internal encryption system. The encryption/decryption is application-specific so a string encrypted in one Oxygen installation cannot be decrypted in another. You can use this method if you want to store user-specific data on disk with a moderate level of security.
  Parameters: toEncrypt - The string to encrypt. Returns: The string encrypted using the Oxygen internal encryption system. Since: 12.1
### decrypt

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) decrypt([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toDecrypt)

Decrypts a string using the Oxygen internal encryption system. The encryption/decryption is application-specific so a string encrypted in one Oxygen installation cannot be decrypted in another. You can use this method if you want to store user-specific data on disk with a moderate level of security.
  Parameters: toDecrypt - The string to decrypt. Returns: The string decrypted using the Oxygen internal encryption system or NULL if the string format is not understood. Since: 12.1
### addCustomEditorVariablesResolver

void addCustomEditorVariablesResolver([EditorVariablesResolver](EditorVariablesResolver.md) resolver)

Add a custom editor variables resolver. The resolver receives a string which may or may not contain custom editor variables. It can either return the unmodified string or a modified version of the string in which certain editor variables have been expanded to certain values.
  Parameters: resolver - The resolver. Since: 16.1
### removeCustomEditorVariablesResolver

void removeCustomEditorVariablesResolver([EditorVariablesResolver](EditorVariablesResolver.md) resolver)

Remove a custom editor variables resolver.
  Parameters: resolver - The resolver to remove. Since: 16.1
### createReader

[Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) createReader([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultEncoding)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Opens a connection for the given URL, examines its contents and decides what kind of encoding should be used.
  Parameters: url - The URL to be opened. defaultEncoding - The encoding to be used when all other ways of detecting it returned null. This is used instead of creating the input stream reader with no encoding arguments. This is a JAVA encoding. Returns: A reader for the given URL. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - when an error occurs during the URL connection. Since: 17
### createImage

[BufferedImage](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/image/BufferedImage.html) createImage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imageUrl)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Create the image described by the URL.
  Parameters: imageUrl - The URL of the image for which to return the buffered image. Returns: The BufferedImage of the image located at the provided URL. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Unable to create the image. Since: 17.1
### optimizeImage

[ImageHolder](ImageHolder.md) optimizeImage([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) imageUrl)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

Optimize an image to be consumed by a web browser. In case the image is too large it scales it down to fit a normal page.
  Parameters: imageUrl - The image URL. Returns: The holder of the image that can forward it to the browser. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - Unable to create the image. Since: 19.1
### getContentType

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContentType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)

Get the content type for the given URL. The content type is detected from the file extension based on the file extension associations saved in the application preferences.
  Parameters: systemID - The systemID to get the content type for. Returns: the content type string or null if there is no mapping. The content type is returned as a mime type value, for example "text/xml" for XML documents. Can be null if the content type is unknown for the application. Since: 24.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
