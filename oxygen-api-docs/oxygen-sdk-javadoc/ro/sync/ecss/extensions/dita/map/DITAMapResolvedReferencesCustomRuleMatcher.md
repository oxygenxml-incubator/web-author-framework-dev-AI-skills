Package [ro.sync.ecss.extensions.dita.map](package-summary.md)

# Class DITAMapResolvedReferencesCustomRuleMatcher

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.DocumentTypeAdvancedCustomRuleMatcher](../../api/DocumentTypeAdvancedCustomRuleMatcher.md)
        * ro.sync.ecss.extensions.dita.map.DITAMapResolvedReferencesCustomRuleMatcher
   All Implemented Interfaces: [DocumentTypeCustomRuleMatcher](../../api/DocumentTypeCustomRuleMatcher.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAMapResolvedReferencesCustomRuleMatcher extends [DocumentTypeAdvancedCustomRuleMatcher](../../api/DocumentTypeAdvancedCustomRuleMatcher.md)
Matches a specific DITA Map opened with resolved topics

## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapResolvedReferencesCustomRuleMatcher](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 boolean [matches](#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.util.Map,java.io.Reader))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypeSystemID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> queryParameters, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) contentReader)
Check if the document type to which this custom rule belongs to should be used for the given document properties.

### Methods inherited from class ro.sync.ecss.extensions.api.[DocumentTypeAdvancedCustomRuleMatcher](../../api/DocumentTypeAdvancedCustomRuleMatcher.md)
 [matches](../../api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)), [matches](../../api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.io.Reader))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAMapResolvedReferencesCustomRuleMatcher

public DITAMapResolvedReferencesCustomRuleMatcher()

## Method Details

### matches

public boolean matches([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypeSystemID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> queryParameters, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) contentReader)
 Description copied from class: [DocumentTypeAdvancedCustomRuleMatcher](../../api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.util.Map,java.io.Reader))
Check if the document type to which this custom rule belongs to should be used for the given document properties. This method receives a reader over the entire content.
  Overrides: [matches](../../api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.util.Map,java.io.Reader)) in class [DocumentTypeAdvancedCustomRuleMatcher](../../api/DocumentTypeAdvancedCustomRuleMatcher.md) Parameters: systemID - The system ID of the current file in an URL format with not allowed characters corrected. For example: "file:/C:/path/to/file/file.xml" rootNamespace - The namespace of the root. rootLocalName - The root local name. doctypePublicID - The public id of the specified DTD if any. doctypeSystemID - The system id of the specified DTD if any. rootAttributes - The root attributes. The attributes are DOM level 2 and the namespaces are available for each one. queryParameters - The parameters which were set in the query string used to open this resource. May be null. contentReader - Reader over the entire XML content. Can be used for detection if all other parameters are not enough. The reader does not need to be reset or closed. It may be null. Returns: true if the document type to which this rule belongs to will be used for the current file. See Also:
        * [DocumentTypeAdvancedCustomRuleMatcher.matches(java.lang.String, java.lang.String, java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes, java.util.Map, java.io.Reader)](../../api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.util.Map,java.io.Reader))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
