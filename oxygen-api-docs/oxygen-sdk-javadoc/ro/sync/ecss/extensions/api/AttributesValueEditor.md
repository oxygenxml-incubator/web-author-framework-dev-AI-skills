Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AttributesValueEditor
    @API(type=EXTENDABLE, src=PUBLIC) public interface AttributesValueEditor Deprecated.
Starting with version 15 the [CustomAttributeValueEditor](CustomAttributeValueEditor.md) can be used instead to edit only specific attributes using a custom editor.

Editor for attribute values.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttributeValue](#getAttributeValue(ro.sync.ecss.extensions.api.EditedAttribute,java.lang.Object))([EditedAttribute](EditedAttribute.md) attribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentComponent)  Deprecated.
Get a value for the current attribute.

## Method Details

### getAttributeValue

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttributeValue([EditedAttribute](EditedAttribute.md) attribute, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) parentComponent)
 Deprecated.
Get a value for the current attribute.
  Parameters: attribute - The attribute to be edited. parentComponent - The parent component. Used as parent when creating dialogs. Returns: The proposed value.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
