Package [ro.sync.exml.plugin.ai](package-summary.md)

# Interface ExternalAIFunction
    @API(type=EXTENDABLE, src=PUBLIC) public interface ExternalAIFunction
Interface representing a function used by the AI to interact with the application. This interface defines the structure for function that can be invoked by the AI system to perform actions or retrieve information within the application. This function may require specific parameters (defined by a JSON schema) and can be used to extend the functionality of the AI system. The functions are typically invoked by the AI to access external services, manipulate data, or perform tasks that require interaction with the application environment.
  Since: 27.1
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [executeFunction](#executeFunction(java.lang.String,java.util.Map))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parameters, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> extraContext)
Executes the function with the specified parameters and additional context.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDescription](#getDescription())()
Returns a description of what the function does, used by the AI to choose when and how to call the function.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()
Returns The name of the AI function.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getParameterDescriptions](#getParameterDescriptions())()
Returns a JSON schema in String format describing the parameters the functions accepts.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getUIDecription](#getUIDecription())()
Returns a short description that will be displayed in the UI when the function is executed.
  default boolean [isEnabled](#isEnabled())()
Checks whether the function is enabled and can be sent to the AI.

## Method Details

### getName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()

Returns The name of the AI function. Must be a-z, A-Z, 0-9, or contain underscores and dashes, with a maximum length of 64.
The name should uniquely identify the external AI function and can be used to locate and execute the function.

  Returns: A string representing the name of the AI function. Cannot be null or empty.
### getDescription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDescription()

Returns a description of what the function does, used by the AI to choose when and how to call the function.
This method provides a detailed description of the AI function's purpose and behavior. It should explain what the function does, what kind of data it processes, and any relevant details about its operation.

  Returns: A string describing the AI function's behavior and purpose. It may be empty or null.
### getUIDecription

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getUIDecription()

Returns a short description that will be displayed in the UI when the function is executed. This description will not be sent to the AI.
  Returns: A description to be presented in the UI when function is executed. It may be empty or null.
### getParameterDescriptions

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getParameterDescriptions()

Returns a JSON schema in String format describing the parameters the functions accepts.
Example:

```
{
                "type": "object",
                "properties": {
                    "order_id": {
                        "type": "string",
                        "description": "The customer's order ID."
                    }
                },
                "required": ["order_id"],
                "additionalProperties": False
            }
```

  Returns: A string containing the JSON schema that describes parameters the functions accepts. Can be null when the function doesn't have parameters.
### executeFunction

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) executeFunction([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) parameters, [Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> extraContext)throws [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html), [ExternalServiceException](ExternalServiceException.md)

Executes the function with the specified parameters and additional context.
This method allows the AI to execute the function, passing in the required parameters (which should conform to the JSON schema returned by [getParameterDescriptions()](#getParameterDescriptions())) and any additional application context as key-value pairs. The function performs its operation (which may involve interacting with external services, accessing application data, or manipulating internal state) and returns a result as a string. The result could be a serialized JSON object or a plain string.

The function may modify the application's state, provide results back to the AI, or trigger further actions within the application based on the inputs provided.

  Parameters: parameters - A string representing the parameters required to execute the function. The format and content of this string should conform to the JSON schema returned by [getParameterDescriptions()](#getParameterDescriptions()). extraContext - A map containing additional application context or information needed by the function. When called from WebAuthor, it will contain an "author_document_model" key with the [AuthorDocumentModel](../../../ecss/extensions/api/webapp/AuthorDocumentModel.md) of the current editor. It will also contain a "session_id" key with a unique identifier assigned to the execution request session. Returns: A string representing the result of executing the AI function, which may be a serialized JSON object or a plain string, depending on the function's purpose and the interaction with the application. If an error occurs, the return value can contain an error message that the AI can interpret. Throws: [IllegalArgumentException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/IllegalArgumentException.html) - If the parameters are in an incorrect format or do not conform to the JSON schema defined by [getParameterDescriptions()](#getParameterDescriptions()). [ExternalServiceException](ExternalServiceException.md) - If an error occurs while calling the external AI service, or if the execution of the function fails.
### isEnabled

default boolean isEnabled()

Checks whether the function is enabled and can be sent to the AI.
This method allows the system to verify if the function is active and available for invocation. It is useful for determining whether the function should be executed in a given context, based on its enabled state.

The default implementation returns true, indicating that the function is enabled. However, this method can be overridden to introduce custom logic for enabling or disabling the function.

  Returns: true if the function is enabled and can be provided to the AI for calling it, false if the function is disabled and is not provided as a possible tool/function to the AI Since: 28
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
