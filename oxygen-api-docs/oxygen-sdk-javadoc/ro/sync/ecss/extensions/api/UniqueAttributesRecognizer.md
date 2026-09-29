Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface UniqueAttributesRecognizer
    All Superinterfaces: [AuthorExtensionStateListener](AuthorExtensionStateListener.md), [Extension](Extension.md), [UniqueAttributesProcessor](UniqueAttributesProcessor.md)   All Known Implementing Classes: [DefaultUniqueAttributesRecognizer](../commons/id/DefaultUniqueAttributesRecognizer.md), [DITAUniqueAttributesRecognizer](../dita/id/DITAUniqueAttributesRecognizer.md), [Docbook4UniqueAttributesRecognizer](../docbook/id/Docbook4UniqueAttributesRecognizer.md), [Docbook5UniqueAttributesRecognizer](../docbook/id/Docbook5UniqueAttributesRecognizer.md), [DocBookUniqueAttributesRecognizer](../docbook/id/DocBookUniqueAttributesRecognizer.md), [TEIP5UniqueAttributesRecognizer](../tei/id/TEIP5UniqueAttributesRecognizer.md), [XHTMLUniqueAttributesRecognizer](../xhtml/id/XHTMLUniqueAttributesRecognizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface UniqueAttributesRecognizerextends [AuthorExtensionStateListener](AuthorExtensionStateListener.md), [UniqueAttributesProcessor](UniqueAttributesProcessor.md)
Identifies unique attributes like ID's.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [isAutoIDGenerationActive](#isAutoIDGenerationActive())()

### Methods inherited from interface ro.sync.ecss.extensions.api.[AuthorExtensionStateListener](AuthorExtensionStateListener.md)
 [activated](AuthorExtensionStateListener.md#activated(ro.sync.ecss.extensions.api.AuthorAccess)), [deactivated](AuthorExtensionStateListener.md#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))
### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
### Methods inherited from interface ro.sync.ecss.extensions.api.[UniqueAttributesProcessor](UniqueAttributesProcessor.md)
 [assignUniqueIDs](UniqueAttributesProcessor.md#assignUniqueIDs(int,int,boolean)), [copyAttributeOnSplit](UniqueAttributesProcessor.md#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))
## Method Details

### isAutoIDGenerationActive

boolean isAutoIDGenerationActive()
  Returns: true if auto
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
