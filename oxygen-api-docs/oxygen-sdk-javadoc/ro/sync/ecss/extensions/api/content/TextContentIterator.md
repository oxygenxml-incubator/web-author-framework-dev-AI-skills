Package [ro.sync.ecss.extensions.api.content](package-summary.md)

# Interface TextContentIterator
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface TextContentIterator
Iterate over the text content in the Author document between a start and an end offset.
  Since: 13
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [hasNext](#hasNext())()
Check if has a next text context.
  [TextContext](TextContext.md) [next](#next())()
Get the next text context.

## Method Details

### next

[TextContext](TextContext.md) next()

Get the next text context.
  Returns: the next texy context.
### hasNext

boolean hasNext()

Check if has a next text context.
  Returns: true if has next context or false if it has reached the end of the iteration interval. Throws: [NoSuchElementException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/NoSuchElementException.html)
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
