# Hierarchy For Package ro.sync.ecss.extensions.api
 Package Hierarchies:
* [All Packages](../../../../../overview-tree.md)

## Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * javax.swing.undo.[AbstractUndoableEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/AbstractUndoableEdit.html) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), javax.swing.undo.[UndoableEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoableEdit.html))
        * javax.swing.undo.[CompoundEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html)

            * javax.swing.undo.[UndoManager](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html) (implements javax.swing.event.[UndoableEditListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/UndoableEditListener.html))

                * ro.sync.ecss.extensions.api.[AuthorUndoManager](AuthorUndoManager.md)

    * ro.sync.ecss.extensions.api.[ArgumentDescriptor](ArgumentDescriptor.md)
    * ro.sync.ecss.extensions.api.[AuthorActionEventDetails](AuthorActionEventDetails.md)
    * ro.sync.ecss.extensions.api.[AuthorActionEventHandlerBase](AuthorActionEventHandlerBase.md) (implements ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md))
        * ro.sync.ecss.extensions.api.[DefaultAuthorActionEventHandler](DefaultAuthorActionEventHandler.md)

            * ro.sync.ecss.extensions.api.[DITAAuthorActionEventHandler](DITAAuthorActionEventHandler.md)
            * ro.sync.ecss.extensions.api.[DocbookAuthorActionEventHandler](DocbookAuthorActionEventHandler.md)
            * ro.sync.ecss.extensions.api.[TEIAuthorActionEventHandler](TEIAuthorActionEventHandler.md)
            * ro.sync.ecss.extensions.api.[XHTMLAuthorActionEventHandler](XHTMLAuthorActionEventHandler.md)

    * ro.sync.ecss.extensions.api.[AuthorCaretEvent](AuthorCaretEvent.md)
    * ro.sync.ecss.extensions.api.[AuthorDocumentFilter](AuthorDocumentFilter.md)
    * ro.sync.ecss.extensions.api.[AuthorDocumentType](AuthorDocumentType.md) (implements java.lang.[Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html))
    * ro.sync.ecss.extensions.api.[AuthorExtensionStateAdapter](AuthorExtensionStateAdapter.md) (implements ro.sync.ecss.extensions.api.[AuthorExtensionStateListener](AuthorExtensionStateListener.md))
    * ro.sync.ecss.extensions.api.[AuthorExtensionStateListenerDelegator](AuthorExtensionStateListenerDelegator.md) (implements ro.sync.ecss.extensions.api.[AuthorExtensionStateListener](AuthorExtensionStateListener.md))
    * ro.sync.ecss.extensions.api.[AuthorExternalObjectInsertionHandler](AuthorExternalObjectInsertionHandler.md) (implements ro.sync.ecss.extensions.api.[Extension](Extension.md), ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](ExternalObjectInsertionSources.md))
    * ro.sync.ecss.extensions.api.[AuthorImageDecorator](AuthorImageDecorator.md) (implements ro.sync.ecss.extensions.api.[Extension](Extension.md))
    * ro.sync.ecss.extensions.api.[AuthorInputEvent](AuthorInputEvent.md)
        * ro.sync.ecss.extensions.api.[AuthorMouseEvent](AuthorMouseEvent.md)

    * ro.sync.ecss.extensions.api.[AuthorListenerAdapter](AuthorListenerAdapter.md) (implements ro.sync.ecss.extensions.api.[AuthorListener](AuthorListener.md))
    * ro.sync.ecss.extensions.api.[AuthorMouseAdapter](AuthorMouseAdapter.md) (implements ro.sync.ecss.extensions.api.[AuthorMouseListener](AuthorMouseListener.md))
    * ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter](AuthorSchemaAwareEditingHandlerAdapter.md) (implements ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md))
    * ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions](AuthorSchemaAwareEditingHandlerAdapter.WrapInAncestorsOptions.md)
    * ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProviderBase](AuthorTableColumnWidthProviderBase.md) (implements ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md))
    * ro.sync.ecss.extensions.api.[ContentInterval](ContentInterval.md)
    * ro.sync.ecss.extensions.api.[CustomAttributeValueEditor](CustomAttributeValueEditor.md) (implements ro.sync.ecss.extensions.api.[Extension](Extension.md))
    * ro.sync.ecss.extensions.api.[DefaultAuthorActionEventHandler.CiElementAndOffset](DefaultAuthorActionEventHandler.CiElementAndOffset.md)
    * ro.sync.ecss.extensions.api.[DITAConrefsResolverBase](DITAConrefsResolverBase.md) (implements ro.sync.ecss.extensions.api.[ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md))
    * ro.sync.ecss.extensions.api.[DocumentTypeAdvancedCustomRuleMatcher](DocumentTypeAdvancedCustomRuleMatcher.md) (implements ro.sync.ecss.extensions.api.[DocumentTypeCustomRuleMatcher](DocumentTypeCustomRuleMatcher.md))
    * ro.sync.ecss.extensions.api.[EditPropertiesHandlerAdapter](EditPropertiesHandlerAdapter.md) (implements ro.sync.ecss.extensions.api.[EditPropertiesHandler](EditPropertiesHandler.md))
    * ro.sync.ecss.extensions.api.[ErrorResolverContextInfo](ErrorResolverContextInfo.md)
    * ro.sync.ecss.extensions.api.[ExtensionsBundle](ExtensionsBundle.md) (implements ro.sync.ecss.extensions.api.[Extension](Extension.md))
    * ro.sync.ecss.extensions.api.[OptionChangedEvent](OptionChangedEvent.md)
    * ro.sync.ecss.extensions.api.[OptionListener](OptionListener.md)
    * ro.sync.ecss.extensions.api.[ProfilingConditionalTextProvider](ProfilingConditionalTextProvider.md)
    * ro.sync.ecss.extensions.api.[ReferenceErrorResolverExt](ReferenceErrorResolverExt.md) (implements ro.sync.ecss.extensions.api.[ReferenceErrorResolver](ReferenceErrorResolver.md))
    * ro.sync.ecss.extensions.api.[SpellCheckingProblemInfo](SpellCheckingProblemInfo.md)
        * ro.sync.ecss.extensions.api.[SpellCheckingProblemInfoWithSuggestions](SpellCheckingProblemInfoWithSuggestions.md)

    * ro.sync.ecss.extensions.api.[SpellSuggestionsInfo](SpellSuggestionsInfo.md)
    * java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))
        * java.lang.[Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

            * ro.sync.ecss.extensions.api.[AuthorOperationException](AuthorOperationException.md)
                * ro.sync.ecss.extensions.api.[AuthorOperationStoppedByUserException](AuthorOperationStoppedByUserException.md)

            * ro.sync.ecss.extensions.api.[CancelledByUserException](CancelledByUserException.md)
            * ro.sync.ecss.extensions.api.[InvalidEditException](InvalidEditException.md)
            * java.io.[IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
                * ro.sync.ecss.extensions.api.[CustomResolverException](CustomResolverException.md)

            * java.lang.[RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html)
                * ro.sync.ecss.extensions.api.[ReferenceResolverException](ReferenceResolverException.md)

            * org.xml.sax.[SAXException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXException.html)
                * org.xml.sax.[SAXParseException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html)

                    * ro.sync.ecss.extensions.api.[ReferenceResolverSAXParseException](ReferenceResolverSAXParseException.md)

            * ro.sync.ecss.extensions.api.[ValidatingReferenceResolverException](ValidatingReferenceResolverException.md)

    * ro.sync.ecss.extensions.api.[TooltipIconInfo](TooltipIconInfo.md)
    * ro.sync.ecss.extensions.api.[WidthRepresentation](WidthRepresentation.md) (implements java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

## Interface Hierarchy

* ro.sync.ecss.extensions.api.[ArgumentsMap](ArgumentsMap.md)
* ro.sync.ecss.extensions.api.[AttributesValueEditor](AttributesValueEditor.md)
* ro.sync.ecss.extensions.api.[AuthorAccessDeprecated](AuthorAccessDeprecated.md)
    * ro.sync.ecss.extensions.api.[AuthorAccess](AuthorAccess.md) (also extends ro.sync.ecss.extensions.api.[AuthorClipboardAccess](AuthorClipboardAccess.md), ro.sync.ecss.extensions.api.[AuthorConstants](AuthorConstants.md))

* ro.sync.ecss.extensions.api.[AuthorAttributesController](AuthorAttributesController.md)
    * ro.sync.ecss.extensions.api.[AuthorDocumentController](AuthorDocumentController.md) (also extends ro.sync.ecss.extensions.api.[AuthorPseudoClassController](AuthorPseudoClassController.md))

* ro.sync.ecss.extensions.api.[AuthorCaretListener](AuthorCaretListener.md)
* ro.sync.ecss.extensions.api.[AuthorClipboardAccess](AuthorClipboardAccess.md)
    * ro.sync.ecss.extensions.api.[AuthorAccess](AuthorAccess.md) (also extends ro.sync.ecss.extensions.api.[AuthorAccessDeprecated](AuthorAccessDeprecated.md), ro.sync.ecss.extensions.api.[AuthorConstants](AuthorConstants.md))

* ro.sync.ecss.extensions.api.[AuthorConstants](AuthorConstants.md)
    * ro.sync.ecss.extensions.api.[AuthorAccess](AuthorAccess.md) (also extends ro.sync.ecss.extensions.api.[AuthorAccessDeprecated](AuthorAccessDeprecated.md), ro.sync.ecss.extensions.api.[AuthorClipboardAccess](AuthorClipboardAccess.md))

* ro.sync.ecss.extensions.api.[AuthorDocumentEvent](AuthorDocumentEvent.md)
    * ro.sync.ecss.extensions.api.[AttributeChangedEvent](AttributeChangedEvent.md)
    * ro.sync.ecss.extensions.api.[DocumentContentChangedEvent](DocumentContentChangedEvent.md)

        * ro.sync.ecss.extensions.api.[DocumentContentDeletedEvent](DocumentContentDeletedEvent.md)
        * ro.sync.ecss.extensions.api.[DocumentContentInsertedEvent](DocumentContentInsertedEvent.md)

* ro.sync.ecss.extensions.api.[AuthorDocumentFilterBypass](AuthorDocumentFilterBypass.md)
* ro.sync.ecss.extensions.api.[AuthorExtensionActionProvider](AuthorExtensionActionProvider.md)
* ro.sync.ecss.extensions.api.[AuthorMouseListener](AuthorMouseListener.md)
* ro.sync.ecss.extensions.api.node.[AuthorNode](node/AuthorNode.md)
    * ro.sync.ecss.extensions.api.node.[AuthorParentNode](node/AuthorParentNode.md)

        * ro.sync.ecss.extensions.api.[AuthorElementBaseInterface](AuthorElementBaseInterface.md)

* ro.sync.ecss.extensions.api.[AuthorOperationWithCustomUndoBehavior](AuthorOperationWithCustomUndoBehavior.md)
* ro.sync.ecss.extensions.api.[AuthorPreloadProcessor](AuthorPreloadProcessor.md)
* ro.sync.ecss.extensions.api.[AuthorPseudoClassController](AuthorPseudoClassController.md)
    * ro.sync.ecss.extensions.api.[AuthorDocumentController](AuthorDocumentController.md) (also extends ro.sync.ecss.extensions.api.[AuthorAttributesController](AuthorAttributesController.md))

* ro.sync.ecss.extensions.api.[AuthorResourceBundle](AuthorResourceBundle.md)
* ro.sync.ecss.extensions.api.[AuthorReviewerNameController](AuthorReviewerNameController.md)
    * ro.sync.ecss.extensions.api.[AuthorReviewController](AuthorReviewController.md) (also extends ro.sync.ecss.extensions.api.[AuthorChangeTrackingController](AuthorChangeTrackingController.md))

* ro.sync.ecss.extensions.api.[AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md)
* ro.sync.ecss.extensions.api.[AuthorSchemaManager](AuthorSchemaManager.md)
* ro.sync.ecss.extensions.api.[AuthorSelectionModel](AuthorSelectionModel.md)
    * ro.sync.ecss.extensions.api.[AuthorSelectionAndCaretModel](AuthorSelectionAndCaretModel.md)

* ro.sync.ecss.extensions.api.[AuthorViewToModelInfo](AuthorViewToModelInfo.md)
* ro.sync.ecss.extensions.api.[AuthorXPathExpressionBuilder](AuthorXPathExpressionBuilder.md)
* ro.sync.ecss.extensions.api.[CacheableAuthorReferencesResolver](CacheableAuthorReferencesResolver.md)
* ro.sync.ecss.extensions.api.[ChangeTrackingController](ChangeTrackingController.md)
    * ro.sync.ecss.extensions.api.[AuthorChangeTrackingController](AuthorChangeTrackingController.md)

        * ro.sync.ecss.extensions.api.[AuthorReviewController](AuthorReviewController.md) (also extends ro.sync.ecss.extensions.api.[AuthorReviewerNameController](AuthorReviewerNameController.md))

* ro.sync.ecss.extensions.api.[ClassPathResourcesAccess](ClassPathResourcesAccess.md)
* ro.sync.ecss.extensions.api.[CompoundEditListener](CompoundEditListener.md)
    * ro.sync.ecss.extensions.api.[AuthorListener](AuthorListener.md)

* ro.sync.ecss.extensions.api.[Content](Content.md)
* ro.sync.ecss.extensions.api.[CustomAttributeValueContext](CustomAttributeValueContext.md)
* ro.sync.ecss.extensions.api.[EditedAttribute](EditedAttribute.md)
* ro.sync.ecss.extensions.api.[Extension](Extension.md)
    * ro.sync.ecss.extensions.api.[AuthorActionEventHandler](AuthorActionEventHandler.md)
    * ro.sync.ecss.extensions.api.[AuthorExtensionStateListener](AuthorExtensionStateListener.md)
        * ro.sync.ecss.extensions.api.[UniqueAttributesRecognizer](UniqueAttributesRecognizer.md) (also extends ro.sync.ecss.extensions.api.[UniqueAttributesProcessor](UniqueAttributesProcessor.md))

    * ro.sync.ecss.extensions.api.[AuthorOperation](AuthorOperation.md)
    * ro.sync.ecss.extensions.api.[AuthorReferenceResolver](AuthorReferenceResolver.md)
        * ro.sync.ecss.extensions.api.[ValidatingAuthorReferenceResolver](ValidatingAuthorReferenceResolver.md)

            * ro.sync.ecss.extensions.api.[DITAMapReferencesResolver](DITAMapReferencesResolver.md)

    * ro.sync.ecss.extensions.api.[AuthorTableCellSepProvider](AuthorTableCellSepProvider.md)
    * ro.sync.ecss.extensions.api.[AuthorTableCellSpanProvider](AuthorTableCellSpanProvider.md)
    * ro.sync.ecss.extensions.api.[AuthorTableColumnWidthProvider](AuthorTableColumnWidthProvider.md)
    * ro.sync.ecss.extensions.api.[AWTExtension](AWTExtension.md)
    * ro.sync.ecss.extensions.api.[DocumentTypeCustomRuleMatcher](DocumentTypeCustomRuleMatcher.md)
    * ro.sync.ecss.extensions.api.[EditPropertiesHandler](EditPropertiesHandler.md)
    * ro.sync.ecss.extensions.api.[StylesFilter](StylesFilter.md)
    * ro.sync.ecss.extensions.api.[SWTExtension](SWTExtension.md)

* ro.sync.ecss.extensions.api.[ExternalObjectInsertionSources](ExternalObjectInsertionSources.md)
* ro.sync.ecss.extensions.api.[OptionsStorage](OptionsStorage.md)
* ro.sync.ecss.extensions.api.[ReferenceErrorResolver](ReferenceErrorResolver.md)
* ro.sync.ecss.extensions.api.[UniqueAttributesProcessor](UniqueAttributesProcessor.md)
    * ro.sync.ecss.extensions.api.[UniqueAttributesRecognizer](UniqueAttributesRecognizer.md) (also extends ro.sync.ecss.extensions.api.[AuthorExtensionStateListener](AuthorExtensionStateListener.md))

* ro.sync.ecss.extensions.api.[WebappExtensionsProvider](WebappExtensionsProvider.md)

## Annotation Interface Hierarchy

* ro.sync.ecss.extensions.api.[WebappCompatible](WebappCompatible.md) (implements java.lang.annotation.[Annotation](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/Annotation.html))

## Enum Class Hierarchy

* java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)

    * java.lang.[Enum](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Enum.html)<E> (implements java.lang.[Comparable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Comparable.html)<T>, java.lang.constant.[Constable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/constant/Constable.html), java.io.[Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html))

        * ro.sync.ecss.extensions.api.[AuthorActionEventHandler.AuthorActionEventType](AuthorActionEventHandler.AuthorActionEventType.md)
        * ro.sync.ecss.extensions.api.[CursorType](CursorType.md)
        * ro.sync.ecss.extensions.api.[CustomAttributeValueEditingContext](CustomAttributeValueEditingContext.md)
        * ro.sync.ecss.extensions.api.[ReferenceType](ReferenceType.md)
        * ro.sync.ecss.extensions.api.[SelectionInterpretationMode](SelectionInterpretationMode.md)
        * ro.sync.ecss.extensions.api.[WidthRepresentation.Unit](WidthRepresentation.Unit.md)
        * ro.sync.ecss.extensions.api.[XPathVersion](XPathVersion.md)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
