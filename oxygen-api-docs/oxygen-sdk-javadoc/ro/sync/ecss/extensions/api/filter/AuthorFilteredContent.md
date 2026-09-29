Package [ro.sync.ecss.extensions.api.filter](package-summary.md)

# Interface AuthorFilteredContent
    All Superinterfaces: [CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorFilteredContentextends [CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html)
The char sequence representing the filtered Author content. The content represents the entire text content of the Author page + additional markers/sentinels at offsets which are pointed to by the AuthorNodes. Each AuthorNode points to specific start and end character markers in the content. The start and end offsets pointed to by the AuthorNode can be retrieved using the AuthorNode.getStartOffset() and AuthorNode.getEndOffset()
  Since: 12.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getOriginalOffset](#getOriginalOffset(int))(int filteredOffset)
Get the original offset corresponding to the given filtered offset.

### Methods inherited from interface java.lang.[CharSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html)
 [charAt](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html#charAt(int)), [chars](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html#chars()), [codePoints](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html#codePoints()), [isEmpty](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html#isEmpty()), [length](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html#length()), [subSequence](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html#subSequence(int,int)), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CharSequence.html#toString())
## Method Details

### getOriginalOffset

int getOriginalOffset(int filteredOffset)

Get the original offset corresponding to the given filtered offset.
  Parameters: filteredOffset - The filtered offset. Returns: The original offset corresponding to the filtered offset.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
