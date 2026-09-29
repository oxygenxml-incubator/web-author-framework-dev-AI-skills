Package [ro.sync.ecss.extensions.dita.topic](package-summary.md)

# Class DITATopic2_xCustomRuleMatcher

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.dita.DITACustomRuleMatcher](../DITACustomRuleMatcher.md)
        * [ro.sync.ecss.extensions.dita.topic.DITATopicCustomRuleMatcher](DITATopicCustomRuleMatcher.md)
            * ro.sync.ecss.extensions.dita.topic.DITATopic2_xCustomRuleMatcher
   All Implemented Interfaces: [DocumentTypeCustomRuleMatcher](../../api/DocumentTypeCustomRuleMatcher.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class DITATopic2_xCustomRuleMatcher extends [DITATopicCustomRuleMatcher](DITATopicCustomRuleMatcher.md)
Matches a specific DITA 2.x framework which provides support for the DITA 2.x standard.

## Constructor Summary
 Constructors
Constructor

Description
 [DITATopic2_xCustomRuleMatcher](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [matches](#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)
Try to find a DITAArchVersion attribute in the root attributes.

### Methods inherited from class ro.sync.ecss.extensions.dita.topic.[DITATopicCustomRuleMatcher](DITATopicCustomRuleMatcher.md)
 [getDescription](DITATopicCustomRuleMatcher.md#getDescription())
### Methods inherited from class ro.sync.ecss.extensions.dita.[DITACustomRuleMatcher](../DITACustomRuleMatcher.md)
 [getVersion](../DITACustomRuleMatcher.md#getVersion(org.xml.sax.Attributes))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITATopic2_xCustomRuleMatcher

public DITATopic2_xCustomRuleMatcher()

## Method Details

### matches

public boolean matches([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootNamespace, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypePublicID, [Attributes](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/Attributes.html) rootAttributes)
 Description copied from class: [DITATopicCustomRuleMatcher](DITATopicCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))
Try to find a DITAArchVersion attribute in the root attributes.
  Specified by: [matches](../../api/DocumentTypeCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)) in interface [DocumentTypeCustomRuleMatcher](../../api/DocumentTypeCustomRuleMatcher.md) Overrides: [matches](DITATopicCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes)) in class [DITATopicCustomRuleMatcher](DITATopicCustomRuleMatcher.md) Parameters: systemID - The system ID of the current file in an URL format with not allowed characters corrected. For example: "file:/C:/path/to/file/file.xml" rootNamespace - The namespace of the root. rootLocalName - The root local name. doctypePublicID - The public id of the specified DTD if any. rootAttributes - The root attributes. The attributes are DOM level 2 and the namespaces are available for each one. Returns: true if the document type to which this rule belongs to will be used for the current file. See Also:
        * [DITAMapCustomRuleMatcher.matches(java.lang.String, java.lang.String, java.lang.String, java.lang.String, org.xml.sax.Attributes)](../map/DITAMapCustomRuleMatcher.md#matches(java.lang.String,java.lang.String,java.lang.String,java.lang.String,org.xml.sax.Attributes))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
