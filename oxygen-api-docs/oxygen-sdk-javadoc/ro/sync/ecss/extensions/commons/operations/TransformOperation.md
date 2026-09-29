Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class TransformOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.TransformOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   Direct Known Subclasses: [XQueryOperation](XQueryOperation.md), [XSLTOperation](XSLTOperation.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class TransformOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../api/AuthorOperation.md)
An implementation of an operation to apply a script (XSLT or XQuery) on a element and replacing it with the result of the transformation or inserting the result in the document.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_AT_CARET](#ACTION_AT_CARET)
The name of the operation action indicating that the transformation result should be inserted at the caret position.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_INSERT_AFTER](#ACTION_INSERT_AFTER)
The name of the operation action indicating that the transformation result should be inserted after the target node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_INSERT_AS_FIRST_CHILD](#ACTION_INSERT_AS_FIRST_CHILD)
The name of the operation action indicating that the transformation result should be inserted as the first child of the target node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_INSERT_AS_LAST_CHILD](#ACTION_INSERT_AS_LAST_CHILD)
The name of the operation action indicating that the transformation result should be inserted as the last child of the target node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_INSERT_BEFORE](#ACTION_INSERT_BEFORE)
The name of the operation action indicating that the transformation result should be inserted before the target node.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ACTION_REPLACE](#ACTION_REPLACE)
The name of the operation action indicating a replace of the target node with the result of the transformation.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_SCRIPT](#ARGUMENT_SCRIPT)
The XSLT or XQuery script.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_SCRIPT_PARAMETERS](#ARGUMENT_SCRIPT_PARAMETERS)
External parameters argument.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CARET_POSITION_AFTER](#CARET_POSITION_AFTER)
Constant for the caret position indicating that the caret should be positioned just after the inserted fragment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CARET_POSITION_BEFORE](#CARET_POSITION_BEFORE)
Constant for the caret position indicating that the caret should be positioned just before the inserted fragment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CARET_POSITION_EDITABLE](#CARET_POSITION_EDITABLE)
Constant for the caret position indicating that the caret should be positioned just at the start of the inserted fragment, in the first editable position.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CARET_POSITION_END](#CARET_POSITION_END)
Constant for the caret position indicating that the caret should be positioned just at the end of the inserted fragment, inside that fragment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CARET_POSITION_PRESERVE](#CARET_POSITION_PRESERVE)
Constant for the caret position indicating that the same caret position offset should be preserved.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CARET_POSITION_START](#CARET_POSITION_START)
Constant for the caret position indicating that the caret should be positioned just at the start of the inserted fragment, inside that fragment.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CURRENT_ELEMENT_LOCATION](#CURRENT_ELEMENT_LOCATION)
The name of a parameter containing the location path of the current element inside the source element.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [TransformOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 protected boolean [canTreatAsScript](#canTreatAsScript(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) script)

 protected abstract [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createTransformer](#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) scriptSrc)
Creates a Transformer from a given script.
  protected [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) [createTransformer](#createTransformer(ro.sync.ecss.extensions.api.AuthorAccess,javax.xml.transform.Source,ro.sync.ecss.extensions.commons.operations.ElementLocationPath))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) scriptSrc, ro.sync.ecss.extensions.commons.operations.ElementLocationPath location)
Creates a Transformer from a given script.
  void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)
Applies the transformation and executes the specified action with the result.
  [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### CURRENT_ELEMENT_LOCATION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CURRENT_ELEMENT_LOCATION

The name of a parameter containing the location path of the current element inside the source element. This can be accessed in the script to perform context sensitive actions.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.CURRENT_ELEMENT_LOCATION)

### ACTION_REPLACE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_REPLACE

The name of the operation action indicating a replace of the target node with the result of the transformation.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.ACTION_REPLACE)

### ACTION_AT_CARET

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_AT_CARET

The name of the operation action indicating that the transformation result should be inserted at the caret position.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.ACTION_AT_CARET)

### ACTION_INSERT_BEFORE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_INSERT_BEFORE

The name of the operation action indicating that the transformation result should be inserted before the target node.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.ACTION_INSERT_BEFORE)

### ACTION_INSERT_AFTER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_INSERT_AFTER

The name of the operation action indicating that the transformation result should be inserted after the target node.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.ACTION_INSERT_AFTER)

### ACTION_INSERT_AS_FIRST_CHILD

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_INSERT_AS_FIRST_CHILD

The name of the operation action indicating that the transformation result should be inserted as the first child of the target node.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.ACTION_INSERT_AS_FIRST_CHILD)

### ACTION_INSERT_AS_LAST_CHILD

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ACTION_INSERT_AS_LAST_CHILD

The name of the operation action indicating that the transformation result should be inserted as the last child of the target node.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.ACTION_INSERT_AS_LAST_CHILD)

### CARET_POSITION_PRESERVE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CARET_POSITION_PRESERVE

Constant for the caret position indicating that the same caret position offset should be preserved.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.CARET_POSITION_PRESERVE)

### CARET_POSITION_BEFORE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CARET_POSITION_BEFORE

Constant for the caret position indicating that the caret should be positioned just before the inserted fragment.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.CARET_POSITION_BEFORE)

### CARET_POSITION_START

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CARET_POSITION_START

Constant for the caret position indicating that the caret should be positioned just at the start of the inserted fragment, inside that fragment.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.CARET_POSITION_START)

### CARET_POSITION_EDITABLE

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CARET_POSITION_EDITABLE

Constant for the caret position indicating that the caret should be positioned just at the start of the inserted fragment, in the first editable position.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.CARET_POSITION_EDITABLE)

### CARET_POSITION_END

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CARET_POSITION_END

Constant for the caret position indicating that the caret should be positioned just at the end of the inserted fragment, inside that fragment.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.CARET_POSITION_END)

### CARET_POSITION_AFTER

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CARET_POSITION_AFTER

Constant for the caret position indicating that the caret should be positioned just after the inserted fragment.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.CARET_POSITION_AFTER)

### ARGUMENT_SCRIPT

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_SCRIPT

The XSLT or XQuery script. The value is script.

### ARGUMENT_SCRIPT_PARAMETERS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_SCRIPT_PARAMETERS

External parameters argument. Pairs key=value separated by comma or new line.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.TransformOperation.ARGUMENT_SCRIPT_PARAMETERS)

## Constructor Details

### TransformOperation

public TransformOperation()

Constructor.

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Applies the transformation and executes the specified action with the result.
  Specified by: [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(AuthorAccess, ArgumentsMap)](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### canTreatAsScript

protected boolean canTreatAsScript([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) script)
  Parameters: script - The value of the script parameter. Returns: true if this is an actual script or false if it isn't.
### createTransformer

protected abstract [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createTransformer([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) scriptSrc)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Creates a Transformer from a given script.
  Parameters: authorAccess - Access to different Author resources. scriptSrc - The XSLT or XQuery script. Returns: A JAXP Transformer that will perform the transformation defined in the given script. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)
### createTransformer

protected [Transformer](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Transformer.html) createTransformer([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Source](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/Source.html) scriptSrc, ro.sync.ecss.extensions.commons.operations.ElementLocationPath location)throws [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)

Creates a Transformer from a given script.
  Parameters: authorAccess - Access to different Author resources. scriptSrc - The XSLT or XQuery script. location - The location of the "current" element. Returns: A JAXP Transformer that will perform the transformation defined in the given script. Throws: [TransformerConfigurationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/javax/xml/transform/TransformerConfigurationException.html)
### getArguments

public [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
