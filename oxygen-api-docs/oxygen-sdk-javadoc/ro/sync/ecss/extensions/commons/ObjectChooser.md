Package [ro.sync.ecss.extensions.commons](package-summary.md)

# Class ObjectChooser

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.ObjectChooser
   Direct Known Subclasses: [ImageFileChooser](ImageFileChooser.md), [MediaFileChooser](MediaFileChooser.md)   @API(type=INTERNAL, src=PUBLIC) public abstract class ObjectChooser extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Base class for choosers dialogs.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [ALLOWED_IMAGE_EXTENSIONS](#ALLOWED_IMAGE_EXTENSIONS)
All the allowed extensions for an image.

## Constructor Summary
 Constructors
Constructor

Description
 [ObjectChooser](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [makeUrlRelative](#makeUrlRelative(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)
Makes the given URL relative to the XML whose access object we are given.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### ALLOWED_IMAGE_EXTENSIONS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] ALLOWED_IMAGE_EXTENSIONS

All the allowed extensions for an image.

## Constructor Details

### ObjectChooser

public ObjectChooser()

## Method Details

### makeUrlRelative

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) makeUrlRelative([AuthorAccess](../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) url)

Makes the given URL relative to the XML whose access object we are given.
  Parameters: authorAccess - The author access of the XML document. url - The url. Returns: The relative URL.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
