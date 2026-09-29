Package [ro.sync.ecss.extensions.dita.map.topicref](package-summary.md)

# Class CreateAndInsertTopicRef.Arguments

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.map.topicref.CreateAndInsertTopicRef.Arguments
   Enclosing class: [CreateAndInsertTopicRef](CreateAndInsertTopicRef.md)   public static class CreateAndInsertTopicRef.Arguments extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Handles argument retrieval.

## Constructor Summary
 Constructors
Constructor

Description
 [Arguments](#%3Cinit%3E(ro.sync.ecss.extensions.api.ArgumentsMap,java.io.File))([ArgumentsMap](../../../api/ArgumentsMap.md) args, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkFolder)

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getFolderUrl](#getFolderUrl())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getInsertionLocation](#getInsertionLocation())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTopicContent](#getTopicContent())()

 [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) [getTopicFile](#getTopicFile())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### Arguments

public Arguments([ArgumentsMap](../../../api/ArgumentsMap.md) args, [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkFolder)
  Parameters: args - Args map. frameworkFolder - The framework folder.
## Method Details

### getTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()
  Returns: The title.
### getTopicContent

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTopicContent()
  Returns: The topic content
### getFolderUrl

public [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getFolderUrl()
  Returns: The folder URL argument.
### getInsertionLocation

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getInsertionLocation()
  Returns: The insertion location, as one of the constants in [AuthorConstants](../../../api/AuthorConstants.md).
### getTopicFile

public [File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) getTopicFile()
  Returns: The URL where to read the content from.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
