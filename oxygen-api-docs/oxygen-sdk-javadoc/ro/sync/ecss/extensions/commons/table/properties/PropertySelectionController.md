Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Interface PropertySelectionController
    All Known Implementing Classes: [ECPropertiesComposite](ECPropertiesComposite.md)   @API(type=INTERNAL, src=PUBLIC) public interface PropertySelectionController
Used for handling with a change of the properties values.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [selectionChanged](#selectionChanged(ro.sync.ecss.extensions.commons.table.properties.TableProperty,java.lang.String))([TableProperty](TableProperty.md) property, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)
Method which controls the change of the selected key.

## Method Details

### selectionChanged

void selectionChanged([TableProperty](TableProperty.md) property, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)throws [AuthorOperationException](../../../api/AuthorOperationException.md)

Method which controls the change of the selected key.
  Parameters: property - The modified property. newValue - The new selected value of the given property Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the handling of selection changed cannot be performed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
