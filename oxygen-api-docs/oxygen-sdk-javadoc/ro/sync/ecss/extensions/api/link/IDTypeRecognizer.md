Package [ro.sync.ecss.extensions.api.link](package-summary.md)

# Class IDTypeRecognizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.link.IDTypeRecognizer
   Direct Known Subclasses: [DITAIDTypeRecognizer](../../dita/id/DITAIDTypeRecognizer.md), [TEIP5IDTypeRecognizer](../../tei/id/TEIP5IDTypeRecognizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class IDTypeRecognizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Recognizer for ID declaration and references in attribute values. The recognizer may be used when search references and declaration for a particular ID.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final short [MODE_LOCATE_DECLARATIONS](#MODE_LOCATE_DECLARATIONS)
Mode used when locate an ID.
  static final short [MODE_LOCATE_REFERENCES](#MODE_LOCATE_REFERENCES)
Mode used when locate an ID.

## Constructor Summary
 Constructors
Constructor

Description
 [IDTypeRecognizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IDTypeIdentifier](IDTypeIdentifier.md)> [detectIDType](#detectIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int offset)
Detect the ID declaration or reference for the provided attribute context and offset.
  abstract boolean [isDefaultIDTypeRecognitionAvailable](#isDefaultIDTypeRecognitionAvailable())()
If false then disable the default recognition of the IDs based on the current associated schema.
  abstract boolean [isIDTypeRecognitionAvailable](#isIDTypeRecognitionAvailable())()
If true then ID type recognition is available.
  abstract int[] [locateIDType](#locateIDType(java.lang.String,ro.sync.contentcompletion.xml.Context,java.lang.String,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.link.IDTypeIdentifier,short))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, [IDTypeIdentifier](IDTypeIdentifier.md) idIdentifier, short mode)
Detect if the given ID is located in the specified attribute.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### MODE_LOCATE_DECLARATIONS

public static final short MODE_LOCATE_DECLARATIONS

Mode used when locate an ID. It is used to locate declaration.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.link.IDTypeRecognizer.MODE_LOCATE_DECLARATIONS)

### MODE_LOCATE_REFERENCES

public static final short MODE_LOCATE_REFERENCES

Mode used when locate an ID. It is used to locate references.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.link.IDTypeRecognizer.MODE_LOCATE_REFERENCES)

## Constructor Details

### IDTypeRecognizer

public IDTypeRecognizer()

## Method Details

### detectIDType

public abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[IDTypeIdentifier](IDTypeIdentifier.md)> detectIDType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, int offset)throws [CannotRecognizeIDException](CannotRecognizeIDException.md)

Detect the ID declaration or reference for the provided attribute context and offset. The offset is relative to the attribute value.
  Parameters: systemID - The systemID of the resource that specifies the attribute. context - The element content to detect the ID. The top element from the context element stack represents the parent element. attrName - The attribute name. attrNs - The attribute namespace. attributeValue - The attribute value. offset - The offset that is relative to the attribute value. It is zero based. If it is -1 and the attribute type is IDREFS then all the IDs should be returned. Returns: The ID identifier for the given attribute and offset. If the offset is -1 and the attribute type is IDREFS then all the IDs should be returned. Can be null if no ID was detected. Throws: [CannotRecognizeIDException](CannotRecognizeIDException.md) - Exception that can be thrown when an ID cannot be identified in the given context.
### locateIDType

public abstract int[] locateIDType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [Context](../../../../contentcompletion/xml/Context.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attributeValue, [IDTypeIdentifier](IDTypeIdentifier.md) idIdentifier, short mode)

Detect if the given ID is located in the specified attribute. If an attribute declaration or reference was identified then compute it's location relative to the attribute value. Usually the method is used for attributes with IDREFS type to detect the internal ID references.
  Parameters: systemID - The systemID of the resource that specifies the attribute. context - The element content to detect the ID. The top element from the context element stack represents the parent element. attrName - The attribute name. attrNs - The attribute namespace. attributeValue - The attribute value. idIdentifier - The ID identifier. mode - The detection mode that is represented as a bitwise mask. Supported modes are [MODE_LOCATE_REFERENCES](#MODE_LOCATE_REFERENCES) and [MODE_LOCATE_DECLARATIONS](#MODE_LOCATE_DECLARATIONS). Returns: The location of the ID [startOffset, endOffset) in the given attribute value, by example if the attribute value is 'idRef1 idRef2' and we are looking for 'idRef1' the method should return [0, 6). The endOffset is exclusive. Null value can be returned if the ID was not located.
### isDefaultIDTypeRecognitionAvailable

public abstract boolean isDefaultIDTypeRecognitionAvailable()

If false then disable the default recognition of the IDs based on the current associated schema. Otherwise the IDs declaration and references will be detected for document with DTD, XML Schema or RelaxNG schemas.
  Returns: True to disable the recognition of the IDs based on the current associated schema.
### isIDTypeRecognitionAvailable

public abstract boolean isIDTypeRecognitionAvailable()

If true then ID type recognition is available. If this method return false also the default ID type recognition will be disabled.
  Returns: False to disable the recognition of the IDs.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
