Package [ro.sync.ecss.extensions.api.access](package-summary.md)

# Class EditingSessionContext

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.access.EditingSessionContext
   All Implemented Interfaces: [ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public abstract class EditingSessionContext extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md)
The editing session context.

An editing session correspond to an user editing a document in the editor. Custom attributes can be registered from the API which can include information about the context of the editing, e.g. the user that performs the edit, the project in whose scope the editing session was started, etc.

The session context is serializable and it serializes only the attributes whose value is serializable. The rest of the attributes are ignored.

In Web Author, attributes can be added to the editing context by using:

* URL parameters specified in the web brosers
* JavaScript LoadingOptions set on the sync.api.Workspace.EventType.BEFORE_EDITOR_LOADED event handler.
* The [WebappEditingSessionLifecycleListener.editingSessionAboutToBeStarted(String, String, java.net.URL, java.util.Map)](../webapp/access/WebappEditingSessionLifecycleListener.md#editingSessionAboutToBeStarted(java.lang.String,java.lang.String,java.net.URL,java.util.Map)) callback.
  Since: 15.2
## Constructor Summary
 Constructors
Constructor

Description
 [EditingSessionContext](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAttribute](#getAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attr)
Gets the value of a custom attribute.
  abstract [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getAttributes](#getAttributes())()
Returns the set of all attributes.
  abstract void [setAttribute](#setAttribute(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attr, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)
Sets a custom attribute for the editing session.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface ro.sync.ecss.dita.[ContextKeyManagerProvider](../../../dita/ContextKeyManagerProvider.md)
 [getContextKeyManager](../../../dita/ContextKeyManagerProvider.md#getContextKeyManager())
## Constructor Details

### EditingSessionContext

public EditingSessionContext()

## Method Details

### setAttribute

public abstract void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attr, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

Sets a custom attribute for the editing session. If the attribute is already set it overrides the previous value.
  Parameters: attr - The attribute name. value - The attribute value.
### getAttribute

public abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attr)

Gets the value of a custom attribute.
  Parameters: attr - The attribute name. Returns: The attribute value or null if the attribute was not set.
### getAttributes

public abstract [Set](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Set.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getAttributes()

Returns the set of all attributes.
  Returns: The set of all attributes.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
