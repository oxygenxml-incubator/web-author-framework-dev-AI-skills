Package [com.oxygenxml.editor.editors](package-summary.md)

# Interface IDropDownMenuAction
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface IDropDownMenuAction
Adds the possibility to add a drop down menu customizer.
  Since: 17
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addMenuCustomizer](#addMenuCustomizer(com.oxygenxml.editor.editors.IDropDownMenuCustomizer))([IDropDownMenuCustomizer](IDropDownMenuCustomizer.md) customizer)
Add a customizer to customize the drop down menu before it gets shown.
  void [removeMenuCustomizer](#removeMenuCustomizer(com.oxygenxml.editor.editors.IDropDownMenuCustomizer))([IDropDownMenuCustomizer](IDropDownMenuCustomizer.md) customizer)
Remove a customizer.

## Method Details

### addMenuCustomizer

void addMenuCustomizer([IDropDownMenuCustomizer](IDropDownMenuCustomizer.md) customizer)

Add a customizer to customize the drop down menu before it gets shown.
  Parameters: customizer - The drop down menu customizer.
### removeMenuCustomizer

void removeMenuCustomizer([IDropDownMenuCustomizer](IDropDownMenuCustomizer.md) customizer)

Remove a customizer.
  Parameters: customizer - The drop down menu customizer.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
