Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class OptionListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.OptionListener
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class OptionListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The listener which is notified about the value changes of an author extension level option.

## Constructor Summary
 Constructors
Constructor

Description
 [OptionListener](#%3Cinit%3E())()
Default constructor for the option listener.
  [OptionListener](#%3Cinit%3E(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Constructor for the option listener.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsConcrete Methods
Modifier and Type

Method

Description
 final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKey](#getKey())()

 abstract void [optionValueChanged](#optionValueChanged(ro.sync.ecss.extensions.api.OptionChangedEvent))([OptionChangedEvent](OptionChangedEvent.md) event)
This method is called when the value of the option associated with this listener has been modified.
  void [setKey](#setKey(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Set the key to listen to.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### OptionListener

public OptionListener()

Default constructor for the option listener. IMPORTANT, this default constructor is mostly intended to facilitate creating such objects from Javascript Rhino code. You must set a an option key using the "setKey" method after you are using this implicit constructor.
  Since: 21
### OptionListener

public OptionListener([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Constructor for the option listener.
  Parameters: key - The key of the option whose value modification triggers the listener notification.
## Method Details

### optionValueChanged

public abstract void optionValueChanged([OptionChangedEvent](OptionChangedEvent.md) event)

This method is called when the value of the option associated with this listener has been modified.
  Parameters: event - An [OptionChangedEvent](OptionChangedEvent.md) which indicates that the value of the associated option has been changed.
### setKey

public void setKey([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Set the key to listen to. The key must be set before the listener is added.
  Parameters: key - The key of the option whose value modification triggers the listener notification. Since: 21
### getKey

public final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKey()
  Returns: The key of the option this listener is notified about.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
