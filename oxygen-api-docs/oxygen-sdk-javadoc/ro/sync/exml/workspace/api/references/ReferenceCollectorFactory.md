Package [ro.sync.exml.workspace.api.references](package-summary.md)

# Interface ReferenceCollectorFactory
    All Known Implementing Classes: [WebappReferenceCollectorFactory](../../../../ecss/extensions/api/webapp/references/WebappReferenceCollectorFactory.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ReferenceCollectorFactory
Factory that creates ReferenceCollector objects to collect references from an XML document at specified URL.
  Since: 21.1
## Method Summary
  All MethodsStatic MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [ReferenceCollector](ReferenceCollector.md) [createCollector](#createCollector(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Creates a ReferenceCollector for the given URL.
  static [ReferenceCollector](ReferenceCollector.md) [getCollector](#getCollector(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Convenience method that returns a collector for the given URL.

## Method Details

### createCollector

[ReferenceCollector](ReferenceCollector.md) createCollector([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Creates a ReferenceCollector for the given URL.
  Parameters: url - the URL of the document Returns: the created ReferenceCollector instance
### getCollector

static [ReferenceCollector](ReferenceCollector.md) getCollector([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Convenience method that returns a collector for the given URL. It searches the StaticComponentsRegistry registry for registered factory to create the new collector. If none found it returns the default implementation.
  Parameters: url - the URL of the XML document Returns: the reference collector
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
