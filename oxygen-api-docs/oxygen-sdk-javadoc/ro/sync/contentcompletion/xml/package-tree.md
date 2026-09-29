# Hierarchy For Package ro.sync.contentcompletion.xml
 Package Hierarchies:
* [All Packages](../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.contentcompletion.xml.[CIAttribute](CIAttribute.md) (implements java.lang.[Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, ro.sync.contentcompletion.xml.[NodeDescription](NodeDescription.md))
    * ro.sync.contentcompletion.xml.[CIElementAdapter](CIElementAdapter.md) (implements ro.sync.contentcompletion.xml.[CIElement](CIElement.md))
    * ro.sync.contentcompletion.xml.[CIValue](CIValue.md) (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>)
    * ro.sync.contentcompletion.xml.[Context](Context.md) (implements java.lang.[Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html))
        * ro.sync.contentcompletion.xml.WhatContextInParent
            * ro.sync.contentcompletion.xml.[WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md)
            * ro.sync.contentcompletion.xml.[WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md)

        * ro.sync.contentcompletion.xml.[WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md)

    * ro.sync.contentcompletion.xml.[ContextElement](ContextElement.md) (implements java.lang.[Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html))
    * ro.sync.contentcompletion.xml.[NameValue](NameValue.md)
        * ro.sync.contentcompletion.xml.[ExternalEntityNameValue](ExternalEntityNameValue.md)

    * ro.sync.contentcompletion.xml.[SchemaManagerFilterBase](SchemaManagerFilterBase.md) (implements ro.sync.contentcompletion.xml.[SchemaManagerFilter](SchemaManagerFilter.md))

        * ro.sync.contentcompletion.xml.[StyleGuideSchemaManagerFilterBase](StyleGuideSchemaManagerFilterBase.md)

## Interface Hierarchy

* ro.sync.contentcompletion.xml.[CIAttribute.DefaultValueProvider](CIAttribute.DefaultValueProvider.md)
* java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>
    * ro.sync.contentcompletion.xml.[CIElement](CIElement.md) (also extends ro.sync.contentcompletion.xml.[NodeDescription](NodeDescription.md))

* ro.sync.ecss.extensions.api.[Extension](../../ecss/extensions/api/Extension.md)
    * ro.sync.contentcompletion.xml.[SchemaManagerFilter](SchemaManagerFilter.md)

* ro.sync.contentcompletion.xml.[NodeDescription](NodeDescription.md)

    * ro.sync.contentcompletion.xml.[CIElement](CIElement.md) (also extends java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>)

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.contentcompletion.xml.[CIAttribute.EditableState](CIAttribute.EditableState.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
