Package [ro.sync.ecss.extensions.commons.imagemap.operations](package-summary.md)

# Class UpdateImageMapOperationBase

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.imagemap.operations.UpdateImageMapOperationBase
   All Implemented Interfaces: [AuthorOperation](../../../api/AuthorOperation.md), [Extension](../../../api/Extension.md)   Direct Known Subclasses: [DITAUpdateImageMapOperation](../../../dita/DITAUpdateImageMapOperation.md), [XHTMLUpdateImageMapOperation](../../../xhtml/imagemap/XHTMLUpdateImageMapOperation.md)   @API(type=EXTENDABLE, src=PUBLIC) public abstract class UpdateImageMapOperationBase extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorOperation](../../../api/AuthorOperation.md)
Updates an image map with shape information from an SVG.
  Since: 25.0
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ARGUMENT_SHAPES](#ARGUMENT_SHAPES)
An SVG with the shapes to be used to update the Image Map at caret.
  protected static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [ARGUMENTS](#ARGUMENTS)
The arguments descriptor.

### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [UpdateImageMapOperationBase](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)
Perform the actual operation.
  [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] [getArguments](#getArguments())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()

 protected abstract [AuthorElement](../../../api/node/AuthorElement.md)[] [getExistingShapesList](#getExistingShapesList(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) existingImageMap)
Return the list of existing shapes starting from the existing Image Map.
  protected abstract [AuthorElement](../../../api/node/AuthorElement.md) [getImageMapElement](#getImageMapElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../api/node/AuthorElement.md) currentElement)
Return the image map that contains the current element.
  protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [NewShapeDescriptor](NewShapeDescriptor.md)> [getNewShapesList](#getNewShapesList(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) svgText)
Return the list of new shapes descriptors.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### ARGUMENT_SHAPES

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ARGUMENT_SHAPES

An SVG with the shapes to be used to update the Image Map at caret.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.imagemap.operations.UpdateImageMapOperationBase.ARGUMENT_SHAPES)

### ARGUMENTS

protected static final [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] ARGUMENTS

The arguments descriptor.

## Constructor Details

### UpdateImageMapOperationBase

public UpdateImageMapOperationBase()

## Method Details

### getDescription

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()
  Specified by: [getDescription](../../../api/Extension.md#getDescription()) in interface [Extension](../../../api/Extension.md) Returns: The description of the extension. See Also:
        * [Extension.getDescription()](../../../api/Extension.md#getDescription())

### doOperation

public void doOperation([AuthorAccess](../../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../../api/AuthorOperation.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getImageMapElement

protected abstract [AuthorElement](../../../api/node/AuthorElement.md) getImageMapElement([AuthorElement](../../../api/node/AuthorElement.md) currentElement)

Return the image map that contains the current element.
  Parameters: currentElement - The current element. Returns: The image map element.
### getNewShapesList

protected abstract [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [NewShapeDescriptor](NewShapeDescriptor.md)> getNewShapesList([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) svgText)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Return the list of new shapes descriptors.
  Parameters: svgText - The SVG text. Returns: The list. Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - If the conversion fails.
### getExistingShapesList

protected abstract [AuthorElement](../../../api/node/AuthorElement.md)[] getExistingShapesList([AuthorElement](../../../api/node/AuthorElement.md) existingImageMap)

Return the list of existing shapes starting from the existing Image Map.
  Parameters: existingImageMap - The existing Image Map. Returns: The array of elements that correspond to shapes.
### getArguments

public [ArgumentDescriptor](../../../api/ArgumentDescriptor.md)[] getArguments()
  Specified by: [getArguments](../../../api/AuthorOperation.md#getArguments()) in interface [AuthorOperation](../../../api/AuthorOperation.md) Returns: An array of [ArgumentDescriptor](../../../api/ArgumentDescriptor.md) representing the arguments this operation uses. See Also:
        * [AuthorOperation.getArguments()](../../../api/AuthorOperation.md#getArguments())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
