Package [ro.sync.ecss.dita](package-summary.md)

# Class DitaReferenceTargetDescriptor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.dita.DitaReferenceTargetDescriptor
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class DitaReferenceTargetDescriptor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Descriptor for a conref target.
  Since: 18.0
## Constructor Summary
 Constructors
Constructor

Description
 [DitaReferenceTargetDescriptor](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) nodeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentTopicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) className)
Constructor.
  [DitaReferenceTargetDescriptor](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) nodeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentTopicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) className, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootClassName)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getClassName](#getClassName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContent](#getContent())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getId](#getId())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNodeName](#getNodeName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParentTopicId](#getParentTopicId())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReferenceUrl](#getReferenceUrl())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRootClassName](#getRootClassName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DitaReferenceTargetDescriptor

public DitaReferenceTargetDescriptor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) nodeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentTopicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) className, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) rootClassName)

Constructor.
  Parameters: id - The ID of the target node. nodeName - The name of the target node. content - Some content from the target node. parentTopicId - The ID of the parent topic (if there is a topic ancestor). referenceUrl - The reference URL. className - The name of the class. rootClassName - Root element class name.
### DitaReferenceTargetDescriptor

public DitaReferenceTargetDescriptor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) nodeName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) content, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parentTopicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) referenceUrl, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) className)

Constructor.
  Parameters: id - The ID of the target node. nodeName - The name of the target node. content - Some content from the target node. parentTopicId - The ID of the parent topic (if there is a topic ancestor). referenceUrl - The reference URL. className - The name of the class.
## Method Details

### getId

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getId()
  Returns: The ID of the target node.
### getContent

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContent()
  Returns: Some content from the target node.
### getNodeName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNodeName()
  Returns: The name of the target node.
### getParentTopicId

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParentTopicId()
  Returns: The ID of the parent topic.
### getReferenceUrl

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReferenceUrl()
  Returns: Returns the reference URL.
### getClassName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getClassName()
  Returns: Returns the class of the target element.
### getRootClassName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRootClassName()
  Returns: Returns the rootClassName. Can be null.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
