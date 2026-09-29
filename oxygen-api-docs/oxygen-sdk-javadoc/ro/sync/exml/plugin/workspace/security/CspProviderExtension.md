Package [ro.sync.exml.plugin.workspace.security](package-summary.md)

# Interface CspProviderExtension
    All Superinterfaces: [PluginExtension](../../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface CspProviderExtensionextends [PluginExtension](../../PluginExtension.md)
Extension that can be used by plugins to contribute to the Content-Security-Policy header.
  Since: 26.1.1  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[CspDirective](CspDirective.md),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> [getAdditionalCspConfiguration](#getAdditionalCspConfiguration())()
Method used to provide the additional CSP configuration.

## Method Details

### getAdditionalCspConfiguration

[Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[CspDirective](CspDirective.md),[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)>> getAdditionalCspConfiguration()

Method used to provide the additional CSP configuration.
  Returns: A map from [CspDirective](CspDirective.md) to the values to be added to that directive.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
