Package [ro.sync.ecss.extensions.dita.id](package-summary.md)

# Class DITAUniqueAttributesRecognizerUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.id.DITAUniqueAttributesRecognizerUtil
   @API(type=INTERNAL, src=PUBLIC) public class DITAUniqueAttributesRecognizerUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility class for Schema Aware actions.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static void [correctFragmentReferences](#correctFragmentReferences(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment,java.net.URL,java.net.URL))([AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) fragment, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) sourceURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) destinationURL)
Corrects fragment references before insert

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### correctFragmentReferences

public static void correctFragmentReferences([AuthorDocumentFragment](../../api/node/AuthorDocumentFragment.md) fragment, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) sourceURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) destinationURL)

Corrects fragment references before insert
  Parameters: fragment - The fragment to check for references and correct. sourceURL - Source URL. destinationURL - The URL of the file where the fragments will be inserted. References will be relative to this location.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
