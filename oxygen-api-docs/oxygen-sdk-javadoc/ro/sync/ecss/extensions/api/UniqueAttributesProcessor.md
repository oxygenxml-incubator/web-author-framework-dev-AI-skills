Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface UniqueAttributesProcessor
    All Known Subinterfaces: [UniqueAttributesRecognizer](UniqueAttributesRecognizer.md)   All Known Implementing Classes: [DefaultUniqueAttributesRecognizer](../commons/id/DefaultUniqueAttributesRecognizer.md), [DITAUniqueAttributesRecognizer](../dita/id/DITAUniqueAttributesRecognizer.md), [Docbook4UniqueAttributesRecognizer](../docbook/id/Docbook4UniqueAttributesRecognizer.md), [Docbook5UniqueAttributesRecognizer](../docbook/id/Docbook5UniqueAttributesRecognizer.md), [DocBookUniqueAttributesRecognizer](../docbook/id/DocBookUniqueAttributesRecognizer.md), [TEIP5UniqueAttributesRecognizer](../tei/id/TEIP5UniqueAttributesRecognizer.md), [XHTMLUniqueAttributesRecognizer](../xhtml/id/XHTMLUniqueAttributesRecognizer.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface UniqueAttributesProcessor
Identifies unique attributes like ID's.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [assignUniqueIDs](#assignUniqueIDs(int,int,boolean))(int startOffset, int endOffset, boolean forceGeneration)
Assigns unique IDs between a start and an end offset in the document.
  boolean [copyAttributeOnSplit](#copyAttributeOnSplit(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName, [AuthorElement](node/AuthorElement.md) element)
Checks if the attribute specified by QName can be considered as a valid attribute to copy when the element is split.

## Method Details

### copyAttributeOnSplit

boolean copyAttributeOnSplit([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrQName, [AuthorElement](node/AuthorElement.md) element)

Checks if the attribute specified by QName can be considered as a valid attribute to copy when the element is split.
  Parameters: attrQName - The attribute qualified name. element - The element. Returns: true if the attribute should be copied when Split is performed.
### assignUniqueIDs

void assignUniqueIDs(int startOffset, int endOffset, boolean forceGeneration)

Assigns unique IDs between a start and an end offset in the document.
  Parameters: startOffset - Start offset. endOffset - End offset. forceGeneration - true to generate ID even if the ID generation pattern list does not match.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
