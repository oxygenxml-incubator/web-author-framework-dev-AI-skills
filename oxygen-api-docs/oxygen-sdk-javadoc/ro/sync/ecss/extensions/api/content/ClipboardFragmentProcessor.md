Package [ro.sync.ecss.extensions.api.content](package-summary.md)

# Interface ClipboardFragmentProcessor
    All Known Implementing Classes: [DefaultUniqueAttributesRecognizer](../../commons/id/DefaultUniqueAttributesRecognizer.md), [DITAUniqueAttributesRecognizer](../../dita/id/DITAUniqueAttributesRecognizer.md), [Docbook4UniqueAttributesRecognizer](../../docbook/id/Docbook4UniqueAttributesRecognizer.md), [Docbook5UniqueAttributesRecognizer](../../docbook/id/Docbook5UniqueAttributesRecognizer.md), [DocBookUniqueAttributesRecognizer](../../docbook/id/DocBookUniqueAttributesRecognizer.md), [TEIP5UniqueAttributesRecognizer](../../tei/id/TEIP5UniqueAttributesRecognizer.md), [XHTMLUniqueAttributesRecognizer](../../xhtml/id/XHTMLUniqueAttributesRecognizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ClipboardFragmentProcessor
Process a document fragment from the clipboard (pasted or dropped in the Author page).
  Since: 12.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [process](#process(ro.sync.ecss.extensions.api.content.ClipboardFragmentInformation))([ClipboardFragmentInformation](ClipboardFragmentInformation.md) fragmentInformation)
Process a fragment in the clipboard before inserting it in the document.

## Method Details

### process

void process([ClipboardFragmentInformation](ClipboardFragmentInformation.md) fragmentInformation)

Process a fragment in the clipboard before inserting it in the document.
  Parameters: fragmentInformation - Information about a fragment in the clipboard.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
