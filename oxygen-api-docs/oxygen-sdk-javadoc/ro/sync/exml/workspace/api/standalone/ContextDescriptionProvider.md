Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface ContextDescriptionProvider
    All Known Subinterfaces: [InputURLChooser](InputURLChooser.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ContextDescriptionProvider
Provides language-independent information about a certain context.
  Since: 14.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AttributeEditingContextDescription](AttributeEditingContextDescription.md) [getAttributeEditingContextDescription](#getAttributeEditingContextDescription())()
When the chooser is used for editing an attribute value, we can obtain an additional description about the element name and the attribute name which is being edited.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContextDescription](#getContextDescription())()
Get a language-independent description for the dialog in which the CMS action will be provided.

## Method Details

### getContextDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContextDescription()

Get a language-independent description for the dialog in which the CMS action will be provided. Can be null if no such description is available.
  Returns: a language-independent description for the dialog in which the CMS action will be provided. Can be null if no such description is available.
### getAttributeEditingContextDescription

[AttributeEditingContextDescription](AttributeEditingContextDescription.md) getAttributeEditingContextDescription()

When the chooser is used for editing an attribute value, we can obtain an additional description about the element name and the attribute name which is being edited.
  Returns: an additional description about the element name and the attribute name which is being edited. Can be null if the editing context is not called when editing an attribute value. Since: 15
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
