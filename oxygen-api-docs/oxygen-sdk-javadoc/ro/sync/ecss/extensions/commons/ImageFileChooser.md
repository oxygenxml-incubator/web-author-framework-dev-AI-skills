Package [ro.sync.ecss.extensions.commons](package-summary.md)

# Class ImageFileChooser

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.commons.ObjectChooser](ObjectChooser.md)
        * ro.sync.ecss.extensions.commons.ImageFileChooser
   @API(type=INTERNAL, src=PUBLIC) public class ImageFileChooser extends [ObjectChooser](ObjectChooser.md)
Choose an image file.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [IMG_FROM_TESTS](#IMG_FROM_TESTS)
Used to test the class from JUnit test cases.

### Fields inherited from class ro.sync.ecss.extensions.commons.[ObjectChooser](ObjectChooser.md)
 [ALLOWED_IMAGE_EXTENSIONS](ObjectChooser.md#ALLOWED_IMAGE_EXTENSIONS)
## Constructor Summary
 Constructors
Constructor

Description
 [ImageFileChooser](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [chooseImageFile](#chooseImageFile(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../api/AuthorAccess.md) authorAccess)
Ask user to choose an image file.

### Methods inherited from class ro.sync.ecss.extensions.commons.[ObjectChooser](ObjectChooser.md)
 [makeUrlRelative](ObjectChooser.md#makeUrlRelative(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### IMG_FROM_TESTS

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) IMG_FROM_TESTS

Used to test the class from JUnit test cases.

## Constructor Details

### ImageFileChooser

public ImageFileChooser()

## Method Details

### chooseImageFile

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) chooseImageFile([AuthorAccess](../api/AuthorAccess.md) authorAccess)

Ask user to choose an image file.
  Parameters: authorAccess - Access to some author utility methods. Returns: The path to the image file relative to the opened XML and escaped so that it can be used as an attribute value, or null if the user canceled the operation.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
