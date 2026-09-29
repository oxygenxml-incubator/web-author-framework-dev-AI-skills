Package [ro.sync.ecss.dita.topic.ref](package-summary.md)

# Class ExpandableTopicrefCounter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.dita.topic.ref.ExpandableTopicrefCounter
   @API(type=INTERNAL, src=PUBLIC) public class ExpandableTopicrefCounter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class that counts the number of expandable topic references.

## Constructor Summary
 Constructors
Constructor

Description
 [ExpandableTopicrefCounter](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../../extensions/api/AuthorAccess.md) authorAccess)

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getNumberOfReferencesToExpand](#getNumberOfReferencesToExpand())()

 static int [getTopicRefsLimit](#getTopicRefsLimit())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ExpandableTopicrefCounter

public ExpandableTopicrefCounter([AuthorAccess](../../../extensions/api/AuthorAccess.md) authorAccess)
  Parameters: authorAccess - The author access.
## Method Details

### getNumberOfReferencesToExpand

public int getNumberOfReferencesToExpand() throws [AuthorOperationException](../../../extensions/api/AuthorOperationException.md)
  Returns: the number of references found in document. Throws: [AuthorOperationException](../../../extensions/api/AuthorOperationException.md) - If it fails.
### getTopicRefsLimit

public static int getTopicRefsLimit()
  Returns: The maximum number of topic references to expand.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
