Package [ro.sync.ecss.extensions.commons.operations](package-summary.md)

# Class InsertFragmentOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.operations.InsertFragmentOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   Direct Known Subclasses: [InsertOrReplaceFragmentOperation](InsertOrReplaceFragmentOperation.md)   @API(type=INTERNAL, src=PUBLIC) public class InsertFragmentOperation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../api/AuthorOperation.md)
An implementation of an insert operation for an argument of type fragment.

## Field Summary
 Fields
Modifier and Type

Field

Description
 protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) [ARGUMENT_DESCR_INSERT_FRAG_EVEN_IF_INVALID](#ARGUMENT_DESCR_INSERT_FRAG_EVEN_IF_INVALID)
Argument descriptor.
  protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) [ARGUMENT_DESCRIPTOR_FRAGMENT](#ARGUMENT_DESCRIPTOR_FRAGMENT)
Argument defining the XML fragment that will be inserted.
  protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) [ARGUMENT_DESCRIPTOR_GO_TO_NEXT_EDITABLE_POSITION](#ARGUMENT_DESCRIPTOR_GO_TO_NEXT_EDITABLE_POSITION)
Argument defining if the fragment insertion is schema aware.
  protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) [ARGUMENT_DESCRIPTOR_RELATIVE_LOCATION](#ARGUMENT_DESCRIPTOR_RELATIVE_LOCATION)
Argument defining the relative position to the node obtained from the XPath location.
  protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) [ARGUMENT_DESCRIPTOR_XPATH_LOCATION](#ARGUMENT_DESCRIPTOR_XPATH_LOCATION)
Argument defining the location where the operation will be executed as an XPath expression.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_FRAGMENT](#ARGUMENT_FRAGMENT)
The fragment argument.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_GO_TO_NEXT_EDITABLE_POSITION](#ARGUMENT_GO_TO_NEXT_EDITABLE_POSITION)
Detect and position the caret inside the first edit location.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_INSERT_FRAG_EVEN_IF_INVALID](#ARGUMENT_INSERT_FRAG_EVEN_IF_INVALID)
true to insert the fragment even if invalid.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_RELATIVE_LOCATION](#ARGUMENT_RELATIVE_LOCATION)
The insert position argument.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_XPATH_LOCATION](#ARGUMENT_XPATH_LOCATION)
The insert location argument.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [InsertFragmentOperation](#%3Cinit%3E())()
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)
Perform the actual operation.
  protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Object,java.lang.Object,java.lang.Object,boolean,java.lang.Object))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) fragment, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) xpathLocation, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) relativeLocation, boolean goToFirstEditablePosition, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) schemaAwareArgumentValue)
Performs the insert operation.
  protected void [doOperationInternal](#doOperationInternal(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.Object,java.lang.Object,java.lang.Object,boolean,java.lang.Object,boolean))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) fragment, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) xpathLocation, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) relativeLocation, boolean goToFirstEditablePosition, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) schemaAwareArgumentValue, boolean isInsertEvenIfInvalid)
Performs the insert operation.
  [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### ARGUMENT_FRAGMENT

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_FRAGMENT

The fragment argument. The value is fragment.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.InsertFragmentOperation.ARGUMENT_FRAGMENT)

### ARGUMENT_DESCRIPTOR_FRAGMENT

protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) ARGUMENT_DESCRIPTOR_FRAGMENT

Argument defining the XML fragment that will be inserted.

### ARGUMENT_XPATH_LOCATION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_XPATH_LOCATION

The insert location argument. The value is insertLocation.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.InsertFragmentOperation.ARGUMENT_XPATH_LOCATION)

### ARGUMENT_DESCRIPTOR_XPATH_LOCATION

protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) ARGUMENT_DESCRIPTOR_XPATH_LOCATION

Argument defining the location where the operation will be executed as an XPath expression.

### ARGUMENT_RELATIVE_LOCATION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_RELATIVE_LOCATION

The insert position argument. The value is insertPosition.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.InsertFragmentOperation.ARGUMENT_RELATIVE_LOCATION)

### ARGUMENT_DESCRIPTOR_RELATIVE_LOCATION

protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) ARGUMENT_DESCRIPTOR_RELATIVE_LOCATION

Argument defining the relative position to the node obtained from the XPath location.

### ARGUMENT_GO_TO_NEXT_EDITABLE_POSITION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_GO_TO_NEXT_EDITABLE_POSITION

Detect and position the caret inside the first edit location. It can be either an offset inside the content or an in-place editor.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.InsertFragmentOperation.ARGUMENT_GO_TO_NEXT_EDITABLE_POSITION)

### ARGUMENT_DESCRIPTOR_GO_TO_NEXT_EDITABLE_POSITION

protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) ARGUMENT_DESCRIPTOR_GO_TO_NEXT_EDITABLE_POSITION

Argument defining if the fragment insertion is schema aware.

### ARGUMENT_INSERT_FRAG_EVEN_IF_INVALID

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_INSERT_FRAG_EVEN_IF_INVALID

true to insert the fragment even if invalid.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.operations.InsertFragmentOperation.ARGUMENT_INSERT_FRAG_EVEN_IF_INVALID)

### ARGUMENT_DESCR_INSERT_FRAG_EVEN_IF_INVALID

protected static final [ArgumentDescriptor](../../api/ArgumentDescriptor.md) ARGUMENT_DESCR_INSERT_FRAG_EVEN_IF_INVALID

Argument descriptor.

## Constructor Details

### InsertFragmentOperation

public InsertFragmentOperation()

Constructor.

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(AuthorAccess, ArgumentsMap)](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) fragment, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) xpathLocation, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) relativeLocation, boolean goToFirstEditablePosition, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) schemaAwareArgumentValue)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Performs the insert operation.
  Parameters: authorAccess - The author access used to access the document. fragment - The fragment to be inserted. xpathLocation - The XPath location where the insertion takes place. If null, insert at caret position. relativeLocation - The location of the insertion relative to the node selected by the XPath. goToFirstEditablePosition - true if we should go to the first editable position in the fragment after insertion. schemaAwareArgumentValue - true if the insertion should be schema aware. Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### doOperationInternal

protected void doOperationInternal([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) fragment, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) xpathLocation, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) relativeLocation, boolean goToFirstEditablePosition, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) schemaAwareArgumentValue, boolean isInsertEvenIfInvalid)throws [AuthorOperationException](../../api/AuthorOperationException.md)

Performs the insert operation.
  Parameters: authorAccess - The author access used to access the document. fragment - The fragment to be inserted. xpathLocation - The XPath location where the insertion takes place. If null, insert at caret position. relativeLocation - The location of the insertion relative to the node selected by the XPath. goToFirstEditablePosition - true if we should go to the first editable position in the fragment after insertion. schemaAwareArgumentValue - true if the insertion should be schema aware. isInsertEvenIfInvalid - true to insert the fragment even if it would make the document invalid. Throws: [AuthorOperationException](../../api/AuthorOperationException.md)
### getArguments

public [ArgumentDescriptor](../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments())

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../api/Extension.md#getDescription()) in interface [Extension](../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../api/Extension.md#getDescription())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
