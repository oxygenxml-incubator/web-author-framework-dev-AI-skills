Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Class SearchParams

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.project.SearchParams
   @API(type=EXTENDABLE, src=PUBLIC) public class SearchParams extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Params for finding content in the project.
  Since: 28  \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

## Constructor Summary
 Constructors
Constructor

Description
 [SearchParams](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,boolean,boolean,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileNameWildcard, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean caseSensitive, boolean regexp, int maxMatches)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFileNameWildcard](#getFileNameWildcard())()

 int [getMaxMatches](#getMaxMatches())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSearchString](#getSearchString())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getXpathExpression](#getXpathExpression())()

 boolean [isCaseSensitive](#isCaseSensitive())()

 boolean [isRegexp](#isRegexp())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SearchParams

public SearchParams([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fileNameWildcard, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) searchString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) xpathExpression, boolean caseSensitive, boolean regexp, int maxMatches)

Constructor.
  Parameters: fileNameWildcard - The file name wildcard searchString - Search string xpathExpression - Filter xpath expression caseSensitive - Case sensitive regexp - Regexp enabled maxMatches - Maximum matches.
## Method Details

### getSearchString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSearchString()
  Returns: Returns the searchString.
### isRegexp

public boolean isRegexp()
  Returns: Returns the regexp flag.
### isCaseSensitive

public boolean isCaseSensitive()
  Returns: Returns the caseSensitive flag.
### getMaxMatches

public int getMaxMatches()
  Returns: Returns the max matches size.
### getFileNameWildcard

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFileNameWildcard()
  Returns: Returns the file name wildcard.
### getXpathExpression

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getXpathExpression()
  Returns: Returns the xpath expression used to filter matches.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
