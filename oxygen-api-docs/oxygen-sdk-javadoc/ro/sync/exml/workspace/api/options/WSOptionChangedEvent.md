Package [ro.sync.exml.workspace.api.options](package-summary.md)

# Class WSOptionChangedEvent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.options.WSOptionChangedEvent
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class WSOptionChangedEvent extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Represents an event which indicates that the value of an option has been changed.

## Constructor Summary
 Constructors
Constructor

Description
 [WSOptionChangedEvent](#%3Cinit%3E(java.lang.String,java.lang.Object,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) oldValue, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) newValue)
The constructor of the option changed event.
  [WSOptionChangedEvent](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)
The constructor of the option changed event.

## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getNewValue](#getNewValue())()  Deprecated.
The value may not be a plain String, use the "getNewValueObject" instead
   [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getNewValueObject](#getNewValueObject())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOldValue](#getOldValue())()  Deprecated.
The value may not be a plain String, use the "getOldValueObject" instead
   [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getOldValueObject](#getOldValueObject())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOptionKey](#getOptionKey())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### WSOptionChangedEvent

public WSOptionChangedEvent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) oldValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)

The constructor of the option changed event.
  Parameters: optionKey - The identification key of the option whose value modification generated this event. oldValue - The old value of the option. newValue - The new value of the option. When the entire set of Oxygen preferences is reset by the end user, the reported old value will be equal to the new value as the global reset no longer retains the state of the value before the reset...
### WSOptionChangedEvent

public WSOptionChangedEvent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionKey, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) oldValue, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) newValue)

The constructor of the option changed event.
  Parameters: optionKey - The identification key of the option whose value modification generated this event. oldValue - The old value of the option. newValue - The new value of the option. When the entire set of Oxygen preferences is reset by the end user, the reported old value will be equal to the new value as the global reset no longer retains the state of the value before the reset...
## Method Details

### getOptionKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOptionKey()
  Returns: Returns the identification key of the option associated with this event.
### getOldValue

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOldValue()
 Deprecated.
The value may not be a plain String, use the "getOldValueObject" instead
   Returns: Returns the old value of the option associated with this event.
### getOldValueObject

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getOldValueObject()
  Returns: Returns the old value of the option associated with this event. Since: 21.1
### getNewValue

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getNewValue()
 Deprecated.
The value may not be a plain String, use the "getNewValueObject" instead
   Returns: Returns the new value of the option associated with this event.
### getNewValueObject

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getNewValueObject()
  Returns: Returns the new value of the option associated with this event. Since: 21.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
