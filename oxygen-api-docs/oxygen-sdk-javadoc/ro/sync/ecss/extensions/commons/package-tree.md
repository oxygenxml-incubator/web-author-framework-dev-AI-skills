# Hierarchy For Package ro.sync.ecss.extensions.commons
 Package Hierarchies:
* [All Packages](../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * ro.sync.ecss.extensions.commons.[AbstractDocumentTypeHelper](AbstractDocumentTypeHelper.md) (implements ro.sync.ecss.extensions.commons.table.operations.[AuthorTableHelper](table/operations/AuthorTableHelper.md))
    * ro.sync.ecss.extensions.commons.[DefaultElementLocatorProvider](DefaultElementLocatorProvider.md) (implements ro.sync.ecss.extensions.api.link.[ElementLocatorProvider](../api/link/ElementLocatorProvider.md))
    * ro.sync.ecss.extensions.api.link.[ElementLocator](../api/link/ElementLocator.md)
        * ro.sync.ecss.extensions.commons.[IDElementLocator](IDElementLocator.md)
        * ro.sync.ecss.extensions.commons.[XPointerElementLocator](XPointerElementLocator.md)

    * ro.sync.ecss.extensions.commons.[MediaObjectsUtil](MediaObjectsUtil.md)
    * ro.sync.ecss.extensions.commons.[ObjectChooser](ObjectChooser.md)
        * ro.sync.ecss.extensions.commons.[ImageFileChooser](ImageFileChooser.md)
        * ro.sync.ecss.extensions.commons.[MediaFileChooser](MediaFileChooser.md)

    * java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.lang.[Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

            * ro.sync.ecss.extensions.api.[AuthorOperationException](../api/AuthorOperationException.md)
                * ro.sync.ecss.extensions.commons.[PasteAsReferenceException](PasteAsReferenceException.md)

            * ro.sync.exml.workspace.api.images.handlers.[CannotEditException](../../../exml/workspace/api/images/handlers/CannotEditException.md)

                * ro.sync.ecss.extensions.commons.[CannotEditException](CannotEditException.md)

    * ro.sync.exml.workspace.api.node.customizer.[XMLNodeRendererCustomizer](../../../exml/workspace/api/node/customizer/XMLNodeRendererCustomizer.md) (implements ro.sync.ecss.extensions.api.[Extension](../api/Extension.md))

        * ro.sync.ecss.extensions.commons.[XMLNodeRendererCustomizerAdapter](XMLNodeRendererCustomizerAdapter.md)

## Interface Hierarchy

* ro.sync.ecss.extensions.commons.[ExtensionTags](ExtensionTags.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
