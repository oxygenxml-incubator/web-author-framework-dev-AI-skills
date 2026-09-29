Package [ro.sync.json](package-summary.md)

# Class JSONAndYAMLPropertiesRuleMatcherBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.DocumentTypeAdvancedCustomRuleMatcher](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md)
        * ro.sync.json.JSONAndYAMLPropertiesRuleMatcherBase
   All Implemented Interfaces: [DocumentTypeCustomRuleMatcher](../ecss/extensions/api/DocumentTypeCustomRuleMatcher.md), [Extension](../ecss/extensions/api/Extension.md)   @API(type=EXTENDABLE, src=PRIVATE) public abstract class JSONAndYAMLPropertiesRuleMatcherBase extends [DocumentTypeAdvancedCustomRuleMatcher](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md)
Matcher for schemas that have no versions, but have required properties. (ex: JSON-LD)

## Constructor Summary
 Constructors
Modifier

Constructor

Description
 protected  [JSONAndYAMLPropertiesRuleMatcherBase](#%3Cinit%3E(java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] props)
Constructor

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [matches](#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.io.Reader))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) contentReader)
Check if the document type to which this custom rule belongs to should be used for the given document properties.

### Methods inherited from class ro.sync.ecss.extensions.api.[DocumentTypeAdvancedCustomRuleMatcher](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md)
 [matches](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.util.Map,java.io.Reader)), [matches](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../ecss/extensions/api/Extension.md)
 [getDescription](../ecss/extensions/api/Extension.md#getDescription())
## Constructor Details

### JSONAndYAMLPropertiesRuleMatcherBase

protected JSONAndYAMLPropertiesRuleMatcherBase([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] props)

Constructor
  Parameters: props - The expected properties.
## Method Details

### matches

public boolean matches([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) contentReader)
 Description copied from class: [DocumentTypeAdvancedCustomRuleMatcher](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.io.Reader))
Check if the document type to which this custom rule belongs to should be used for the given document properties. This method receives a reader over the entire content.
  Overrides: [matches](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.io.Reader)) in class [DocumentTypeAdvancedCustomRuleMatcher](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md) Parameters: systemID - The system ID of the current file in an URL format with not allowed characters corrected. For example: "file:/C:/path/to/file/file.xml" rootNamespace - The namespace of the root. rootLocalName - The root local name. doctypePublicID - The public id of the specified DTD if any. rootAttributes - The root attributes. The attributes are DOM level 2 and the namespaces are available for each one. contentReader - Reader over the entire XML content. Can be used for detection if all other parameters are not enough. The reader does not need to be reset or closed. It may be null. Returns: true if the document type to which this rule belongs to will be used for the current file. See Also:
        * [DocumentTypeAdvancedCustomRuleMatcher.matches(java.lang.String, java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes, java.io.Reader)](../ecss/extensions/api/DocumentTypeAdvancedCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes,java.io.Reader))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
