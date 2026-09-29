Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface ClassPathResourcesAccess
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ClassPathResourcesAccess
Provides access to all URLs which were added in the classpath for the specific framework when the document type was edited from the Oxygen preferences.
  Since: 12.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] [getClassPathResources](#getClassPathResources())()
Get the list of resources the user has added to the classpath of the corresponding framework

## Method Details

### getClassPathResources

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)[] getClassPathResources()

Get the list of resources the user has added to the classpath of the corresponding framework
  Returns: the list of resources the user has added to the classpath of the corresponding framework Since: 12.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
