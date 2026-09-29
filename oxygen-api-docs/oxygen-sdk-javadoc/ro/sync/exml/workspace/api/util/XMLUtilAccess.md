Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface XMLUtilAccess
    All Known Subinterfaces: [AuthorXMLUtilAccess](../../../../ecss/extensions/api/access/AuthorXMLUtilAccess.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface XMLUtilAccess
XML Utilities
  Since: 11.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EXTENSION_NS](#EXTENSION_NS)
Namespace for XPath extension functions.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EXTENSION_PREFIX](#EXTENSION_PREFIX)
Predefined prefix for XPath extension function.
  static final int [TRANSFORMER_SAXON_6](#TRANSFORMER_SAXON_6)
Saxon 6 transformer
  static final int [TRANSFORMER_SAXON_ENTERPRISE_EDITION](#TRANSFORMER_SAXON_ENTERPRISE_EDITION)  Deprecated.
Since Oxygen 23 you can no longer create Saxon 9 PE transformers using this constant.
   static final int [TRANSFORMER_SAXON_HOME_EDITION](#TRANSFORMER_SAXON_HOME_EDITION)
Saxon 9 Home Edition transformer type (no extensions support).
  static final int [TRANSFORMER_SAXON_PROFESSIONAL_EDITION](#TRANSFORMER_SAXON_PROFESSIONAL_EDITION)  Deprecated.
Since Oxygen 23 you can no longer create Saxon 9 PE transformers using this constant.
   static final int [TRANSFORMER_XALAN](#TRANSFORMER_XALAN)
Xalan transformer

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [addPriorityEntityResolver](#addPriorityEntityResolver(org.xml.sax.EntityResolver))([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Add a priority entity resolver.
  void [addPriorityURIResolver](#addPriorityURIResolver(javax.xml.transform.URIResolver))([URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver)
Add a priority URI resolver.
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createSaxon9HEXSLTTransformerWithExtensions](#createSaxon9HEXSLTTransformerWithExtensions(javax.xml.transform.Source,net.sf.saxon.lib.ExtensionFunctionDefinition%5B%5D))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, net.sf.saxon.lib.ExtensionFunctionDefinition[] saxonExtensions)
Create a Saxon 9 Home Edition transformer with the specified extension functions.
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createSaxon9XSLTTransformerWithExtensions](#createSaxon9XSLTTransformerWithExtensions(javax.xml.transform.Source,net.sf.saxon.lib.ExtensionFunctionDefinition%5B%5D,int))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, net.sf.saxon.lib.ExtensionFunctionDefinition[] extensionFunctions, int transformerType)
Create a Saxon 9 Home Edition transformer with the specified extension functions.
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createXQueryTransformer](#createXQueryTransformer(javax.xml.transform.Source,java.net.URL%5B%5D,int))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) xquerySource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType)
Create a new XQuery transformer.
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createXQueryTransformer](#createXQueryTransformer(javax.xml.transform.Source,java.net.URL%5B%5D,int,boolean))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) xquerySource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType, boolean useOxygenOptions)
Create a new XQuery transformer.
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createXSLTTransformer](#createXSLTTransformer(javax.xml.transform.Source,java.net.URL%5B%5D,int))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType)
Create a new XSLT transformer.
  [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createXSLTTransformer](#createXSLTTransformer(javax.xml.transform.Source,java.net.URL%5B%5D,int,boolean))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType, boolean useOxygenOptions)
Create a new XSLT transformer.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [escapeAttributeValue](#escapeAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)
Escape an attribute value so that the XML document remains well-formed.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [escapeTextValue](#escapeTextValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textValue)
Escape text which will be inserted in the XML so that the XML document remains well-formed.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getAssociatedTransformationScenarioInputURL](#getAssociatedTransformationScenarioInputURL(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) xsltOrXQueryLocation)
If the given URL is for an XQuery or XSL content type, it will try to detect the XML/JSON source from the associated scenario.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getAssociatedValidationScenarioInputURL](#getAssociatedValidationScenarioInputURL(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaLocation)
If the given URL is for a schema (XSD, RNG, DTD), it will try to detect the XML/JSON source from the associated validation scenario.
  [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) [getEntityResolver](#getEntityResolver())()
Get the same entity resolver Oxygen sets to its constructed SAX Parsers (which looks into the Oxygen options and document types for catalogs).
  [URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) [getURIResolver](#getURIResolver())()
Get the same URI resolver Oxygen sets to its constructed XSLT transformers (which looks into the Oxygen options and document types for catalogs).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXMLStructureAsDTD](#getXMLStructureAsDTD(java.io.Reader))([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Get the structure of the provided XML document as a DTD.
  [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newNonValidatingXMLReader](#newNonValidatingXMLReader())()
Creates an [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) without validation.
  [XMLReaderWithGrammar](XMLReaderWithGrammar.md) [newNonValidatingXMLReader](#newNonValidatingXMLReader(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCacheToken)
Creates an [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) without validation and with the possibility to reuse the grammar pool.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [prettyPrint](#prettyPrint(java.io.Reader,java.lang.String))([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)
Pretty prints the given XML document.
  void [removePriorityEntityResolver](#removePriorityEntityResolver(org.xml.sax.EntityResolver))([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Remove a priority entity resolver.
  void [removePriorityURIResolver](#removePriorityURIResolver(javax.xml.transform.URIResolver))([URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver)
Remove a priority URI resolver.
  void [resetXMLCatalogs](#resetXMLCatalogs())()
Reset the loaded XML catalogs.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolvePathThroughCatalogs](#resolvePathThroughCatalogs(java.net.URL,java.lang.String,boolean,boolean))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativeLocation, boolean entityResolve, boolean uriResolve)
Try to resolve a relative location to an absolute path by using the XML catalogs.
  [MergeResult](../../../../merge/MergeResult.md) [threeWayAutoMerge](#threeWayAutoMerge(java.lang.String,java.lang.String,java.lang.String,ro.sync.merge.MergeConflictResolutionMethods))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ancestor, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) left, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) right, [MergeConflictResolutionMethods](../../../../merge/MergeConflictResolutionMethods.md) conflictResolutionMethod)  Deprecated.
since 19.1, please use the equivalent [CompareUtilAccess](CompareUtilAccess.md) utilities.
   [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [unescapeAttributeValue](#unescapeAttributeValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)
Unescape an attribute value.

## Field Details

### TRANSFORMER_XALAN

static final int TRANSFORMER_XALAN

Xalan transformer
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.util.XMLUtilAccess.TRANSFORMER_XALAN)

### TRANSFORMER_SAXON_6

static final int TRANSFORMER_SAXON_6

Saxon 6 transformer
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.util.XMLUtilAccess.TRANSFORMER_SAXON_6)

### TRANSFORMER_SAXON_HOME_EDITION

static final int TRANSFORMER_SAXON_HOME_EDITION

Saxon 9 Home Edition transformer type (no extensions support).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.util.XMLUtilAccess.TRANSFORMER_SAXON_HOME_EDITION)

### TRANSFORMER_SAXON_PROFESSIONAL_EDITION

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) static final int TRANSFORMER_SAXON_PROFESSIONAL_EDITION
 Deprecated.
Since Oxygen 23 you can no longer create Saxon 9 PE transformers using this constant. The created transformer will be a Saxon HE transformer instead.

Saxon 9 Professional Edition transformer type (full extensions support).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.util.XMLUtilAccess.TRANSFORMER_SAXON_PROFESSIONAL_EDITION)

### TRANSFORMER_SAXON_ENTERPRISE_EDITION

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) static final int TRANSFORMER_SAXON_ENTERPRISE_EDITION
 Deprecated.
Since Oxygen 23 you can no longer create Saxon 9 PE transformers using this constant. The created transformer will be a Saxon HE transformer instead.

Saxon 9 Enterprise Edition transformer type (full extensions support + schema aware).
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.util.XMLUtilAccess.TRANSFORMER_SAXON_ENTERPRISE_EDITION)

### EXTENSION_PREFIX

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EXTENSION_PREFIX

Predefined prefix for XPath extension function.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.util.XMLUtilAccess.EXTENSION_PREFIX)

### EXTENSION_NS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EXTENSION_NS

Namespace for XPath extension functions.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.util.XMLUtilAccess.EXTENSION_NS)

## Method Details

### createXSLTTransformer

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createXSLTTransformer([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Create a new XSLT transformer. The options set in the oXygen preferences are used.
  Parameters: styleSource - The source XSL extensionJars - Jars with extension libraries which can be used by the transformer, can be null transformerType - The type of the transformer to create, one of the constants defined in this class starting with TRANSFORMER_ Returns: The new transformer. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) - An Exceptionis thrown if an error occurs during parsing of the source.
### createSaxon9XSLTTransformerWithExtensions

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createSaxon9XSLTTransformerWithExtensions([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, net.sf.saxon.lib.ExtensionFunctionDefinition[] extensionFunctions, int transformerType)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Create a Saxon 9 Home Edition transformer with the specified extension functions.
  Parameters: styleSource - The source XSL extensionFunctions - Jars with extension libraries which can be used by the transformer, can be null transformerType - The type of the transformer to create can only be TRANSFORMER_SAXON_HOME_EDITION. Returns: The new transformer. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) - An Exceptionis thrown if an error occurs during parsing of the source.
### createXSLTTransformer

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createXSLTTransformer([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType, boolean useOxygenOptions)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Create a new XSLT transformer.
  Parameters: styleSource - The source XSL extensionJars - Jars with extension libraries which can be used by the transformer. Can be null. transformerType - The type of the transformer to create, one of the constants defined in this class starting with TRANSFORMER_ useOxygenOptions - If true the options set in the oXygen preferences are used. Otherwise no options are set to the transformers. Returns: The new transformer. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) - An Exception is thrown if an error occurs during parsing of the source. Since: 12.2
### createSaxon9HEXSLTTransformerWithExtensions

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createSaxon9HEXSLTTransformerWithExtensions([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) styleSource, net.sf.saxon.lib.ExtensionFunctionDefinition[] saxonExtensions)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Create a Saxon 9 Home Edition transformer with the specified extension functions. This is necessary when the extension functions cannot be called by reflection because there is no license for the commercial version of Saxon 9.

The Saxon 9 options set in the oXygen preferences are not used.
  Parameters: styleSource - The source XSL saxonExtensions - The list of Saxon 9 extensions. Returns: The new transformer. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) - An Exception is thrown if an error occurs during parsing of the source. Since: 12.2
### createXQueryTransformer

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createXQueryTransformer([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) xquerySource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Create a new XQuery transformer. The options set in the oXygen preferences are used.
  Parameters: xquerySource - The source XQuery file extensionJars - Jars with extension libraries which can be used by the transformer, can be null transformerType - The type of the transformer to create, can only be [TRANSFORMER_SAXON_HOME_EDITION](#TRANSFORMER_SAXON_HOME_EDITION) Returns: The new transformer. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) - An Exception is thrown if an error occurs during parsing of the source.
### createXQueryTransformer

[Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createXQueryTransformer([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) xquerySource, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] extensionJars, int transformerType, boolean useOxygenOptions)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Create a new XQuery transformer.
  Parameters: xquerySource - The source XQuery file extensionJars - Jars with extension libraries which can be used by the transformer. Can be null. transformerType - The type of the transformer to create, can only be [TRANSFORMER_SAXON_HOME_EDITION](#TRANSFORMER_SAXON_HOME_EDITION) useOxygenOptions - If true the options set in the oXygen preferences are used. Otherwise no options are set to the transformers. Returns: The new transformer. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) - An Exception is thrown if an error occurs during parsing of the source. Since: 12.2
### resetXMLCatalogs

void resetXMLCatalogs()

Reset the loaded XML catalogs. This way next time the catalogs are needed they will first be rebuilt.

### resolvePathThroughCatalogs

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolvePathThroughCatalogs([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) baseURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) relativeLocation, boolean entityResolve, boolean uriResolve)

Try to resolve a relative location to an absolute path by using the XML catalogs.
  Parameters: baseURL - The URL of the current opened XML file. relativeLocation - The relative location to be resolved. entityResolve - true if the catalog entity resolver should be used. uriResolve - true if the catalog URI resolver should be used. Returns: The absolute URL. It returns null only for URLs with unknown protocols for which an URL object cannot be constructed.
### escapeAttributeValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) escapeAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)

Escape an attribute value so that the XML document remains well-formed.
  Parameters: attributeValue - The attribute value. Returns: The escaped value. It does not return null.
### escapeTextValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) escapeTextValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) textValue)

Escape text which will be inserted in the XML so that the XML document remains well-formed.
  Parameters: textValue - The text value. Returns: The escaped value. It does not return null. Since: 18
### unescapeAttributeValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) unescapeAttributeValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue)

Unescape an attribute value.
  Parameters: attributeValue - The attribute value to be unescaped. Returns: The unescaped value. It does not return null. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - when having problems with unescaping hex or decimal characters from the method's argument. Since: 17.1
### prettyPrint

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) prettyPrint([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)throws [PrettyPrintException](PrettyPrintException.md)

Pretty prints the given XML document. The oXygen pretty printing options are used.
  Parameters: reader - The reader with over the document that is to be pretty printed. systemID - The URL location where the current XML fragment to format and indent is located. This parameter is not required but it may be used to solves relative entities from the DOCTYPE declaration in the XML content. Returns: The pretty printed version of the XML document. Throws: [PrettyPrintException](PrettyPrintException.md) - If the pretty printing failed. Since: 17.1
### newNonValidatingXMLReader

[XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newNonValidatingXMLReader()

Creates an [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) without validation.
  Returns: A new XML Reader.
### newNonValidatingXMLReader

[XMLReaderWithGrammar](XMLReaderWithGrammar.md) newNonValidatingXMLReader([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) grammarCacheToken)

Creates an [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) without validation and with the possibility to reuse the grammar pool. If you are parsing XML fragments with DOCTYPE many times in your operation this method will be faster than the newNonValidatingXMLReader() method.  *Usage example:*
```
 String xml = new String("<!DOCTYPE map PUBLIC \"-//OASIS//DTD DITA Map//EN\" \"map.dtd\">\n" +
     "<map/>");
 Object grammarToken = null;
 for (int i = 0; i < 100000; i++) {
   XMLReaderWithGrammar readerAndCache = authorAccess.getXMLUtilAccess().newNonValidatingXMLReader(grammarToken);
   XMLReader reader = readerAndCache.getXmlReader();
   grammarToken = readerAndCache.getGrammarCache();
   reader.parse(new InputSource(new StringReader(xml)));
 }

```

  Parameters: grammarCacheToken - The grammar cache token, if not null, it will be used to cache the grammar pool. Returns: A new XML Reader with a grammar cache token which can be then reused on the same method to provide grammar caching.
### getEntityResolver

[EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) getEntityResolver()

Get the same entity resolver Oxygen sets to its constructed SAX Parsers (which looks into the Oxygen options and document types for catalogs). The resolver also looks at the additionally set priority entity resolvers.
  Returns: the same entity resolver Oxygen sets to its constructed SAX Parsers (which looks into the Oxygen options and document types for catalogs). Since: 12.1
### getURIResolver

[URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) getURIResolver()

Get the same URI resolver Oxygen sets to its constructed XSLT transformers (which looks into the Oxygen options and document types for catalogs). The resolver also looks at the additionally set priority URI resolvers.
  Returns: the same URI resolver Oxygen sets to its constructed XSLT transformers (which looks into the Oxygen options and document types for catalogs). Since: 12.1
### addPriorityEntityResolver

void addPriorityEntityResolver([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)

Add a priority entity resolver. For performance reasons, when Oxygen only needs the URL of an entity, it does not call the EntityResolver#resolveEntity(String, String) method because it also fetches the content of the entity. To intercept also these cases, your EntityResolver should extend the [EntityUrlResolver](EntityUrlResolver.md) interface.
  Parameters: entityResolver - The entity resolver which will be called with priority before Oxygen calls the standard resolvers which are based on the catalog files specified in the preferences catalogs list and in each document type association. Since: 13
### removePriorityEntityResolver

void removePriorityEntityResolver([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)

Remove a priority entity resolver.
  Parameters: entityResolver - The entity resolver which will be called with priority before Oxygen calls the standard resolvers which are based on the catalog files specified in the preferences catalogs list and in each document type association. Since: 13
### addPriorityURIResolver

void addPriorityURIResolver([URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver)

Add a priority URI resolver.
  Parameters: uriResolver - The URI resolver which will be called with priority before Oxygen calls the standard resolvers which are based on the catalog files specified in the preferences catalogs list and in each document type association. Since: 13
### removePriorityURIResolver

void removePriorityURIResolver([URIResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/URIResolver.html) uriResolver)

Remove a priority URI resolver.
  Parameters: uriResolver - The URI resolver which will be called with priority before Oxygen calls the standard resolvers which are based on the catalog files specified in the preferences catalogs list and in each document type association. Since: 13
### threeWayAutoMerge

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [MergeResult](../../../../merge/MergeResult.md) threeWayAutoMerge([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ancestor, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) left, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) right, [MergeConflictResolutionMethods](../../../../merge/MergeConflictResolutionMethods.md) conflictResolutionMethod)
 Deprecated.
since 19.1, please use the equivalent [CompareUtilAccess](CompareUtilAccess.md) utilities.

Merges two strings representing XML files using a three way merging algorithm which needs an ancestor file.
  Parameters: ancestor - The original file string which has been modified into left and right. left - The left version of the file string, the one with "our" changes. right - The right version of the file string, the one with "others" changes. conflictResolutionMethod - The conflict resolution method to use. Returns: A merged file string where conflicts are resolved by using the left version of the file or null if the merge encountered an error. Since: 17.1
### getXMLStructureAsDTD

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXMLStructureAsDTD([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)

Get the structure of the provided XML document as a DTD.
  Parameters: reader - The reader representing the XML document to get the learn structure for. Returns: The learn structure as a DTD schema. Since: 27
### getAssociatedTransformationScenarioInputURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getAssociatedTransformationScenarioInputURL([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) xsltOrXQueryLocation)

If the given URL is for an XQuery or XSL content type, it will try to detect the XML/JSON source from the associated scenario.
  Parameters: xsltOrXQueryLocation - XSLT or XQuery location. Returns: The URL of the input from the transformation scenario or null. Since: 28  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

### getAssociatedValidationScenarioInputURL

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getAssociatedValidationScenarioInputURL([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaLocation)

If the given URL is for a schema (XSD, RNG, DTD), it will try to detect the XML/JSON source from the associated validation scenario. The first found scenario will be used.
  Parameters: schemaLocation - Schema location. Returns: The URL of the input from the validation scenario or null. Since: 28  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
