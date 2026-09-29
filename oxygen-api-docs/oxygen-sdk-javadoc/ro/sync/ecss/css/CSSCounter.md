Package [ro.sync.ecss.css](package-summary.md)

# Class CSSCounter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.css.CSSCounter
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class CSSCounter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)
A CSS counter identified by it's name.

## Constructor Summary
 Constructors
Constructor

Description
 [CSSCounter](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Constructor.
  [CSSCounter](#%3Cinit%3E(java.lang.String,int))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int defaultValue)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [CSSCounter](CSSCounter.md) [clone](#clone())()
Clones this counter.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()

 int [getValue](#getValue())()

 int [hashCode](#hashCode())()

 void [increment](#increment(int))(int increment)
Increment the counter.
  void [increment](#increment(int,boolean))(int increment, boolean ignoreNextIncremenet)
Increment the counter.
  void [reset](#reset())()
Reset the counter to the initial value.
  void [setDefaultValue](#setDefaultValue(int))(int defValue)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CSSCounter

public CSSCounter([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Constructor.
  Parameters: name - The name of the counter.
### CSSCounter

public CSSCounter([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, int defaultValue)

Constructor.
  Parameters: name - The name of the counter. defaultValue - The default value.
## Method Details

### increment

public void increment(int increment, boolean ignoreNextIncremenet)

Increment the counter.
  Parameters: increment - The increment value. ignoreNextIncremenet - true when the current counter is set to an element deleted with track changes, and the next increment should be ignored.
### increment

public void increment(int increment)

Increment the counter.
  Parameters: increment - The increment value.
### reset

public void reset()

Reset the counter to the initial value.

### getValue

public int getValue()
  Returns: The current value of the counter.
### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()
  Returns: The counter name.
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### setDefaultValue

public void setDefaultValue(int defValue)
  Parameters: defValue - A default value to be used both as initial and current values.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### clone

public [CSSCounter](CSSCounter.md) clone() throws [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html)

Clones this counter.
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Throws: [CloneNotSupportedException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/CloneNotSupportedException.html) See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
