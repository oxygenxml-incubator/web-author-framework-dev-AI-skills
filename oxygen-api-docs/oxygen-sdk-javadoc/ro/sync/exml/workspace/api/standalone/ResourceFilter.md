Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface ResourceFilter
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ResourceFilter
Resource filter returned by the InputURLCustomizer.
  Since: 13
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Get the description of this filter.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getExtensions](#getExtensions())()
Get the list of extensions.

## Method Details

### getExtensions

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getExtensions()

Get the list of extensions. Example: "dita", "ditamap", "bookmap", "ditaval".
  Returns: Returns the extensions.
### getDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Get the description of this filter.
  Returns: The description of this filter.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
