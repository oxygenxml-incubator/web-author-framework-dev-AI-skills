# Hierarchy For Package ro.sync.ecss.extensions.dita.map
 Package Hierarchies:
* [All Packages](../../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.api.[AuthorExternalObjectInsertionHandler](../../api/AuthorExternalObjectInsertionHandler.md) (implements ro.sync.ecss.extensions.api.[Extension](../../api/Extension.md), ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../../api/ExternalObjectInsertionSources.md))
        * ro.sync.ecss.extensions.dita.[DITAExternalObjectInsertionHandler](../DITAExternalObjectInsertionHandler.md)

            * ro.sync.ecss.extensions.dita.map.[DITAMapExternalObjectInsertionHandler](DITAMapExternalObjectInsertionHandler.md)

    * ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter](../../api/AuthorSchemaAwareEditingHandlerAdapter.md) (implements ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](../../api/AuthorSchemaAwareEditingHandler.md))
        * ro.sync.ecss.extensions.dita.[DITASchemaAwareEditingHandler](../DITASchemaAwareEditingHandler.md)

            * ro.sync.ecss.extensions.dita.map.[DITAMapSchemaAwareEditingHandler](DITAMapSchemaAwareEditingHandler.md)

    * ro.sync.ecss.extensions.api.table.operations.[AuthorTableOperationsHandler](../../api/table/operations/AuthorTableOperationsHandler.md)
        * ro.sync.ecss.extensions.dita.map.[DITAMapAuthorTableOperationsHandler](DITAMapAuthorTableOperationsHandler.md)

    * ro.sync.ecss.extensions.dita.[DITACustomRuleMatcher](../DITACustomRuleMatcher.md) (implements ro.sync.ecss.extensions.api.[DocumentTypeCustomRuleMatcher](../../api/DocumentTypeCustomRuleMatcher.md))
        * ro.sync.ecss.extensions.dita.map.[DITAMapCustomRuleMatcher](DITAMapCustomRuleMatcher.md)

            * ro.sync.ecss.extensions.dita.map.[DITAMap2_xCustomRuleMatcher](DITAMap2_xCustomRuleMatcher.md)

    * ro.sync.ecss.extensions.dita.map.[DITAMapTopicTitlesResolveListener](DITAMapTopicTitlesResolveListener.md) (implements ro.sync.ecss.extensions.api.[AuthorExtensionStateListener](../../api/AuthorExtensionStateListener.md))
    * ro.sync.ecss.extensions.api.[DocumentTypeAdvancedCustomRuleMatcher](../../api/DocumentTypeAdvancedCustomRuleMatcher.md) (implements ro.sync.ecss.extensions.api.[DocumentTypeCustomRuleMatcher](../../api/DocumentTypeCustomRuleMatcher.md))
        * ro.sync.ecss.extensions.dita.map.[DITAMapResolvedReferencesCustomRuleMatcher](DITAMapResolvedReferencesCustomRuleMatcher.md)

    * ro.sync.ecss.extensions.dita.map.[EditPropertiesOperation](EditPropertiesOperation.md) (implements ro.sync.ecss.extensions.api.[AuthorOperation](../../api/AuthorOperation.md))
    * ro.sync.ecss.extensions.api.[ExtensionsBundle](../../api/ExtensionsBundle.md) (implements ro.sync.ecss.extensions.api.[Extension](../../api/Extension.md))
        * ro.sync.ecss.extensions.dita.[DITAExtensionsBundle](../DITAExtensionsBundle.md) (implements ro.sync.ecss.dita.[ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md))

            * ro.sync.ecss.extensions.dita.map.[DITAMapExtensionsBundle](DITAMapExtensionsBundle.md)

    * ro.sync.ecss.extensions.api.text.[TextPageExternalObjectInsertionHandler](../../api/text/TextPageExternalObjectInsertionHandler.md) (implements ro.sync.ecss.extensions.api.[Extension](../../api/Extension.md), ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](../../api/ExternalObjectInsertionSources.md))

        * ro.sync.ecss.extensions.dita.[DITATextPageExternalObjectInsertionHandler](../DITATextPageExternalObjectInsertionHandler.md)

            * ro.sync.ecss.extensions.dita.map.[DITAMapTextPageExternalObjectInsertionHandler](DITAMapTextPageExternalObjectInsertionHandler.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
