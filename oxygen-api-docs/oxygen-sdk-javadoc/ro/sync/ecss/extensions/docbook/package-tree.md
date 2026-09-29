# Hierarchy For Package ro.sync.ecss.extensions.docbook
 Package Hierarchies:
* [All Packages](../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.api.[AuthorExternalObjectInsertionHandler](../api/AuthorExternalObjectInsertionHandler.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md), ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../api/ExternalObjectInsertionSources.md))
        * ro.sync.ecss.extensions.docbook.[Docbook4ExternalObjectInsertionHandler](Docbook4ExternalObjectInsertionHandler.md)
        * ro.sync.ecss.extensions.docbook.[Docbook5ExternalObjectInsertionHandler](Docbook5ExternalObjectInsertionHandler.md)

    * ro.sync.ecss.extensions.api.[AuthorImageDecorator](../api/AuthorImageDecorator.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md))
        * ro.sync.ecss.extensions.commons.imagemap.[AuthorImageMapDecorator](../commons/imagemap/AuthorImageMapDecorator.md)

            * ro.sync.ecss.extensions.docbook.[DocbookAuthorImageDecorator](DocbookAuthorImageDecorator.md)

    * ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter](../api/AuthorSchemaAwareEditingHandlerAdapter.md) (implements ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](../api/AuthorSchemaAwareEditingHandler.md))
        * ro.sync.ecss.extensions.docbook.[DocbookSchemaAwareEditingHandler](DocbookSchemaAwareEditingHandler.md)

            * ro.sync.ecss.extensions.docbook.[Docbook5SchemaAwareEditingHandler](Docbook5SchemaAwareEditingHandler.md)

    * ro.sync.ecss.extensions.api.table.operations.[AuthorTableOperationsHandler](../api/table/operations/AuthorTableOperationsHandler.md)
        * ro.sync.ecss.extensions.docbook.[DocbookAuthorTableOperationsHandler](DocbookAuthorTableOperationsHandler.md)

    * ro.sync.ecss.extensions.docbook.[Docbook4PasteAsLinkOperation](Docbook4PasteAsLinkOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[Docbook4PasteAsXIncludeOperation](Docbook4PasteAsXIncludeOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[Docbook4PasteAsXrefOperation](Docbook4PasteAsXrefOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[Docbook5PasteAsLinkOperation](Docbook5PasteAsLinkOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[Docbook5PasteAsXIncludeOperation](Docbook5PasteAsXIncludeOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[Docbook5PasteAsXrefOperation](Docbook5PasteAsXrefOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.commons.imagemap.[EditImageMapCore](../commons/imagemap/EditImageMapCore.md)
        * ro.sync.ecss.extensions.commons.imagemap.[EditImageMapWithSurroundCore](../commons/imagemap/EditImageMapWithSurroundCore.md)

            * ro.sync.ecss.extensions.docbook.[DocbookEditImageMapCore](DocbookEditImageMapCore.md)

    * ro.sync.ecss.extensions.commons.operations.[EditImageMapOperation](../commons/operations/EditImageMapOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.docbook.[EditImageMapOperation](EditImageMapOperation.md)

    * ro.sync.ecss.extensions.api.[ExtensionsBundle](../api/ExtensionsBundle.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md))
        * ro.sync.ecss.extensions.docbook.[DocBookExtensionsBundleBase](DocBookExtensionsBundleBase.md)

            * ro.sync.ecss.extensions.docbook.[DocBook4ExtensionsBundle](DocBook4ExtensionsBundle.md)
            * ro.sync.ecss.extensions.docbook.[DocBook5ExtensionsBundle](DocBook5ExtensionsBundle.md)

    * ro.sync.ecss.extensions.commons.operations.[InsertEquationOperation](../commons/operations/InsertEquationOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.docbook.[InsertEquationOperation](InsertEquationOperation.md)

    * ro.sync.ecss.extensions.docbook.[InsertGraphicOperation](InsertGraphicOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[InsertGUIButtonOperation](InsertGUIButtonOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[InsertImageDataOperation](InsertImageDataOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.commons.operations.[InsertListOperation](../commons/operations/InsertListOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.docbook.[DocbookInsertListOperation](DocbookInsertListOperation.md)

            * ro.sync.ecss.extensions.docbook.[DB4InsertListOperation](DB4InsertListOperation.md)
            * ro.sync.ecss.extensions.docbook.[DB5InsertListOperation](DB5InsertListOperation.md)

    * ro.sync.ecss.extensions.docbook.[InsertMediaDataOperationBase](InsertMediaDataOperationBase.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
        * ro.sync.ecss.extensions.docbook.[Docbook4InsertMediaDataOperation](Docbook4InsertMediaDataOperation.md)
        * ro.sync.ecss.extensions.docbook.[Docbook5InsertMediaDataOperation](Docbook5InsertMediaDataOperation.md)

    * ro.sync.ecss.extensions.docbook.[InsertScreenshotOperation](InsertScreenshotOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[PromoteDemoteSectionOperation](PromoteDemoteSectionOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.docbook.[PromoteDemoteSectionUtil](PromoteDemoteSectionUtil.md)
    * ro.sync.contentcompletion.xml.[SchemaManagerFilterBase](../../../contentcompletion/xml/SchemaManagerFilterBase.md) (implements ro.sync.contentcompletion.xml.[SchemaManagerFilter](../../../contentcompletion/xml/SchemaManagerFilter.md))
        * ro.sync.ecss.extensions.docbook.[DocbookSchemaManagerFilter](DocbookSchemaManagerFilter.md)

    * ro.sync.exml.workspace.api.node.customizer.[XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md))

        * ro.sync.ecss.extensions.docbook.[DocbookNodeRendererCustomizer](DocbookNodeRendererCustomizer.md)

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.ecss.extensions.docbook.[PromoteDemoteSectionUtil.PromoteDemote](PromoteDemoteSectionUtil.PromoteDemote.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
