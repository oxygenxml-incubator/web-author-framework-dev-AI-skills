Package [ro.sync.ecss.extensions.api.webapp.references](package-summary.md)

# Class WebappReferenceCollectorFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.references.WebappReferenceCollectorFactory
   All Implemented Interfaces: [ReferenceCollectorFactory](../../../../../exml/workspace/api/references/ReferenceCollectorFactory.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class WebappReferenceCollectorFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ReferenceCollectorFactory](../../../../../exml/workspace/api/references/ReferenceCollectorFactory.md)
Contains methods to create a reference collector for the webapp component

## Constructor Summary
 Constructors
Constructor

Description
 [WebappReferenceCollectorFactory](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md) [createCollector](#createCollector(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Creates a reference collector that has additional extractors
  static [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md) [createCollector](#createCollector(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([AuthorDocumentModel](../AuthorDocumentModel.md) model)
Creates a reference collector with additional extractors from a document model

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WebappReferenceCollectorFactory

public WebappReferenceCollectorFactory()

## Method Details

### createCollector

public [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md) createCollector([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Creates a reference collector that has additional extractors
  Specified by: [createCollector](../../../../../exml/workspace/api/references/ReferenceCollectorFactory.md#createCollector(java.net.URL)) in interface [ReferenceCollectorFactory](../../../../../exml/workspace/api/references/ReferenceCollectorFactory.md) Parameters: url - the URL of the XML document Returns: the reference collector See Also:
        * [ReferenceCollectorFactory.createCollector(java.net.URL)](../../../../../exml/workspace/api/references/ReferenceCollectorFactory.md#createCollector(java.net.URL))

### createCollector

public static [ReferenceCollector](../../../../../exml/workspace/api/references/ReferenceCollector.md) createCollector([AuthorDocumentModel](../AuthorDocumentModel.md) model)

Creates a reference collector with additional extractors from a document model
  Parameters: model - the document model Returns: the reference collector
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
