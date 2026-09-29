Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Class EditorVariablesResolver

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.util.EditorVariablesResolver
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class EditorVariablesResolver extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Such a resolver can be registered via the "ro.sync.exml.workspace.api.util.UtilAccess" API and is called to resolve custom editor variables in a string.
  Since: 16.1
## Constructor Summary
 Constructors
Constructor

Description
 [EditorVariablesResolver](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[EditorVariableDescription](EditorVariableDescription.md)> [getCustomResolverEditorVariableDescriptions](#getCustomResolverEditorVariableDescriptions())()
Get a list with all editor variables which are custom resolved by this resolver.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resolveEditorVariables](#resolveEditorVariables(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentWithEditorVariables, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL)
Resolve editor variables in the received content.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditorVariablesResolver

public EditorVariablesResolver()

## Method Details

### resolveEditorVariables

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resolveEditorVariables([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentWithEditorVariables, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) currentEditedFileURL)

Resolve editor variables in the received content.
  Parameters: contentWithEditorVariables - The initial content which possibly contains unresolved editor variables. currentEditedFileURL - The current edited file URL, can be used if the editor variable depends on the current edited file. Returns: The processed content with certain editor variables replaced with developer-specific values or the original content. Can also return null to let the default processing occur.
### getCustomResolverEditorVariableDescriptions

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[EditorVariableDescription](EditorVariableDescription.md)> getCustomResolverEditorVariableDescriptions()

Get a list with all editor variables which are custom resolved by this resolver.
  Returns: a list with all editor variables which are custom resolved by this resolver. Since: 18.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
