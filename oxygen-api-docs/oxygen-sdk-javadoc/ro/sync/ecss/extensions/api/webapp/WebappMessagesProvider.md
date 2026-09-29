Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface WebappMessagesProvider
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappMessagesProvider
Gets all the error messages reported by the application.
  Since: 16.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [clearMessages](#clearMessages())()
Clears messages list.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappMessage](WebappMessage.md)> [getMessages](#getMessages())()

## Method Details

### clearMessages

void clearMessages()

Clears messages list.

### getMessages

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[WebappMessage](WebappMessage.md)> getMessages()
  Returns: Returns The error messages reported so far.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
