Package [ro.sync.ecss.extensions.api.access](package-summary.md)

# Interface AuthorUtilAccess
    All Superinterfaces: [UtilAccess](../../../../exml/workspace/api/util/UtilAccess.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorUtilAccessextends [UtilAccess](../../../../exml/workspace/api/util/UtilAccess.md)
Provides access to utility methods related to author access.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [escapeAttributeValue](#escapeAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)  Deprecated.
Use the method from the AuthorXMLUtilAccess class.
   [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newNonValidatingXMLReader](#newNonValidatingXMLReader())()  Deprecated.
Use the method from the AuthorXMLUtilAccess class.
   void [resetXMLCatalogs](#resetXMLCatalogs())()  Deprecated.
Use the method from the AuthorXMLUtilAccess class.
   [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolvePath](#resolvePath(java.net.URL,java.lang.String,boolean,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativeLocation, boolean entityResolve, boolean uriResolve)  Deprecated.
Use the method from the AuthorXMLUtilAccess class.

### Methods inherited from interface ro.sync.exml.workspace.api.util.[UtilAccess](../../../../exml/workspace/api/util/UtilAccess.md)
 [addCustomEditorVariablesResolver](../../../../exml/workspace/api/util/UtilAccess.md#addCustomEditorVariablesResolver(ro.sync.exml.workspace.api.util.EditorVariablesResolver)), [convertFileToURL](../../../../exml/workspace/api/util/UtilAccess.md#convertFileToURL(java.io.File)), [correctURL](../../../../exml/workspace/api/util/UtilAccess.md#correctURL(java.lang.String)), [createImage](../../../../exml/workspace/api/util/UtilAccess.md#createImage(java.lang.String)), [createReader](../../../../exml/workspace/api/util/UtilAccess.md#createReader(java.net.URL,java.lang.String)), [decrypt](../../../../exml/workspace/api/util/UtilAccess.md#decrypt(java.lang.String)), [encrypt](../../../../exml/workspace/api/util/UtilAccess.md#encrypt(java.lang.String)), [expandEditorVariables](../../../../exml/workspace/api/util/UtilAccess.md#expandEditorVariables(java.lang.String,java.net.URL)), [expandEditorVariables](../../../../exml/workspace/api/util/UtilAccess.md#expandEditorVariables(java.lang.String,java.net.URL,boolean)), [getContentType](../../../../exml/workspace/api/util/UtilAccess.md#getContentType(java.lang.String)), [getExtension](../../../../exml/workspace/api/util/UtilAccess.md#getExtension(java.net.URL)), [getFileName](../../../../exml/workspace/api/util/UtilAccess.md#getFileName(java.lang.String)), [isSupportedImageURL](../../../../exml/workspace/api/util/UtilAccess.md#isSupportedImageURL(java.net.URL)), [isUnhandledBinaryResourceURL](../../../../exml/workspace/api/util/UtilAccess.md#isUnhandledBinaryResourceURL(java.net.URL)), [locateFile](../../../../exml/workspace/api/util/UtilAccess.md#locateFile(java.net.URL)), [makeRelative](../../../../exml/workspace/api/util/UtilAccess.md#makeRelative(java.net.URL,java.net.URL)), [optimizeImage](../../../../exml/workspace/api/util/UtilAccess.md#optimizeImage(java.net.URL)), [removeCustomEditorVariablesResolver](../../../../exml/workspace/api/util/UtilAccess.md#removeCustomEditorVariablesResolver(ro.sync.exml.workspace.api.util.EditorVariablesResolver)), [removeUserCredentials](../../../../exml/workspace/api/util/UtilAccess.md#removeUserCredentials(java.net.URL)), [uncorrectURL](../../../../exml/workspace/api/util/UtilAccess.md#uncorrectURL(java.lang.String))
## Method Details

### escapeAttributeValue

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) escapeAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)
 Deprecated.
Use the method from the AuthorXMLUtilAccess class.

Escape an attribute value so that the XML document remains well-formed.
  Parameters: attributeValue - The attribute value. Returns: The escaped value. It does not return null.
### newNonValidatingXMLReader

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newNonValidatingXMLReader()
 Deprecated.
Use the method from the AuthorXMLUtilAccess class.

Creates an [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) without validation.
  Returns: A new XML Reader.
### resolvePath

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolvePath([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativeLocation, boolean entityResolve, boolean uriResolve)
 Deprecated.
Use the method from the AuthorXMLUtilAccess class.

Try to resolve a relative location to an absolute path by using the XML catalogs.
  Parameters: baseURL - The URL of the current opened XML file. relativeLocation - The relative location to be resolved. entityResolve - true if the catalog entity resolver should be used. uriResolve - true if the catalog URI resolver should be used. Returns: The absolute URL. It does not return null.
### resetXMLCatalogs

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) void resetXMLCatalogs()
 Deprecated.
Use the method from the AuthorXMLUtilAccess class.

Reset the loaded XML catalogs. This way next time the catalogs are needed they will first be rebuilt.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
