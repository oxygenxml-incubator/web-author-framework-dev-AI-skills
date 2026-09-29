Package [ro.sync.ecss.extensions.dita.map](package-summary.md)

# Class DITAMapCustomRuleMatcher

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.dita.DITACustomRuleMatcher](../DITACustomRuleMatcher.md)
        * ro.sync.ecss.extensions.dita.map.DITAMapCustomRuleMatcher
   All Implemented Interfaces: [DocumentTypeCustomRuleMatcher](../../api/DocumentTypeCustomRuleMatcher.md), [Extension](../../api/Extension.md)   Direct Known Subclasses: [DITAMap2_xCustomRuleMatcher](DITAMap2_xCustomRuleMatcher.md)   @API(type=INTERNAL, src=PUBLIC) public class DITAMapCustomRuleMatcher extends [DITACustomRuleMatcher](../DITACustomRuleMatcher.md)
DITA map custom rule matcher.

## Constructor Summary
 Constructors
Constructor

Description
 [DITAMapCustomRuleMatcher](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 boolean [matches](#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)
Try to find a DITAArchVersion attribute in the root attributes.

### Methods inherited from class ro.sync.ecss.extensions.dita.[DITACustomRuleMatcher](../DITACustomRuleMatcher.md)
 [getVersion](../DITACustomRuleMatcher.md#getVersion(org.xml.sax.Attributes))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAMapCustomRuleMatcher

public DITAMapCustomRuleMatcher()

## Method Details

### matches

public boolean matches([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)

Try to find a DITAArchVersion attribute in the root attributes.
  Specified by: [matches](../../api/DocumentTypeCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)) in interface [DocumentTypeCustomRuleMatcher](../../api/DocumentTypeCustomRuleMatcher.md) Overrides: [matches](../DITACustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)) in class [DITACustomRuleMatcher](../DITACustomRuleMatcher.md) Parameters: systemID - The system ID of the current file in an URL format with not allowed characters corrected. For example: "file:/C:/path/to/file/file.xml" rootNamespace - The namespace of the root. rootLocalName - The root local name. doctypePublicID - The public id of the specified DTD if any. rootAttributes - The root attributes. The attributes are DOM level 2 and the namespaces are available for each one. Returns: true if the document type to which this rule belongs to will be used for the current file. See Also:
        * [DocumentTypeCustomRuleMatcher.matches(java.lang.String, java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes)](../../api/DocumentTypeCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
