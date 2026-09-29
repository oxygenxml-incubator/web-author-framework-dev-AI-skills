Package [ro.sync.ecss.extensions.xhtml.imagemap](package-summary.md)

# Class XHTMLUpdateImageMapOperation

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.imagemap.operations.UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md)
        * ro.sync.ecss.extensions.xhtml.imagemap.XHTMLUpdateImageMapOperation
   All Implemented Interfaces: [AuthorOperation](../../api/AuthorOperation.md), [Extension](../../api/Extension.md)   @API(type=INTERNAL, src=PUBLIC) public class XHTMLUpdateImageMapOperation extends [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md)
XHTML implementation of the operation that updates an image map with shape information from an SVG.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static class  [XHTMLUpdateImageMapOperation.XHTMLNewShapeDescriptor](XHTMLUpdateImageMapOperation.XHTMLNewShapeDescriptor.md)
Descriptor of a shape that was added client-side.

## Field Summary

### Fields inherited from class ro.sync.ecss.extensions.commons.imagemap.operations.[UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md)
 [ARGUMENT_SHAPES](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#ARGUMENT_SHAPES), [ARGUMENTS](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#ARGUMENTS)
### Fields inherited from interface ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md)
 [NAMESPACE_ARGUMENT](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT), [NAMESPACE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#NAMESPACE_ARGUMENT_DESCRIPTOR), [SCHEMA_AWARE_ARGUMENT](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT), [SCHEMA_AWARE_ARGUMENT_DESCRIPTOR](../../api/AuthorOperation.md#SCHEMA_AWARE_ARGUMENT_DESCRIPTOR)
## Constructor Summary
 Constructors
Constructor

Description
 [XHTMLUpdateImageMapOperation](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [doOperation](#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)
Perform the actual operation.
  protected [AuthorElement](../../api/node/AuthorElement.md)[] [getExistingShapesList](#getExistingShapesList(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) existingImageMap)
Return the list of existing shapes starting from the existing Image Map.
  protected [AuthorElement](../../api/node/AuthorElement.md) [getImageMapElement](#getImageMapElement(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../api/node/AuthorElement.md) currentElement)
Return the image map that contains the current element.
  protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [NewShapeDescriptor](../../commons/imagemap/operations/NewShapeDescriptor.md)> [getNewShapesList](#getNewShapesList(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) svgText)
Return the list of new shapes descriptors.

### Methods inherited from class ro.sync.ecss.extensions.commons.imagemap.operations.[UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md)
 [getArguments](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getArguments()), [getDescription](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getDescription())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### XHTMLUpdateImageMapOperation

public XHTMLUpdateImageMapOperation()

## Method Details

### doOperation

public void doOperation([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [ArgumentsMap](../../api/ArgumentsMap.md) args)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from interface: [AuthorOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))
Perform the actual operation. You can check if the operation was invoked from the oXygen standalone application or from the oXygen plugin for Eclipse by using the method: [ApplicationInformationAccess.getPlatform()](../../../../exml/workspace/api/application/ApplicationInformationAccess.md#getPlatform()). To get to the [Workspace](../../../../exml/workspace/api/Workspace.md) you may use: [AuthorAccess.getWorkspaceAccess()](../../api/AuthorAccess.md#getWorkspaceAccess()).
  Specified by: [doOperation](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in interface [AuthorOperation](../../api/AuthorOperation.md) Overrides: [doOperation](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap)) in class [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md) Parameters: authorAccess - The author access. Provides access to specific informations and actions for editor, document, workspace, tables, change tracking, utility a.s.o. args - The map of arguments. All the arguments defined by method [AuthorOperation.getArguments()](../../api/AuthorOperation.md#getArguments()) must be present in the map of arguments. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - Thrown when the operation fails. See Also:
        * [AuthorOperation.doOperation(ro.sync.ecss.extensions.api.AuthorAccess, ro.sync.ecss.extensions.api.ArgumentsMap)](../../api/AuthorOperation.md#doOperation(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.ArgumentsMap))

### getNewShapesList

protected [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<? extends [NewShapeDescriptor](../../commons/imagemap/operations/NewShapeDescriptor.md)> getNewShapesList([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) svgText)throws [AuthorOperationException](../../api/AuthorOperationException.md)
 Description copied from class: [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getNewShapesList(java.lang.String))
Return the list of new shapes descriptors.
  Specified by: [getNewShapesList](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getNewShapesList(java.lang.String)) in class [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md) Parameters: svgText - The SVG text. Returns: The list. Throws: [AuthorOperationException](../../api/AuthorOperationException.md) - If the conversion fails. See Also:
        * [UpdateImageMapOperationBase.getNewShapesList(java.lang.String)](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getNewShapesList(java.lang.String))

### getExistingShapesList

protected [AuthorElement](../../api/node/AuthorElement.md)[] getExistingShapesList([AuthorElement](../../api/node/AuthorElement.md) existingImageMap)
 Description copied from class: [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getExistingShapesList(ro.sync.ecss.extensions.api.node.AuthorElement))
Return the list of existing shapes starting from the existing Image Map.
  Specified by: [getExistingShapesList](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getExistingShapesList(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md) Parameters: existingImageMap - The existing Image Map. Returns: The array of elements that correspond to shapes. See Also:
        * [UpdateImageMapOperationBase.getExistingShapesList(ro.sync.ecss.extensions.api.node.AuthorElement)](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getExistingShapesList(ro.sync.ecss.extensions.api.node.AuthorElement))

### getImageMapElement

protected [AuthorElement](../../api/node/AuthorElement.md) getImageMapElement([AuthorElement](../../api/node/AuthorElement.md) currentElement)
 Description copied from class: [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getImageMapElement(ro.sync.ecss.extensions.api.node.AuthorElement))
Return the image map that contains the current element.
  Specified by: [getImageMapElement](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getImageMapElement(ro.sync.ecss.extensions.api.node.AuthorElement)) in class [UpdateImageMapOperationBase](../../commons/imagemap/operations/UpdateImageMapOperationBase.md) Parameters: currentElement - The current element. Returns: The image map element. See Also:
        * [UpdateImageMapOperationBase.getImageMapElement(ro.sync.ecss.extensions.api.node.AuthorElement)](../../commons/imagemap/operations/UpdateImageMapOperationBase.md#getImageMapElement(ro.sync.ecss.extensions.api.node.AuthorElement))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
