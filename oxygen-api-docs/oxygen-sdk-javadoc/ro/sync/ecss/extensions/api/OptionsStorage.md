Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface OptionsStorage
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface OptionsStorage
This interface should be used if Author extension level options need to be stored and retrieved.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addOptionListener](#addOptionListener(ro.sync.ecss.extensions.api.OptionListener))([OptionListener](OptionListener.md) listener)
Adds an [OptionListener](OptionListener.md) to the current set of options.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOption](#getOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)
Provides the value of the option associated with the specified key.
  void [removeOptionListener](#removeOptionListener(ro.sync.ecss.extensions.api.OptionListener))([OptionListener](OptionListener.md) listener)
Removes an option listener from the current set of option listeners.
  void [setOption](#setOption(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)
Modifies the value of an option.
  void [setOptionsDoctypePrefix](#setOptionsDoctypePrefix(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionsDoctypePrefix)
Sets the options doctype prefix which is used to prefix options like a namespace.

## Method Details

### setOptionsDoctypePrefix

void setOptionsDoctypePrefix([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) optionsDoctypePrefix)

Sets the options doctype prefix which is used to prefix options like a namespace.
  Parameters: optionsDoctypePrefix - The document type prefix used to build the options keys. This should not be null.
### addOptionListener

void addOptionListener([OptionListener](OptionListener.md) listener)

Adds an [OptionListener](OptionListener.md) to the current set of options. The listener is notified when the value of its associated option changes.
  Parameters: listener - The [OptionListener](OptionListener.md) to be added.
### removeOptionListener

void removeOptionListener([OptionListener](OptionListener.md) listener)

Removes an option listener from the current set of option listeners.
  Parameters: listener - The [OptionListener](OptionListener.md) to be removed.
### getOption

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultValue)

Provides the value of the option associated with the specified key.
  Parameters: key - The key that uniquely identifies an option. defaultValue - The default value for the specified option. Returns: The value of the specified option or the default value if the option has not been set yet.
### setOption

void setOption([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) value)

Modifies the value of an option. If the supplied value is nullThe option will be removed from storage.
  Parameters: key - The key of the option whose value is to be modified. value - The new value of the option. If nullthe option will be removed from the storage.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
