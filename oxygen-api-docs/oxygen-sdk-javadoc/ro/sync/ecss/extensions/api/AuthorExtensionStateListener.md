Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorExtensionStateListener
    All Superinterfaces: [Extension](Extension.md)   All Known Subinterfaces: [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md)   All Known Implementing Classes: [AuthorExtensionStateAdapter](AuthorExtensionStateAdapter.md), [AuthorExtensionStateListenerDelegator](AuthorExtensionStateListenerDelegator.md), [DefaultUniqueAttributesRecognizer](../commons/id/DefaultUniqueAttributesRecognizer.md), [DITAMapTopicTitlesResolveListener](../dita/map/DITAMapTopicTitlesResolveListener.md), [DITAUniqueAttributesRecognizer](../dita/id/DITAUniqueAttributesRecognizer.md), [Docbook4UniqueAttributesRecognizer](../docbook/id/Docbook4UniqueAttributesRecognizer.md), [Docbook5UniqueAttributesRecognizer](../docbook/id/Docbook5UniqueAttributesRecognizer.md), [DocBookUniqueAttributesRecognizer](../docbook/id/DocBookUniqueAttributesRecognizer.md), [TEIP5UniqueAttributesRecognizer](../tei/id/TEIP5UniqueAttributesRecognizer.md), [XHTMLUniqueAttributesRecognizer](../xhtml/id/XHTMLUniqueAttributesRecognizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorExtensionStateListenerextends [Extension](Extension.md)
Notified when the Author extension, where the listener is defined, was activated or deactivated in the detection process.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [activated](#activated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Method called when the Author extension was activated.
  void [deactivated](#deactivated(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Method called when the Author extension was deactivated.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### activated

void activated([AuthorAccess](AuthorAccess.md) authorAccess)

Method called when the Author extension was activated. This event is triggered when the Author extension where this listener is defined was activated in relation with a document opened in Author page. Listeners like [AuthorMouseListener](AuthorMouseListener.md) or [AuthorListener](AuthorListener.md) can be added at this point.
  Parameters: authorAccess - The [AuthorAccess](AuthorAccess.md) of the Author page where the listener was activated.
### deactivated

void deactivated([AuthorAccess](AuthorAccess.md) authorAccess)

Method called when the Author extension was deactivated. This event is triggered when another Author extension corresponding to the the current document opened in Author page was activated, the user switches to another editor page or the editor is closed.
  Parameters: authorAccess - The [AuthorAccess](AuthorAccess.md) of the Author page where the listener was deactivated.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
