Package [ro.sync.xml.parser](package-summary.md)

# Class ParserCreator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.xml.parser.ParserCreator
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class ParserCreator extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Creates all the parsers from the system. All have catalog resolvers, except the ones with specified FakeResolver.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ASSERT_COMMENT_PI_CHECKING_ID](#ASSERT_COMMENT_PI_CHECKING_ID)
Feature identifier: Enables comments and PIs for assertions processing
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [BASE_URI_FIXUP](#BASE_URI_FIXUP)
Feature identifier: base uri fixup.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CTA_FULL_XPATH_FEATURE_ID](#CTA_FULL_XPATH_FEATURE_ID)
Feature identifier: Full XPath 2.0 for CTA evaluations
  static final int [VALIDATE](#VALIDATE)
Check that the document is conformant to a strict set of rules.
  static final int [VALIDATE_OR_WELLFORMED](#VALIDATE_OR_WELLFORMED)
If the document declares the use of a schema, then it will be used validation, otherwise only a wellformed check will be done.
  static final int [WELLFORMED](#WELLFORMED)
Check if the document is conformant to a relaxed set of rules.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [XINCLUDE_FEATURE](#XINCLUDE_FEATURE)
Feature identifier: XInclude processing
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [XML_SCHEMA_VERSION](#XML_SCHEMA_VERSION)
The XML schema version Xerces parser property

## Constructor Summary
 Constructors
Constructor

Description
 [ParserCreator](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [changeValidationMode](#changeValidationMode(org.xml.sax.XMLReader,int))([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) parser, int validationMode)
Changes the validation mode.
  static [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) [createCatalogSAXSource](#createCatalogSAXSource(javax.xml.transform.stream.StreamSource))([StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) streamSource)
Create a SAX source starting from a stream source/
  static [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) [createCatalogSource](#createCatalogSource(javax.xml.transform.Source))([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) source)
Adds an XML reader with a catalog resolver in case of a stream source transforming it into a SAXSource.
  static org.apache.xerces.parsers.DOMParser [createDOMParser](#createDOMParser())()
Create a DOM parser.
  static org.apache.xerces.parsers.XMLGrammarPreparser [createDTDValidationPreparser](#createDTDValidationPreparser())()
Creates a preparser for DTD validation.
  static org.apache.xerces.parsers.DOMParser [createGrammarCachedDOMParser](#createGrammarCachedDOMParser(ro.sync.xml.parser.GrammarCache))(ro.sync.xml.parser.GrammarCache xgp)
Create a DOM parser with cached grammar
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [createGrammarCachedXMLReader](#createGrammarCachedXMLReader(ro.sync.xml.parser.GrammarCache,boolean))(ro.sync.xml.parser.GrammarCache xgp, boolean valid)
Create an XML reader with cached grammar
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [createGrammarCachedXMLReader](#createGrammarCachedXMLReader(ro.sync.xml.parser.GrammarCache,boolean,ro.sync.exml.editor.xsdeditor.XMLSchemaVersion))(ro.sync.xml.parser.GrammarCache xgp, boolean valid, ro.sync.exml.editor.xsdeditor.XMLSchemaVersion version)
Create an XML reader with cached grammar
  static org.apache.xerces.parsers.XMLGrammarPreparser [createMultipleSchemasPreparser](#createMultipleSchemasPreparser(org.xml.sax.InputSource%5B%5D))([InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html)[] sources)
Gets the XSD's Grammars from XSD Files URLs
  static org.apache.xerces.parsers.XMLGrammarPreparser [createSchemaValidationPreparser](#createSchemaValidationPreparser(ro.sync.exml.editor.xsdeditor.XMLSchemaVersion))(ro.sync.exml.editor.xsdeditor.XMLSchemaVersion schemaVersion)
Creates a preparser for schema validation.
  static org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl [createXMLGrammarPool](#createXMLGrammarPool(ro.sync.xml.parser.GrammarCache))(ro.sync.xml.parser.GrammarCache xgp)
Create the XML Grammar Pool
  static ro.sync.exml.editor.xsdeditor.XMLSchemaVersion [getSchemaVersionFromParser](#getSchemaVersionFromParser(org.xml.sax.XMLReader))([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) parser)
Gets the schema version set the parser and converts the Xerces schema version, that can be Constants.W3C_XML_SCHEMA11_NS_URI, or Constants.W3C_XML_SCHEMA10_NS_URI, to an XMLSchemaVersion object.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXercesSchemaVersionPropertyValue](#getXercesSchemaVersionPropertyValue(ro.sync.exml.editor.xsdeditor.XMLSchemaVersion))(ro.sync.exml.editor.xsdeditor.XMLSchemaVersion schemaVersion)
Converts the given enum constant representing an XML Schema version to a String value to be set for the Xerces property [XML_SCHEMA_VERSION](#XML_SCHEMA_VERSION).
  static org.apache.xerces.xni.parser.XMLInputSource [getXMLInputSource](#getXMLInputSource(org.xml.sax.InputSource))([InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) source)
Carefully creates an XMLInputSource from an InputSource.
  static org.apache.xerces.parsers.DOMParser [newAttrOrderDomParser](#newAttrOrderDomParser(boolean,boolean))(boolean sortAttributes, boolean preserveNotNormalizedAttributeValues)
Creates a DOM parser that preserves the order of attributes as they are received from Xerces.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilder](#newDocumentBuilder())()
Creates a document buider with a catalog reslover.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilder](#newDocumentBuilder(boolean,boolean,boolean))(boolean fakeResolver, boolean noExpand, boolean namespaceAware)
Create a document builder.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilder](#newDocumentBuilder(boolean,boolean,boolean,java.net.URL))(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl)
Create a document builder.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilder](#newDocumentBuilder(boolean,boolean,boolean,java.net.URL,boolean))(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl, boolean schemaAware)
Create a document builder.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilder](#newDocumentBuilder(boolean,boolean,boolean,java.net.URL,boolean,boolean))(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl, boolean schemaAware, boolean forceXIncludeAndBaseURIFixup)
Create a document builder.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilder](#newDocumentBuilder(boolean,boolean,boolean,java.net.URL,boolean,boolean,boolean))(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl, boolean schemaAware, boolean forceXIncludeAndBaseURIFixup, boolean dynamicValidation)
Create a document builder.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilderFakeResolver](#newDocumentBuilderFakeResolver())()
Creates a document buider with a fake resolver.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilderNoExpand](#newDocumentBuilderNoExpand())()
Creates a document buider with a catalog reslover.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newDocumentBuilderNS](#newDocumentBuilderNS())()
Creates a document builder which is namespace aware.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newDTDXRFullValidIdCollector](#newDTDXRFullValidIdCollector(java.util.List,org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl xgp)
Creates an XMLReader that collects ID Attributes values with full validation and schema checking, disabled std.output and with no resolver set.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newDTDXRFullValidIdCollector](#newDTDXRFullValidIdCollector(java.util.List,ro.sync.xml.parser.GrammarCache))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, ro.sync.xml.parser.GrammarCache xgc)
Creates an XMLReader that collects ID Attributes values with full validation and schema checking, disabled std.output and with no resolver set.
  static ro.sync.basic.xml.dom.LocationDomParser [newLocationDomParser](#newLocationDomParser())()
Creates a DOM Parser that populates with location information the nodes.
  static ro.sync.basic.xml.dom.LocationDomParser [newLocationDomParser](#newLocationDomParser(org.apache.xerces.xni.parser.XMLParserConfiguration,boolean))(org.apache.xerces.xni.parser.XMLParserConfiguration config, boolean dtdAware)
Creates a DOM Parser that populates with location information the nodes.
  static ro.sync.basic.xml.dom.LocationDomParser [newLocationDomParserForXpath](#newLocationDomParserForXpath())()
Creates a Location DOM Parser that is tuned for XPath.
  static ro.sync.basic.xml.dom.LocationDomParser [newLocationDomParserForXpath](#newLocationDomParserForXpath(ro.sync.basic.execution.ExecutionStopper))(ro.sync.basic.execution.ExecutionStopper executionStopper)
Creates a Location DOM Parser that is tuned for XPath.
  static ro.sync.basic.xml.dom.LocationDomParser [newLocationDomParserForXpath](#newLocationDomParserForXpath(ro.sync.basic.execution.ExecutionStopper,org.apache.xerces.xni.grammars.XMLGrammarPool))(ro.sync.basic.execution.ExecutionStopper executionStopper, org.apache.xerces.xni.grammars.XMLGrammarPool gp)
Creates a Location DOM Parser that is tuned for XPath.
  static ro.sync.basic.xml.dom.LocationDomParser [newLocationDomParserNoResolver](#newLocationDomParserNoResolver())()
Creates a DOM parser that has no catalog resolver.
  static ro.sync.basic.xml.dom.LocationDomParser [newLocationDomParserNoResolverForDiff](#newLocationDomParserNoResolverForDiff())()
Creates a DOM parser that has no catalog resolver, no DTD validation for last stage and no RNG defaults processing.
  static com.thaiopensource.validate.ValidationDriver [newRelaxNGValidator](#newRelaxNGValidator(org.xml.sax.ErrorHandler,boolean))([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax)
Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  static com.thaiopensource.validate.ValidationDriver [newRelaxNGValidator](#newRelaxNGValidator(org.xml.sax.ErrorHandler,boolean,java.util.List))([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idList)
Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  static com.thaiopensource.validate.ValidationDriver [newRelaxNGValidator](#newRelaxNGValidator(org.xml.sax.ErrorHandler,boolean,java.util.List,com.thaiopensource.xml.sax.XMLReaderCreator))([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) idList, com.thaiopensource.xml.sax.XMLReaderCreator readerCreator)
Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  static com.thaiopensource.validate.ValidationDriver [newRelaxNGValidatorNoOptions](#newRelaxNGValidatorNoOptions(org.xml.sax.ErrorHandler,boolean))([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax)
Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) [newSchemaAwareDocumentBuilder](#newSchemaAwareDocumentBuilder())()
Creates a document buider with a catalog resolver.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newWSDLFullValid](#newWSDLFullValid(org.apache.xerces.xni.grammars.XMLGrammarPool))(org.apache.xerces.xni.grammars.XMLGrammarPool grammarPool)
Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set for WSDL validation.
  static org.apache.xerces.xni.parser.XMLParserConfiguration [newXmlParserConfiguration](#newXmlParserConfiguration(org.apache.xerces.util.SymbolTable,org.apache.xerces.xni.grammars.XMLGrammarPool,java.util.List,boolean))(org.apache.xerces.util.SymbolTable st, org.apache.xerces.xni.grammars.XMLGrammarPool xgp, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, boolean fakeResolver)
Creates new XMLParserConfiguration depending on options and the list of idValues.
  static org.apache.xerces.xni.parser.XMLParserConfiguration [newXmlParserConfiguration](#newXmlParserConfiguration(org.apache.xerces.util.SymbolTable,org.apache.xerces.xni.grammars.XMLGrammarPool,java.util.List,boolean,boolean))(org.apache.xerces.util.SymbolTable st, org.apache.xerces.xni.grammars.XMLGrammarPool xgp, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, boolean fakeResolver, boolean dtdValidateForLastStage)
Creates new XMLParserConfiguration depending on options and the list of idValues.
  static org.apache.xerces.xni.parser.XMLParserConfiguration [newXmlParserConfiguration](#newXmlParserConfiguration(org.apache.xerces.util.SymbolTable,org.apache.xerces.xni.grammars.XMLGrammarPool,java.util.List,boolean,boolean,boolean))(org.apache.xerces.util.SymbolTable st, org.apache.xerces.xni.grammars.XMLGrammarPool xgp, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, boolean fakeResolver, boolean dtdValidateForLastStage, boolean forceDisableRNGDefaults)
Creates new XMLParserConfiguration depending on options and the list of idValues.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRFullValid](#newXRFullValid())()
Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRFullValid](#newXRFullValid(org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl))(org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl xgp)
Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRFullValid](#newXRFullValid(org.apache.xerces.xni.parser.XMLParserConfiguration))(org.apache.xerces.xni.parser.XMLParserConfiguration parserConfig)
Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRFullValidCompoundResolver](#newXRFullValidCompoundResolver(org.xml.sax.EntityResolver))([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Creates a XMLReader with disabled std.output and a compond resolver, from the catalog resolver and the given resolver.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRFullValidIdCollector](#newXRFullValidIdCollector(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues)
Creates an XMLReader that collects ID Attributes values with full validation and schema checking, disabled std.output and with no resolver set.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRNoValid](#newXRNoValid())()
Creates a XMLReader with disabled std.output and with no extra resolver.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRNoValid](#newXRNoValid(org.apache.xerces.xni.grammars.XMLGrammarPool))(org.apache.xerces.xni.grammars.XMLGrammarPool gp)
Creates a XMLReader with disabled std.output and with no extra resolver.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRNoValid](#newXRNoValid(ro.sync.xml.parser.GrammarCache))(ro.sync.xml.parser.GrammarCache grammarCache)
New XML reader not valid with grammar caching support.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRNoValidCompoundResolver](#newXRNoValidCompoundResolver(org.xml.sax.EntityResolver))([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)
Creates a XMLReader with disabled std.output and a compound resolver, from the catalog resolver and the given resolver.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRNoValidFakeResolver](#newXRNoValidFakeResolver())()
Creates a XMLReader with disabled std.output and with a fake resolver.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRNoValidNoRNGDefaults](#newXRNoValidNoRNGDefaults())()
New XML reader not valid without expansion of default RNG attributes.
  static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) [newXRValid](#newXRValid(org.apache.xerces.xni.grammars.XMLGrammarPool))(org.apache.xerces.xni.grammars.XMLGrammarPool grammarPool)
Creates a XMLReader with validation support.
  static void [setAcceptUndeclaredEntities](#setAcceptUndeclaredEntities(org.apache.xerces.parsers.DOMParser))(org.apache.xerces.parsers.DOMParser parser)
Set accept undeclared entities for the DOM parser.
  static void [setGrammarCacheToParser](#setGrammarCacheToParser(ro.sync.xml.parser.GrammarCache,org.apache.xerces.parsers.DOMParser))(ro.sync.xml.parser.GrammarCache xgp, org.apache.xerces.parsers.DOMParser parser)
Set the grammar cache to the parser.
  static void [setParserSystemProperties](#setParserSystemProperties())()
Sets the parser JAXP properties to point to the correct implementation.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### XINCLUDE_FEATURE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) XINCLUDE_FEATURE

Feature identifier: XInclude processing
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.XINCLUDE_FEATURE)

### BASE_URI_FIXUP

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) BASE_URI_FIXUP

Feature identifier: base uri fixup.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.BASE_URI_FIXUP)

### VALIDATE

public static final int VALIDATE

Check that the document is conformant to a strict set of rules. See validation for XML with a Schema DTD, or XSL when checking if it produces a valid Transformer.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.VALIDATE)

### WELLFORMED

public static final int WELLFORMED

Check if the document is conformant to a relaxed set of rules. See the well formed on XML.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.WELLFORMED)

### VALIDATE_OR_WELLFORMED

public static final int VALIDATE_OR_WELLFORMED

If the document declares the use of a schema, then it will be used validation, otherwise only a wellformed check will be done.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.VALIDATE_OR_WELLFORMED)

### XML_SCHEMA_VERSION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) XML_SCHEMA_VERSION

The XML schema version Xerces parser property
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.XML_SCHEMA_VERSION)

### CTA_FULL_XPATH_FEATURE_ID

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CTA_FULL_XPATH_FEATURE_ID

Feature identifier: Full XPath 2.0 for CTA evaluations
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.CTA_FULL_XPATH_FEATURE_ID)

### ASSERT_COMMENT_PI_CHECKING_ID

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ASSERT_COMMENT_PI_CHECKING_ID

Feature identifier: Enables comments and PIs for assertions processing
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.xml.parser.ParserCreator.ASSERT_COMMENT_PI_CHECKING_ID)

## Constructor Details

### ParserCreator

public ParserCreator()

## Method Details

### newDocumentBuilder

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilder(boolean fakeResolver, boolean noExpand, boolean namespaceAware)throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Create a document builder.
  Parameters: fakeResolver - true if a fake resolver should be used as an entity resolver. If false it will use oxygen catalog an entity resolver from CatalogResolverFactory. noExpand - If true the entities will not be expanded. namespaceAware - true to activate namespace awareness. Returns: A document builder. Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)
### newDocumentBuilder

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilder(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl)throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Create a document builder.
  Parameters: fakeResolver - true if a fake resolver should be used as an entity resolver. If false it will use oxygen catalog an entity resolver from CatalogResolverFactory. noExpand - If true the entities will not be expanded. namespaceAware - true to activate namespace awareness. schemaUrl - The XML schema that should be used for validation. Returns: A document builder. Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)
### newDocumentBuilder

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilder(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl, boolean schemaAware)throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Create a document builder.
  Parameters: fakeResolver - true if a fake resolver should be used as an entity resolver. If false it will use oxygen catalog an entity resolver from CatalogResolverFactory. noExpand - If true the entities will not be expanded. namespaceAware - true to activate namespace awareness. schemaUrl - The XML schema that should be used for validation. schemaAware - True if schema aware Returns: A document builder. Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)
### newDocumentBuilder

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilder(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl, boolean schemaAware, boolean forceXIncludeAndBaseURIFixup)throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Create a document builder.
  Parameters: fakeResolver - true if a fake resolver should be used as an entity resolver. If false it will use oxygen catalog an entity resolver from CatalogResolverFactory. noExpand - If true the entities will not be expanded. namespaceAware - true to activate namespace awareness. schemaUrl - The XML schema that should be used for validation. schemaAware - True if schema aware forceXIncludeAndBaseURIFixup - true if the XInclude support must be enabled no matter the options. Base URI fixup will also be enabled. Returns: A document builder. Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)
### newDocumentBuilder

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilder(boolean fakeResolver, boolean noExpand, boolean namespaceAware, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) schemaUrl, boolean schemaAware, boolean forceXIncludeAndBaseURIFixup, boolean dynamicValidation)throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Create a document builder.
  Parameters: fakeResolver - true if a fake resolver should be used as an entity resolver. If false it will use oxygen catalog an entity resolver from CatalogResolverFactory. noExpand - If true the entities will not be expanded. namespaceAware - true to activate namespace awareness. schemaUrl - The XML schema that should be used for validation. schemaAware - True if schema aware forceXIncludeAndBaseURIFixup - true if the XInclude support must be enabled no matter the options. Base URI fixup will also be enabled. dynamicValidation - true if the dynamic valication feature should be active. Returns: A document builder. Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)
### newSchemaAwareDocumentBuilder

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newSchemaAwareDocumentBuilder() throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Creates a document buider with a catalog resolver. The builder is schema aware (for DITA use) and gets the default attributes specified from the XML Schema as well.
  Returns: The Document Builder Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) - When the parsers are not conf. properly.
### newDocumentBuilder

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilder() throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Creates a document buider with a catalog reslover.
  Returns: The Document Builder Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) - When the parsers are not conf. properly.
### newDocumentBuilderFakeResolver

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilderFakeResolver() throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Creates a document buider with a fake resolver.
  Returns: The Document Builder Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) - When the parsers are not conf. properly.
### newDocumentBuilderNoExpand

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilderNoExpand() throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Creates a document buider with a catalog reslover. Does not expand external entities.
  Returns: The Document Builder Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) - When the parsers are not conf. properly.
### newDocumentBuilderNS

public static [DocumentBuilder](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/DocumentBuilder.html) newDocumentBuilderNS() throws [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html)

Creates a document builder which is namespace aware. Attaches a catalog resolver to it.
  Returns: a new DocumentBuilder Throws: [ParserConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/parsers/ParserConfigurationException.html) - When the parsers are not conf. properly.
### newXmlParserConfiguration

public static org.apache.xerces.xni.parser.XMLParserConfiguration newXmlParserConfiguration(org.apache.xerces.util.SymbolTable st, org.apache.xerces.xni.grammars.XMLGrammarPool xgp, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, boolean fakeResolver)

Creates new XMLParserConfiguration depending on options and the list of idValues.
  Parameters: st - The symbol table used during parsing. xgp - The grammar pool. idValues - The list of the collected id values. If not null creates a PSVIConfiguration. fakeResolver - true if a fake resolver will be imposed on the parser at a later time. This means the default XInclude processing should be disabled in this case, otherwise the document parsing will break in the first xi:include reference. Returns: The new XMLParserConfiguration.
### newXmlParserConfiguration

public static org.apache.xerces.xni.parser.XMLParserConfiguration newXmlParserConfiguration(org.apache.xerces.util.SymbolTable st, org.apache.xerces.xni.grammars.XMLGrammarPool xgp, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, boolean fakeResolver, boolean dtdValidateForLastStage)

Creates new XMLParserConfiguration depending on options and the list of idValues.
  Parameters: st - The symbol table used during parsing. xgp - The grammar pool. idValues - The list of the collected id values. If not null creates a PSVIConfiguration. fakeResolver - true if a fake resolver will be imposed on the parser at a later time. This means the default XInclude processing should be disabled in this case, otherwise the document parsing will break in the first xi:include reference. dtdValidateForLastStage - Add the DTD validation as the last stage in the parser. Returns: The new XMLParserConfiguration.
### newXmlParserConfiguration

public static org.apache.xerces.xni.parser.XMLParserConfiguration newXmlParserConfiguration(org.apache.xerces.util.SymbolTable st, org.apache.xerces.xni.grammars.XMLGrammarPool xgp, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, boolean fakeResolver, boolean dtdValidateForLastStage, boolean forceDisableRNGDefaults)

Creates new XMLParserConfiguration depending on options and the list of idValues.
  Parameters: st - The symbol table used during parsing. xgp - The grammar pool. idValues - The list of the collected id values. If not null creates a PSVIConfiguration. fakeResolver - true if a fake resolver will be imposed on the parser at a later time. This means the default XInclude processing should be disabled in this case, otherwise the document parsing will break in the first xi:include reference. dtdValidateForLastStage - Add the DTD validation as the last stage in the parser. forceDisableRNGDefaults - true if the RNG defaults should be disabled no matter what the option says. This is used for diff parser. Returns: The new XMLParserConfiguration.
### newXRNoValidFakeResolver

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRNoValidFakeResolver()

Creates a XMLReader with disabled std.output and with a fake resolver. The parser is NOT continuing after fatal error and is not validating.
  Returns: an XMLReader
### newXRFullValidCompoundResolver

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRFullValidCompoundResolver([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)

Creates a XMLReader with disabled std.output and a compond resolver, from the catalog resolver and the given resolver. The parser is continuing after fatal error and is validating.
  Parameters: entityResolver - The entity resolver to be compound with the xml catalog resolver. Returns: an XMLReader
### newXRNoValidCompoundResolver

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRNoValidCompoundResolver([EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html) entityResolver)

Creates a XMLReader with disabled std.output and a compound resolver, from the catalog resolver and the given resolver. The parser is NOT continuing after fatal error and is not validating.
  Parameters: entityResolver - The entity resolver to be compound with the xml catalog resolver. Returns: an XMLReader
### newXRNoValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRNoValid(org.apache.xerces.xni.grammars.XMLGrammarPool gp)

Creates a XMLReader with disabled std.output and with no extra resolver. The parser is NOT continuing after fatal error and is not validating. The catalog resolver is installed.
  Parameters: gp - Grammar pool which can be reused. Returns: an XMLReader
### newXRNoValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRNoValid()

Creates a XMLReader with disabled std.output and with no extra resolver. The parser is NOT continuing after fatal error and is not validating. The catalog resolver is installed.
  Returns: an XMLReader
### newXRFullValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRFullValid(org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl xgp)

Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set. The parser is not continuing after fatal error.
The parser has the catalog entity resolver.

  Parameters: xgp - XML Grammar pool Returns: an XMLReader
### newXRFullValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRFullValid()

Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set. The parser is not continuing after fatal error.
The parser has the catalog entity resolver.

  Returns: an XMLReader
### newXRFullValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRFullValid(org.apache.xerces.xni.parser.XMLParserConfiguration parserConfig)

Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set. The parser is not continuing after fatal error.
The parser has the catalog entity resolver.

  Parameters: parserConfig - The parser configuration Returns: an XMLReader
### newWSDLFullValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newWSDLFullValid(org.apache.xerces.xni.grammars.XMLGrammarPool grammarPool)

Creates a XMLReader with full validation and schema checking, disabled std.output and with no resolver set for WSDL validation. The parser is not continuing after fatal error.
The parser has the catalog entity resolver.

  Parameters: grammarPool - The pool containing the grammars the parser must use to validate the documents. Returns: an XMLReader
### newXRValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRValid(org.apache.xerces.xni.grammars.XMLGrammarPool grammarPool)

Creates a XMLReader with validation support. The parser has the catalog entity resolver.
  Parameters: grammarPool - In this pool the parser stores the grammars. They can be further used to examine them. Returns: an XMLReader
### newRelaxNGValidator

public static com.thaiopensource.validate.ValidationDriver newRelaxNGValidator([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax)

Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  Parameters: errorHandler - The error handler to be set to the parser. useCompactSyntax - If true the Relax NG grammar is in compact syntax otherwise in XML syntax. Returns: Verifier the new Relax NG verifier. A ValidationDriver instance.
### newRelaxNGValidator

public static com.thaiopensource.validate.ValidationDriver newRelaxNGValidator([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idList)

Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  Parameters: errorHandler - The error handler to be set to the parser. useCompactSyntax - If true the Relax NG grammar is in compact syntax otherwise in XML syntax. idList - The list of id values to be colected. Returns: Verifier the new Relax NG verifier. A ValidationDriver instance.
### newRelaxNGValidatorNoOptions

public static com.thaiopensource.validate.ValidationDriver newRelaxNGValidatorNoOptions([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax)

Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  Parameters: errorHandler - The error handler to be set to the parser. useCompactSyntax - If true the Relax NG grammar is in compact syntax otherwise in XML syntax. Returns: Verifier the new Relax NG verifier. A ValidationDriver instance.
### newRelaxNGValidator

public static com.thaiopensource.validate.ValidationDriver newRelaxNGValidator([ErrorHandler](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/ErrorHandler.html) errorHandler, boolean useCompactSyntax, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) idList, com.thaiopensource.xml.sax.XMLReaderCreator readerCreator)

Creates a Relax NG validation engine to validate against schemas in XML or compact syntax.
  Parameters: errorHandler - The error handler to be set to the parser. useCompactSyntax - If true the Relax NG grammar is in compact syntax otherwise in XML syntax. idList - The list of id values to be colected. readerCreator - The XMLReaderCreator to be used. Returns: Verifier the new Relax NG verifier. A ValidationDriver instance.
### newAttrOrderDomParser

public static org.apache.xerces.parsers.DOMParser newAttrOrderDomParser(boolean sortAttributes, boolean preserveNotNormalizedAttributeValues)throws [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)

Creates a DOM parser that preserves the order of attributes as they are received from Xerces.
  Parameters: sortAttributes - True if the attributes must be sorted. This is the default implementation in the DOMParser. False if the order of the attributes must be stored in a userdata in a node. preserveNotNormalizedAttributeValues - True if the not normalized (original) attribute values must be preserved. Returns: A Xerces DOM parser with some features set and with a fake entity resolver. Throws: [SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html) - If the features of the parser could not be set.
### newXRFullValidIdCollector

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRFullValidIdCollector([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues)

Creates an XMLReader that collects ID Attributes values with full validation and schema checking, disabled std.output and with no resolver set. The parser is not continuing after fatal error.
The parser has the catalog entity resolver.

  Parameters: idValues - The list of ID values to be modified. Returns: an XMLReader
### newDTDXRFullValidIdCollector

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newDTDXRFullValidIdCollector([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, ro.sync.xml.parser.GrammarCache xgc)

Creates an XMLReader that collects ID Attributes values with full validation and schema checking, disabled std.output and with no resolver set. The parser is not continuing after fatal error.
The parser has the catalog entity resolver.

  Parameters: idValues - The list of ID values to be modified. xgc - The XML Grammar cache, if available Returns: an XMLReader
### newDTDXRFullValidIdCollector

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newDTDXRFullValidIdCollector([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.xml.parser.IDValue> idValues, org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl xgp)

Creates an XMLReader that collects ID Attributes values with full validation and schema checking, disabled std.output and with no resolver set. The parser is not continuing after fatal error.
The parser has the catalog entity resolver.

  Parameters: idValues - The list of ID values to be modified. xgp - The XML Grammar cache, if available Returns: an XMLReader
### changeValidationMode

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) changeValidationMode([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) parser, int validationMode)

Changes the validation mode.
  Parameters: parser - The xml reader to be changed the mode. validationMode - The validation operation. Returns: The same xmlReader as input.
### newLocationDomParser

public static ro.sync.basic.xml.dom.LocationDomParser newLocationDomParser()

Creates a DOM Parser that populates with location information the nodes.
  Returns: The new parser.
### newLocationDomParser

public static ro.sync.basic.xml.dom.LocationDomParser newLocationDomParser(org.apache.xerces.xni.parser.XMLParserConfiguration config, boolean dtdAware)

Creates a DOM Parser that populates with location information the nodes. Call LocationDomParser.setInputSource if the parser will be started from the configuration.
  Parameters: config - The parser configuration. dtdAware - true if the parser is DTD aware. Returns: The new parser.
### newLocationDomParserNoResolver

public static ro.sync.basic.xml.dom.LocationDomParser newLocationDomParserNoResolver()

Creates a DOM parser that has no catalog resolver.
  Returns: The new dom parser.
### newLocationDomParserNoResolverForDiff

public static ro.sync.basic.xml.dom.LocationDomParser newLocationDomParserNoResolverForDiff()

Creates a DOM parser that has no catalog resolver, no DTD validation for last stage and no RNG defaults processing.
  Returns: The new dom parser.
### setAcceptUndeclaredEntities

public static void setAcceptUndeclaredEntities(org.apache.xerces.parsers.DOMParser parser)

Set accept undeclared entities for the DOM parser.
  Parameters: parser - The DOM parser to set the feature on.
### setParserSystemProperties

public static void setParserSystemProperties()

Sets the parser JAXP properties to point to the correct implementation.

### newLocationDomParserForXpath

public static ro.sync.basic.xml.dom.LocationDomParser newLocationDomParserForXpath()

Creates a Location DOM Parser that is tuned for XPath. It will expand external entities and store their systemID in the nodes.
  Returns: A new location dom parser.
### newLocationDomParserForXpath

public static ro.sync.basic.xml.dom.LocationDomParser newLocationDomParserForXpath(ro.sync.basic.execution.ExecutionStopper executionStopper)

Creates a Location DOM Parser that is tuned for XPath. It will expand external entities and store their systemID in the nodes.
  Parameters: executionStopper - The execution stopper. Can be null Returns: A new location dom parser.
### newLocationDomParserForXpath

public static ro.sync.basic.xml.dom.LocationDomParser newLocationDomParserForXpath(ro.sync.basic.execution.ExecutionStopper executionStopper, org.apache.xerces.xni.grammars.XMLGrammarPool gp)

Creates a Location DOM Parser that is tuned for XPath. It will expand external entities and store their systemID in the nodes.
  Parameters: executionStopper - The execution stopper. Can be null gp - The grammar pool. Can be null Returns: A new location dom parser.
### createSchemaValidationPreparser

public static org.apache.xerces.parsers.XMLGrammarPreparser createSchemaValidationPreparser(ro.sync.exml.editor.xsdeditor.XMLSchemaVersion schemaVersion)

Creates a preparser for schema validation.
  Parameters: schemaVersion - An XML Schema version. Returns: A preparser used for XML Schema validation.
### getXercesSchemaVersionPropertyValue

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXercesSchemaVersionPropertyValue(ro.sync.exml.editor.xsdeditor.XMLSchemaVersion schemaVersion)

Converts the given enum constant representing an XML Schema version to a String value to be set for the Xerces property [XML_SCHEMA_VERSION](#XML_SCHEMA_VERSION).
  Parameters: schemaVersion - An XML Schema version. Returns: String value to be set for the Xerces property [XML_SCHEMA_VERSION](#XML_SCHEMA_VERSION).
### getSchemaVersionFromParser

public static ro.sync.exml.editor.xsdeditor.XMLSchemaVersion getSchemaVersionFromParser([XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) parser)

Gets the schema version set the parser and converts the Xerces schema version, that can be Constants.W3C_XML_SCHEMA11_NS_URI, or Constants.W3C_XML_SCHEMA10_NS_URI, to an XMLSchemaVersion object.
  Parameters: parser - The parser to get the schema version from. Returns: the XML schema version as an XMLSchemaVersion object.
### createDTDValidationPreparser

public static org.apache.xerces.parsers.XMLGrammarPreparser createDTDValidationPreparser()

Creates a preparser for DTD validation.
  Returns: A preparser used for DTD validation
### createMultipleSchemasPreparser

public static org.apache.xerces.parsers.XMLGrammarPreparser createMultipleSchemasPreparser([InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html)[] sources)

Gets the XSD's Grammars from XSD Files URLs
  Parameters: sources - The URLs Returns: The Grammar Preparser
### getXMLInputSource

public static org.apache.xerces.xni.parser.XMLInputSource getXMLInputSource([InputSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/InputSource.html) source)

Carefully creates an XMLInputSource from an InputSource.
  Parameters: source - The input source. Returns: The corresponding xml input source.
### createCatalogSource

public static [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) createCatalogSource([Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) source)

Adds an XML reader with a catalog resolver in case of a stream source transforming it into a SAXSource.
  Parameters: source - The source. Returns: A new source or the argument if the input is a DOMSource or a SAXSource.
### createCatalogSAXSource

public static [SAXSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/sax/SAXSource.html) createCatalogSAXSource([StreamSource](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/stream/StreamSource.html) streamSource)

Create a SAX source starting from a stream source/
  Parameters: streamSource - The stream source. Returns: A SAX source.
### createGrammarCachedXMLReader

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) createGrammarCachedXMLReader(ro.sync.xml.parser.GrammarCache xgp, boolean valid)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)

Create an XML reader with cached grammar
  Parameters: xgp - The grammar pool caching valid - True if also validates Returns: The XML Reader Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
### createGrammarCachedXMLReader

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) createGrammarCachedXMLReader(ro.sync.xml.parser.GrammarCache xgp, boolean valid, ro.sync.exml.editor.xsdeditor.XMLSchemaVersion version)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)

Create an XML reader with cached grammar
  Parameters: xgp - The grammar pool caching valid - True if also validates version - The XML Schema version to use. Can be null. Returns: The XML Reader Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
### createXMLGrammarPool

public static org.apache.xerces.util.SynchronizedXMLGrammarPoolImpl createXMLGrammarPool(ro.sync.xml.parser.GrammarCache xgp)

Create the XML Grammar Pool
  Parameters: xgp - The XML Grammar Pool cacher. Returns: The XML Grammar Pool
### createDOMParser

public static org.apache.xerces.parsers.DOMParser createDOMParser() throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)

Create a DOM parser.
  Returns: The DOM Parser. Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
### createGrammarCachedDOMParser

public static org.apache.xerces.parsers.DOMParser createGrammarCachedDOMParser(ro.sync.xml.parser.GrammarCache xgp)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)

Create a DOM parser with cached grammar
  Parameters: xgp - The grammar pool caching. Returns: The DOM Parser. Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
### setGrammarCacheToParser

public static void setGrammarCacheToParser(ro.sync.xml.parser.GrammarCache xgp, org.apache.xerces.parsers.DOMParser parser)throws [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html), [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)

Set the grammar cache to the parser.
  Parameters: xgp - The grammar cache. parser - The parser. Throws: [SAXNotRecognizedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotRecognizedException.html) [SAXNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXNotSupportedException.html)
### newXRNoValidNoRNGDefaults

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRNoValidNoRNGDefaults()

New XML reader not valid without expansion of default RNG attributes.
  Returns: The XML reader
### newXRNoValid

public static [XMLReader](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/XMLReader.html) newXRNoValid(ro.sync.xml.parser.GrammarCache grammarCache)

New XML reader not valid with grammar caching support.
  Parameters: grammarCache - The grammar cache Returns: The XML reader
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
