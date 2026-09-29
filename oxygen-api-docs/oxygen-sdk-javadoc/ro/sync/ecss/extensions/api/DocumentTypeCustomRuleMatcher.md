Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface DocumentTypeCustomRuleMatcher
    All Superinterfaces: [Extension](Extension.md)   All Known Implementing Classes: [DITACustomRuleMatcher](../dita/DITACustomRuleMatcher.md), [DITAMap2_xCustomRuleMatcher](../dita/map/DITAMap2_xCustomRuleMatcher.md), [DITAMapCustomRuleMatcher](../dita/map/DITAMapCustomRuleMatcher.md), [DITAMapResolvedReferencesCustomRuleMatcher](../dita/map/DITAMapResolvedReferencesCustomRuleMatcher.md), [DITATopic2_xCustomRuleMatcher](../dita/topic/DITATopic2_xCustomRuleMatcher.md), [DITATopicCustomRuleMatcher](../dita/topic/DITATopicCustomRuleMatcher.md), [DocumentTypeAdvancedCustomRuleMatcher](DocumentTypeAdvancedCustomRuleMatcher.md), [HTML5CustomRuleMatcher](../html/HTML5CustomRuleMatcher.md), [JSONAndYAMLPropertiesRuleMatcherBase](../../../json/JSONAndYAMLPropertiesRuleMatcherBase.md), [JSONAndYAMLRuleMatcherBase](../../../json/JSONAndYAMLRuleMatcherBase.md), [WebAuthorPlatformCustomRuleMatcher](../xhtml/WebAuthorPlatformCustomRuleMatcher.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface DocumentTypeCustomRuleMatcherextends [Extension](Extension.md)
Interface which can be implemented to provide custom matching to the document type it belongs to.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [matches](#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)
Check if the document type to which this custom rule belongs to should be used for the given document properties.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### matches

boolean matches([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)

Check if the document type to which this custom rule belongs to should be used for the given document properties.
  Parameters: systemID - The system ID of the current file in an URL format with not allowed characters corrected. For example: "file:/C:/path/to/file/file.xml" rootNamespace - The namespace of the root. rootLocalName - The root local name. doctypePublicID - The public id of the specified DTD if any. rootAttributes - The root attributes. The attributes are DOM level 2 and the namespaces are available for each one. Returns: true if the document type to which this rule belongs to will be used for the current file.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
