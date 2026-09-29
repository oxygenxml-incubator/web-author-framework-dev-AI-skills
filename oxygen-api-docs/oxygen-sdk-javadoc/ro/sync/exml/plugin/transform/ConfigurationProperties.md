Package [ro.sync.exml.plugin.transform](package-summary.md)

# Interface ConfigurationProperties
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ConfigurationProperties
Interface with transformer properties that can be passed externally.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [STREAMABLE](#STREAMABLE)
A flag signaling the fact that the processor should support streaming.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [XSLMessageListener](XSLMessageListener.md) [getMessageListener](#getMessageListener())()

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getProperty](#getProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

## Field Details

### STREAMABLE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) STREAMABLE

A flag signaling the fact that the processor should support streaming.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.transform.ConfigurationProperties.STREAMABLE)

## Method Details

### getMessageListener

[XSLMessageListener](XSLMessageListener.md) getMessageListener()
  Returns: Provide the message listener.
### getProperty

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
  Parameters: key - the key. Returns: The value of property specified by key.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
