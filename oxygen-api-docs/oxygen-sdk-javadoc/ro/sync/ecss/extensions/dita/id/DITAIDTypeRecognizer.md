Package [ro.sync.ecss.extensions.dita.id](package-summary.md)

# Class DITAIDTypeRecognizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.link.IDTypeRecognizer](../../api/link/IDTypeRecognizer.md)
        * ro.sync.ecss.extensions.dita.id.DITAIDTypeRecognizer
   @API(type=INTERNAL, src=PUBLIC) public class DITAIDTypeRecognizer extends [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md)
Implementation of ID declarations and references recognizer for DITA framework. In this framework the IDs are declared in attributes with name 'id'. The references are recognized in href attributes.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FIRST_TOPIC_ID](#FIRST_TOPIC_ID)
Points to first topic in file containing the element ID.

### Fields inherited from class ro.sync.ecss.extensions.api.link.[IDTypeRecognizer](../../api/link/IDTypeRecognizer.md)
 [MODE_LOCATE_DECLARATIONS](../../api/link/IDTypeRecognizer.md#MODE_LOCATE_DECLARATIONS), [MODE_LOCATE_REFERENCES](../../api/link/IDTypeRecognizer.md#MODE_LOCATE_REFERENCES)
## Constructor Summary
 Constructors
Constructor

Description
 [DITAIDTypeRecognizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IDTypeIdentifier](../../api/link/IDTypeIdentifier.md)> [detectIDType](#detectIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int offset)
Detect the ID declaration or reference for the provided attribute context and offset.
  boolean [isDefaultIDTypeRecognitionAvailable](#isDefaultIDTypeRecognitionAvailable())()
If false then disable the default recognition of the IDs based on the current associated schema.
  boolean [isIDTypeRecognitionAvailable](#isIDTypeRecognitionAvailable())()
If true then ID type recognition is available.
  int[] [locateIDType](#locateIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.IDTypeIdentifier,short))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, [IDTypeIdentifier](../../api/link/IDTypeIdentifier.md) idIdentifier, short mode)
Detect if the given ID is located in the specified attribute.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### FIRST_TOPIC_ID

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FIRST_TOPIC_ID

Points to first topic in file containing the element ID.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.dita.id.DITAIDTypeRecognizer.FIRST_TOPIC_ID)

## Constructor Details

### DITAIDTypeRecognizer

public DITAIDTypeRecognizer()

## Method Details

### detectIDType

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IDTypeIdentifier](../../api/link/IDTypeIdentifier.md)> detectIDType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int offset)throws [CannotRecognizeIDException](../../api/link/CannotRecognizeIDException.md)
 Description copied from class: [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md#detectIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,int))
Detect the ID declaration or reference for the provided attribute context and offset. The offset is relative to the attribute value.
  Specified by: [detectIDType](../../api/link/IDTypeRecognizer.md#detectIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,int)) in class [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md) Parameters: systemID - The systemID of the resource that specifies the attribute. context - The element content to detect the ID. The top element from the context element stack represents the parent element. attrName - The attribute name. attrNs - The attribute namespace. attributeValue - The attribute value. offset - The offset that is relative to the attribute value. It is zero based. If it is -1 and the attribute type is IDREFS then all the IDs should be returned. Returns: The ID identifier for the given attribute and offset. If the offset is -1 and the attribute type is IDREFS then all the IDs should be returned. Can be null if no ID was detected. Throws: [CannotRecognizeIDException](../../api/link/CannotRecognizeIDException.md) - Exception that can be thrown when an ID cannot be identified in the given context. See Also:
        * [IDTypeRecognizer.detectIDType(java.lang.String, ro.sync.contentcompletion.xml.Context, java.lang.String, java.lang.String, java.lang.String, int)](../../api/link/IDTypeRecognizer.md#detectIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,int))

### locateIDType

public int[] locateIDType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, [IDTypeIdentifier](../../api/link/IDTypeIdentifier.md) idIdentifier, short mode)
 Description copied from class: [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md#locateIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.IDTypeIdentifier,short))
Detect if the given ID is located in the specified attribute. If an attribute declaration or reference was identified then compute it's location relative to the attribute value. Usually the method is used for attributes with IDREFS type to detect the internal ID references.
  Specified by: [locateIDType](../../api/link/IDTypeRecognizer.md#locateIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.IDTypeIdentifier,short)) in class [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md) Parameters: systemID - The systemID of the resource that specifies the attribute. context - The element content to detect the ID. The top element from the context element stack represents the parent element. attrName - The attribute name. attrNs - The attribute namespace. attributeValue - The attribute value. idIdentifier - The ID identifier. mode - The detection mode that is represented as a bitwise mask. Supported modes are [IDTypeRecognizer.MODE_LOCATE_REFERENCES](../../api/link/IDTypeRecognizer.md#MODE_LOCATE_REFERENCES) and [IDTypeRecognizer.MODE_LOCATE_DECLARATIONS](../../api/link/IDTypeRecognizer.md#MODE_LOCATE_DECLARATIONS). Returns: The location of the ID [startOffset, endOffset) in the given attribute value, by example if the attribute value is 'idRef1 idRef2' and we are looking for 'idRef1' the method should return [0, 6). The endOffset is exclusive. Null value can be returned if the ID was not located. See Also:
        * [IDTypeRecognizer.locateIDType(java.lang.String, ro.sync.contentcompletion.xml.Context, java.lang.String, java.lang.String, java.lang.String, ro.sync.ecss.extensions.api.link.IDTypeIdentifier, short)](../../api/link/IDTypeRecognizer.md#locateIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.IDTypeIdentifier,short))

### isDefaultIDTypeRecognitionAvailable

public boolean isDefaultIDTypeRecognitionAvailable()
 Description copied from class: [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md#isDefaultIDTypeRecognitionAvailable())
If false then disable the default recognition of the IDs based on the current associated schema. Otherwise the IDs declaration and references will be detected for document with DTD, XML Schema or RelaxNG schemas.
  Specified by: [isDefaultIDTypeRecognitionAvailable](../../api/link/IDTypeRecognizer.md#isDefaultIDTypeRecognitionAvailable()) in class [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md) Returns: True to disable the recognition of the IDs based on the current associated schema. See Also:
        * [IDTypeRecognizer.isDefaultIDTypeRecognitionAvailable()](../../api/link/IDTypeRecognizer.md#isDefaultIDTypeRecognitionAvailable())

### isIDTypeRecognitionAvailable

public boolean isIDTypeRecognitionAvailable()
 Description copied from class: [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md#isIDTypeRecognitionAvailable())
If true then ID type recognition is available. If this method return false also the default ID type recognition will be disabled.
  Specified by: [isIDTypeRecognitionAvailable](../../api/link/IDTypeRecognizer.md#isIDTypeRecognitionAvailable()) in class [IDTypeRecognizer](../../api/link/IDTypeRecognizer.md) Returns: False to disable the recognition of the IDs. See Also:
        * [IDTypeRecognizer.isIDTypeRecognitionAvailable()](../../api/link/IDTypeRecognizer.md#isIDTypeRecognitionAvailable())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
