Package [ro.sync.exml.workspace.api.markdown](package-summary.md)

# Class MarkdownValidatorFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.markdown.MarkdownValidatorFactory
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public final class MarkdownValidatorFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Factory class for creating MarkdownValidator objects.
  Since: 22
## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [MarkdownValidator](MarkdownValidator.md) [createSchematronValidator](#createSchematronValidator(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)
Creates a new instance of MarkdownValidator that uses a Schematron schema for validation.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### createSchematronValidator

public static [MarkdownValidator](MarkdownValidator.md) createSchematronValidator([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)

Creates a new instance of MarkdownValidator that uses a Schematron schema for validation.
  Parameters: systemId - the system identifier (URI). If the systemId is a URL, it must be fully resolved (it may not be a relative URL). Returns: the created validator
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
