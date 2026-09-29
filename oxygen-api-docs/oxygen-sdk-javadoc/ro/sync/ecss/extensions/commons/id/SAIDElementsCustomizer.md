Package [ro.sync.ecss.extensions.commons.id](package-summary.md)

# Class SAIDElementsCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.id.SAIDElementsCustomizer
   @API(type=INTERNAL, src=PUBLIC) public class SAIDElementsCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Customize the list of elements for auto ID generation. It is used on standalone implementation.

## Constructor Summary
 Constructors
Constructor

Description
 [SAIDElementsCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [GenerateIDElementsInfo](GenerateIDElementsInfo.md) [customizeIDElements](#customizeIDElements(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) autoIDElementsInfo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage)
Ask the user to customize the ID elements.
  [GenerateIDElementsInfo](GenerateIDElementsInfo.md) [customizeIDElements](#customizeIDElements(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo,java.lang.String,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) autoIDElementsInfo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)
Ask the user to customize the ID elements.
  [GenerateIDElementsInfo](GenerateIDElementsInfo.md) [customizeIDElements](#customizeIDElements(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo,java.lang.String,java.lang.String,boolean))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) autoIDElementsInfo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID, boolean isDocBook)
Ask the user to customize the ID elements.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### SAIDElementsCustomizer

public SAIDElementsCustomizer()

## Method Details

### customizeIDElements

public [GenerateIDElementsInfo](GenerateIDElementsInfo.md) customizeIDElements([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) autoIDElementsInfo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage)

Ask the user to customize the ID elements.
  Parameters: authorAccess - Access to author functionality. autoIDElementsInfo - Information about for what elements should IDs be generated. listMessage - The label used on the dialog before the list Returns: The initial list of elements for which to generate IDs.
### customizeIDElements

public [GenerateIDElementsInfo](GenerateIDElementsInfo.md) customizeIDElements([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) autoIDElementsInfo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID)

Ask the user to customize the ID elements.
  Parameters: authorAccess - Access to author functionality. autoIDElementsInfo - Information about for what elements should IDs be generated. listMessage - The label used on the dialog before the list helpPageID - The ID of the help page which will be opened when users invoke help in the dialog. Returns: The initial list of elements for which to generate IDs.
### customizeIDElements

public [GenerateIDElementsInfo](GenerateIDElementsInfo.md) customizeIDElements([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) autoIDElementsInfo, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) listMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) helpPageID, boolean isDocBook)

Ask the user to customize the ID elements.
  Parameters: authorAccess - Access to author functionality. autoIDElementsInfo - Information about for what elements should IDs be generated. listMessage - The label used on the dialog before the list helpPageID - The ID of the help page which will be opened when users invoke help in the dialog. isDocBook - true if we are in DocBook. Returns: The initial list of elements for which to generate IDs.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
