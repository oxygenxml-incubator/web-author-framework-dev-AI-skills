Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITACustomRuleMatcher

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.DITACustomRuleMatcher
   All Implemented Interfaces: [DocumentTypeCustomRuleMatcher](../api/DocumentTypeCustomRuleMatcher.md), [Extension](../api/Extension.md)   Direct Known Subclasses: [DITAMapCustomRuleMatcher](map/DITAMapCustomRuleMatcher.md), [DITATopicCustomRuleMatcher](topic/DITATopicCustomRuleMatcher.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class DITACustomRuleMatcher extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [DocumentTypeCustomRuleMatcher](../api/DocumentTypeCustomRuleMatcher.md)
DITA custom rule matcher abstract class.

## Constructor Summary
 Constructors
Constructor

Description
 [DITACustomRuleMatcher](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getVersion](#getVersion(org.xml.sax.Attributes))([Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)
Get the value of the ditaarch version attribute
  boolean [matches](#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)
Try to find a DITAArchVersion attribute in the root attributes.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](../api/Extension.md)
 [getDescription](../api/Extension.md#getDescription())
## Constructor Details

### DITACustomRuleMatcher

public DITACustomRuleMatcher()

## Method Details

### matches

public boolean matches([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)

Try to find a DITAArchVersion attribute in the root attributes.
  Specified by: [matches](../api/DocumentTypeCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)) in interface [DocumentTypeCustomRuleMatcher](../api/DocumentTypeCustomRuleMatcher.md) Parameters: systemID - The system ID of the current file in an URL format with not allowed characters corrected. For example: "file:/C:/path/to/file/file.xml" rootNamespace - The namespace of the root. rootLocalName - The root local name. doctypePublicID - The public id of the specified DTD if any. rootAttributes - The root attributes. The attributes are DOM level 2 and the namespaces are available for each one. Returns: true if the document type to which this rule belongs to will be used for the current file. See Also:
        * [DocumentTypeCustomRuleMatcher.matches(java.lang.String, java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes)](../api/DocumentTypeCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))

### getVersion

protected static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getVersion([Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)

Get the value of the ditaarch version attribute
  Parameters: rootAttributes - Root attributes. Returns: the value or null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
