Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class XSLTOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.operations.TransformOperation](TransformOperation.md)
        * ro.sync.ecss.extensions.commons.operations.XSLTOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class XSLTOperation extends [TransformOperation](TransformOperation.md)
An implementation of an operation to apply an XSLT stylesheet on a element and replacing it with the result of the XSLT transformation or inserting the result in the document.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.operations.[TransformOperation](TransformOperation.md)
 [ACTION_AT_CARET](TransformOperation.md#ACTION_AT_CARET), [ACTION_INSERT_AFTER](TransformOperation.md#ACTION_INSERT_AFTER), [ACTION_INSERT_AS_FIRST_CHILD](TransformOperation.md#ACTION_INSERT_AS_FIRST_CHILD), [ACTION_INSERT_AS_LAST_CHILD](TransformOperation.md#ACTION_INSERT_AS_LAST_CHILD), [ACTION_INSERT_BEFORE](TransformOperation.md#ACTION_INSERT_BEFORE), [ACTION_REPLACE](TransformOperation.md#ACTION_REPLACE), [ARGUMENT_SCRIPT](TransformOperation.md#ARGUMENT_SCRIPT), [ARGUMENT_SCRIPT_PARAMETERS](TransformOperation.md#ARGUMENT_SCRIPT_PARAMETERS), [CARET_POSITION_AFTER](TransformOperation.md#CARET_POSITION_AFTER), [CARET_POSITION_BEFORE](TransformOperation.md#CARET_POSITION_BEFORE), [CARET_POSITION_EDITABLE](TransformOperation.md#CARET_POSITION_EDITABLE), [CARET_POSITION_END](TransformOperation.md#CARET_POSITION_END), [CARET_POSITION_PRESERVE](TransformOperation.md#CARET_POSITION_PRESERVE), [CARET_POSITION_START](TransformOperation.md#CARET_POSITION_START), [CURRENT_ELEMENT_LOCATION](TransformOperation.md#CURRENT_ELEMENT_LOCATION)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [XSLTOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [canTreatAsScript](#canTreatAsScript(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) script)

 protected [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createTransformer](#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) scriptSrc)
Creates a Transformer from a given script.
  protected [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createTransformer](#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source,ro.sync.ecss.extensions.commons.operations.ElementLocationPath))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) xslSrc, ro.sync.ecss.extensions.commons.operations.ElementLocationPath currentElementLocation)
Create an XSLT transformer.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class ro.sync.ecss.extensions.commons.operations.[TransformOperation](TransformOperation.md)
 [doOperation](TransformOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)), [getArguments](TransformOperation.md#getArguments())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XSLTOperation

public XSLTOperation()

## Method Details

### createTransformer

protected [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createTransformer([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) xslSrc, ro.sync.ecss.extensions.commons.operations.ElementLocationPath currentElementLocation)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Create an XSLT transformer.
  Overrides: [createTransformer](TransformOperation.md#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source,ro.sync.ecss.extensions.commons.operations.ElementLocationPath)) in class [TransformOperation](TransformOperation.md) Parameters: authorAccess - The Author Access. xslSrc - The stylesheet source currentElementLocation - The XPath location of the current element. Returns: The transformer. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)
### createTransformer

protected [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createTransformer([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) scriptSrc)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)
 Description copied from class: [TransformOperation](TransformOperation.md#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source))
Creates a Transformer from a given script.
  Specified by: [createTransformer](TransformOperation.md#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source)) in class [TransformOperation](TransformOperation.md) Parameters: authorAccess - Access to different Author resources. scriptSrc - The XSLT or XQuery script. Returns: A JAXP Transformer that will perform the transformation defined in the given script. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html) See Also:
        * [TransformOperation.createTransformer(ro.sync.ecss.extensions.api.AuthorAccess, javax.xml.transform.Source)](TransformOperation.md#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source))

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Overrides: [getDescription](TransformOperation.md#getDescription()) in class [TransformOperation](TransformOperation.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

### canTreatAsScript

protected boolean canTreatAsScript([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) script)
  Overrides: [canTreatAsScript](TransformOperation.md#canTreatAsScript(java.lang.String)) in class [TransformOperation](TransformOperation.md) Parameters: script - The value of the script parameter. Returns: true if this is an actual script or false if it isn't. See Also:
        * [TransformOperation.canTreatAsScript(java.lang.String)](TransformOperation.md#canTreatAsScript(java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
