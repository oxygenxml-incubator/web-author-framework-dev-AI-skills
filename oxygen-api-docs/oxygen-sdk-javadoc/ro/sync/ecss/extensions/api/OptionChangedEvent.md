Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class OptionChangedEvent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.OptionChangedEvent
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class OptionChangedEvent extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Represents an event which indicates that the value of an option has been changed.

## Constructor Summary
 Constructors
Constructor

Description
 [OptionChangedEvent](#%3Cinit%3E(java.lang.String,java.lang.Object,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) oldValue, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) newValue)
The constructor of the option changed event.
  [OptionChangedEvent](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)  Deprecated.
## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getNewObjectValue](#getNewObjectValue())()
Get the new value as an object (string, boolean or even a more complex persistent object).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNewValue](#getNewValue())()  Deprecated.  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getOldObjectValue](#getOldObjectValue())()
Get the new old as an object (string, boolean or even a more complex persistent object).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOldValue](#getOldValue())()  Deprecated.  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOptionKey](#getOptionKey())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OptionChangedEvent

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public OptionChangedEvent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)
 Deprecated.
The constructor of the option changed event. This constructor is deprecated, you should use the [OptionChangedEvent(String, Object, Object)](#%3Cinit%3E(java.lang.String,java.lang.Object,java.lang.Object)) constructor instead.
  Parameters: optionKey - The identification key of the option whose value modification generated this event. oldValue - The old value of the option. newValue - The new value of the option.
### OptionChangedEvent

public OptionChangedEvent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) oldValue, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) newValue)

The constructor of the option changed event.
  Parameters: optionKey - The identification key of the option whose value modification generated this event. oldValue - The old value of the option. newValue - The new value of the option.
## Method Details

### getOptionKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOptionKey()
  Returns: Returns the identification key of the option associated with this event.
### getOldValue

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOldValue()
 Deprecated.
Get the old value casted as a string. This method is deprecated, you should use the [getOldObjectValue()](#getOldObjectValue()) method instead.
  Returns: Returns the old value of the option associated with this event.
### getNewValue

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNewValue()
 Deprecated.
Get the new value casted as a string. This method is deprecated, you should use the [getNewObjectValue()](#getNewObjectValue()) method instead.
  Returns: Returns the new value of the option associated with this event.
### getOldObjectValue

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getOldObjectValue()

Get the new old as an object (string, boolean or even a more complex persistent object).
  Returns: Returns the old value of the option associated with this event.
### getNewObjectValue

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getNewObjectValue()

Get the new value as an object (string, boolean or even a more complex persistent object).
  Returns: Returns the new value of the option associated with this event.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
