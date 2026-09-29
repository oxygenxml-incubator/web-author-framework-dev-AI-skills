Package [ro.sync.options](package-summary.md)

# Interface PersistentObject
    All Superinterfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html), [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   All Known Subinterfaces: [EditorTemplate](../exml/editor/EditorTemplate.md), [EditorTemplateWithContent](../template/EditorTemplateWithContent.md), [ExternalPersistentObject](../exml/workspace/api/options/ExternalPersistentObject.md)   All Known Implementing Classes: [ProfileConditionGroupPO](../ecss/conditions/ProfileConditionGroupPO.md), [ProfileConditionInfoPO](../ecss/conditions/ProfileConditionInfoPO.md), [ProfileConditionsSetInfoPO](../ecss/conditions/ProfileConditionsSetInfoPO.md), [ProfileConditionValuePO](../ecss/conditions/ProfileConditionValuePO.md), [ProfilingAttributesPresentingColorsPO](../ecss/conditions/ProfilingAttributesPresentingColorsPO.md), [ProfilingAttributeStylePO](../ecss/conditions/ProfilingAttributeStylePO.md), [SimpleListOfStringsExternalPersistentObject](../exml/workspace/api/options/SimpleListOfStringsExternalPersistentObject.md)   @API(type=EXTENDABLE, src=PRIVATE) public interface PersistentObjectextends [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html), [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)
Defines an object that can be stored in the options. It has to be a simple object, containing only primitive types, other PersistentObjects, or arrays of these types or classes from the java.lang, except the Object class.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [checkValid](#checkValid())()
Check if object is valid to be used.
  [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [clone](#clone())()
Forces all the persistent objects to be cloneable.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getNotPersistentFieldNames](#getNotPersistentFieldNames())()

## Method Details

### checkValid

void checkValid() throws [InvalidPersistentObjException](InvalidPersistentObjException.md)

Check if object is valid to be used. Method is called after it is deserialized from options. If not then throw an InvalidPersistentObjException exception.
  Throws: [InvalidPersistentObjException](InvalidPersistentObjException.md) - Thrown when instance is not valid.
### getNotPersistentFieldNames

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getNotPersistentFieldNames()
  Returns: The names of the field from this object which should not be serialized.
### clone

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) clone()

Forces all the persistent objects to be cloneable.
  Returns: A clone of this object. The clone and the original are disjunct. They share only immutable objects, like Strings, Integers, etc.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
