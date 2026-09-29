Package [ro.sync.exml.workspace.api.editor](package-summary.md)

# Class ReadOnlyReason

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.ReadOnlyReason
   @API(type=EXTENDABLE, src=PUBLIC) public class ReadOnlyReason extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
An object describing the cause for which an editor is read-only.
  Since: 19.1
## Constructor Summary
 Constructors
Constructor

Description
 [ReadOnlyReason](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Constructor.
  [ReadOnlyReason](#%3Cinit%3E(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) code)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getCode](#getCode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ReadOnlyReason

public ReadOnlyReason([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) code)

Constructor.
  Parameters: message - The message that explains why the editor is read-only. code - The code of the cause for which the editor is read-only. It will be only accessible through the API.
### ReadOnlyReason

public ReadOnlyReason([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Constructor.
  Parameters: message - The message that explains why the editor is read-only.
## Method Details

### getMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage()
  Returns: The message that explains why the editor is read-only.
### getCode

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getCode()
  Returns: The code of the cause for which the editor is read-only. It will be only accessible through the API.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
