Package [ro.sync.ecss.extensions.api.component.listeners](package-summary.md)

# Class OpenURLHandler

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.component.listeners.OpenURLHandler
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class OpenURLHandler extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Listener for URLs the user is trying to open from the Author Component. For example the user clicked on a link in the Author page.
  Since: 12.2
## Constructor Summary
 Constructors
Constructor

Description
 [OpenURLHandler](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [handleOpenURL](#handleOpenURL(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) toOpen)
An attempt is made to open an URL.
  void [handleOpenURLAsDITAMapTree](#handleOpenURLAsDITAMapTree(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) toOpen)
An attempt is made to open an URL as a DITA Map tree.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OpenURLHandler

public OpenURLHandler()

## Method Details

### handleOpenURL

public void handleOpenURL([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) toOpen)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

An attempt is made to open an URL. For example a click was made in the Author page.
  Parameters: toOpen - The URL which should be opened by the developer's code. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
### handleOpenURLAsDITAMapTree

public void handleOpenURLAsDITAMapTree([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) toOpen)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

An attempt is made to open an URL as a DITA Map tree. For example a map is opened in the DITAMapTreeComponentProvider and the user double clicks a map referenced in the current map. By default this method delegates to handleOpenURL(URL) but it can be overwritten to open the URL as a DITAMapTreeComponentProvider.
  Parameters: toOpen - The URL which should be opened by the developer's code. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) Since: 15
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
