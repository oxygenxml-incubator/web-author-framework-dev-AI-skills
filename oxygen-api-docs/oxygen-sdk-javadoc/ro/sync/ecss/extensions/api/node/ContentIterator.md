Package [ro.sync.ecss.extensions.api.node](package-summary.md)

# Interface ContentIterator
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ContentIterator
Iterator over the content of a node.
  Since: 22
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [hasNext](#hasNext())()

 char [next](#next())()

## Method Details

### hasNext

boolean hasNext()
  Returns: true if another char can be obtain using the next() method.
### next

char next() throws [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
  Returns: The next char in the content. Throws: [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html) - If there are no more next characters.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
