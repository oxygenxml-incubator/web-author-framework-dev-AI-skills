Package [ro.sync.ecss.extensions.api.webapp.findreplace](package-summary.md)

# Class WebappFindOptions

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.findreplace.WebappFindOptions
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class WebappFindOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Find/Replace options.
  Since: 19.1
## Constructor Summary
 Constructors
Constructor

Description
 [WebappFindOptions](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [isMatchCase](#isMatchCase())()

 boolean [isWholeWords](#isWholeWords())()

 void [setMatchCase](#setMatchCase(boolean))(boolean matchCase)

 void [setWholeWords](#setWholeWords(boolean))(boolean wholeWords)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WebappFindOptions

public WebappFindOptions()

## Method Details

### isMatchCase

public boolean isMatchCase()
  Returns: Returns true if search should be case sensitive.
### setMatchCase

public void setMatchCase(boolean matchCase)
  Parameters: matchCase - true if search should be case sensitive.
### setWholeWords

public void setWholeWords(boolean wholeWords)
  Parameters: wholeWords - true if search should match whole words only.
### isWholeWords

public boolean isWholeWords()
  Returns: Returns true if search should match whole words only.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
