# Hierarchy For Package ro.sync.ecss.extensions.dita
 Package Hierarchies:
* [All Packages](../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.api.[AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md), ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md))
        * ro.sync.ecss.extensions.dita.[DITAExternalObjectInsertionHandler](DITAExternalObjectInsertionHandler.md)

    * ro.sync.ecss.extensions.api.[AuthorImageDecorator](../api/AuthorImageDecorator.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md))
        * ro.sync.ecss.extensions.commons.imagemap.[AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md)

            * ro.sync.ecss.extensions.dita.[DITAAuthorImageDecorator](DITAAuthorImageDecorator.md)

    * ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md) (implements ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md))
        * ro.sync.ecss.extensions.dita.[DITASchemaAwareEditingHandler](DITASchemaAwareEditingHandler.md)

    * ro.sync.ecss.extensions.api.table.operations.[AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md)
        * ro.sync.ecss.extensions.dita.[DITAAuthorTableOperationsHandler](DITAAuthorTableOperationsHandler.md)

    * ro.sync.ecss.extensions.commons.[DefaultElementLocatorProvider](../commons/DefaultElementLocatorProvider.md) (implements ro.sync.ecss.extensions.api.link.[ElementLocatorProvider](../api/link/ElementLocatorProvider.md))
        * ro.sync.ecss.extensions.dita.[DITAElementLocatorProvider](DITAElementLocatorProvider.md)

    * ro.sync.ecss.extensions.dita.[DITACustomRuleMatcher](DITACustomRuleMatcher.md) (implements ro.sync.ecss.extensions.api.[DocumentTypeCustomRuleMatcher](../api/DocumentTypeCustomRuleMatcher.md))
    * ro.sync.ecss.extensions.dita.[DITAExternalObjectInsertionHandlerUtil](DITAExternalObjectInsertionHandlerUtil.md)
    * ro.sync.ecss.extensions.dita.[DITASpellCheckerHelper](DITASpellCheckerHelper.md) (implements ro.sync.ecss.extensions.api.spell.[SpellCheckerHelper](../api/spell/SpellCheckerHelper.md))
    * ro.sync.ecss.extensions.dita.[DITAUpdateImageMapOperation.DITANewShapeDescriptor](DITAUpdateImageMapOperation.DITANewShapeDescriptor.md) (implements ro.sync.ecss.extensions.commons.imagemap.operations.[NewShapeDescriptor](../commons/imagemap/operations/NewShapeDescriptor.md))
    * ro.sync.ecss.extensions.dita.[DOTProjectAuthorReferenceResolver](DOTProjectAuthorReferenceResolver.md) (implements ro.sync.ecss.extensions.api.[AuthorReferenceResolver](../api/AuthorReferenceResolver.md))
    * ro.sync.ecss.extensions.commons.imagemap.[EditImageMapCore](../commons/imagemap/EditImageMapCore.md)
        * ro.sync.ecss.extensions.commons.imagemap.[EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)

            * ro.sync.ecss.extensions.dita.[DITAEditImageMapCore](DITAEditImageMapCore.md)

    * ro.sync.ecss.extensions.commons.operations.[EditImageMapOperation](../commons/operations/EditImageMapOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.dita.[EditImageMapOperation](EditImageMapOperation.md)

    * ro.sync.ecss.extensions.api.link.[ElementLocator](../api/link/ElementLocator.md)
        * ro.sync.ecss.extensions.dita.[DITAElementLocator](DITAElementLocator.md)
        * ro.sync.ecss.extensions.dita.[DITAMapKeyDefElementLocator](DITAMapKeyDefElementLocator.md)
        * ro.sync.ecss.extensions.commons.[IDElementLocator](../commons/IDElementLocator.md)

            * ro.sync.ecss.extensions.dita.[DITAIDElementLocator](DITAIDElementLocator.md)

    * ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md))
        * ro.sync.ecss.extensions.dita.[DITAExtensionsBundle](DITAExtensionsBundle.md) (implements ro.sync.ecss.dita.[ContextKeyManagerProvider](../../dita/ContextKeyManagerProvider.md))
            * ro.sync.ecss.extensions.dita.[LWDITAExtensionsBundle](LWDITAExtensionsBundle.md)

        * ro.sync.ecss.extensions.dita.[DITAValExtensionsBundle](DITAValExtensionsBundle.md)
        * ro.sync.ecss.extensions.dita.[DOTProjectExtensionsBundle](DOTProjectExtensionsBundle.md)

    * ro.sync.ecss.extensions.dita.[FindSimilarTopicsOperation](FindSimilarTopicsOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.dita.[InsertKeydefWithKeywordOperation](InsertKeydefWithKeywordOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.commons.operations.[InsertListOperation](../commons/operations/InsertListOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.dita.[DITAInsertListOperation](DITAInsertListOperation.md)

    * ro.sync.contentcompletion.xml.[SchemaManagerFilterBase](../../../contentcompletion/xml/SchemaManagerFilterBase.md) (implements ro.sync.contentcompletion.xml.[SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md))
        * ro.sync.ecss.extensions.dita.[DITASchemaManagerFilter](DITASchemaManagerFilter.md)
        * ro.sync.ecss.extensions.dita.[DITAValSchemaManagerFilter](DITAValSchemaManagerFilter.md)

    * ro.sync.ecss.extensions.dita.[ShowDITAElementDocumentationOperation](ShowDITAElementDocumentationOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.api.text.[TextPageExternalObjectInsertionHandler](../api/text/TextPageExternalObjectInsertionHandler.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md), ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md))
        * ro.sync.ecss.extensions.dita.[DITATextPageExternalObjectInsertionHandler](DITATextPageExternalObjectInsertionHandler.md)

    * ro.sync.ecss.extensions.commons.imagemap.operations.[UpdateImageMapOperationBase](../commons/imagemap/operations/UpdateImageMapOperationBase.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.dita.[DITAUpdateImageMapOperation](DITAUpdateImageMapOperation.md)

    * ro.sync.exml.workspace.api.node.customizer.[XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md))

        * ro.sync.ecss.extensions.dita.[DITANodeRendererCustomizer](DITANodeRendererCustomizer.md)

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.ecss.extensions.dita.[DITANodeRendererCustomizer.DitaClass](DITANodeRendererCustomizer.DitaClass.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
