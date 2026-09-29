Package [ro.sync.ecss.extensions.commons.table.support](package-summary.md)

# Class CALSColSpanSpec

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.support.CALSColSpanSpec
   @API(type=INTERNAL, src=PUBLIC) public class CALSColSpanSpec extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Contains information about column span for the CALS table model (e.g. DocBook or DITA tables).

## Constructor Summary
 Constructors
Constructor

Description
 [CALSColSpanSpec](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) spanName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namest, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) nameend)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getEndColumnName](#getEndColumnName())()
Return the name of the end column.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSpanName](#getSpanName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getStartColumnName](#getStartColumnName())()
Return the name of the start column.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CALSColSpanSpec

public CALSColSpanSpec([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) spanName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namest, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) nameend)

Constructor.
  Parameters: spanName - The name of the span element. namest - The start column name. nameend - The end column name.
## Method Details

### getSpanName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSpanName()
  Returns: The name of the span specification. Can be null.
### getStartColumnName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getStartColumnName()

Return the name of the start column.
  Returns: The name of the start column. It can be null if the value for the start column name given on the constructor was null.
### getEndColumnName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getEndColumnName()

Return the name of the end column.
  Returns: The name of the end column. It can be null if the value for the end column name given on the constructor was null.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
