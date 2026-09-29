Package [ro.sync.exml.workspace.api.templates](package-summary.md)

# Interface TemplatesCategory
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TemplatesCategory
A template category...
  Since: 18
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAdditionalInformation](#getAdditionalInformation())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TemplatesCategory](TemplatesCategory.md)> [getChildCategories](#getChildCategories())()
Get the subcategories.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFrameworkId](#getFrameworkId())()
Get the corresponding framework id.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Get the name of the category.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[EditorTemplate](../../../editor/EditorTemplate.md)> [getTemplates](#getTemplates())()
Get the templates list for this category.

## Method Details

### getAdditionalInformation

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAdditionalInformation()
  Returns: The additional information for the category. It can be the absolute path of the folder associated with the category or the store location of the framework this category was created for.
### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Get the name of the category.
  Returns: Returns the name of the category.
### getChildCategories

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TemplatesCategory](TemplatesCategory.md)> getChildCategories()

Get the subcategories.
  Returns: Returns the subcategories.
### getTemplates

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[EditorTemplate](../../../editor/EditorTemplate.md)> getTemplates()

Get the templates list for this category.
  Returns: The templates list strictly in this category.
### getFrameworkId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFrameworkId()

Get the corresponding framework id.
  Returns: Framework id or null for templates that aren't from a framework. Since: 20.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
