Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Class AuthorDocumentModelContextManager

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.AuthorDocumentModelContextManager
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorDocumentModelContextManager extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
A helper class that handles the current editing context. In Oxygen there are many 'per editing session' (e.g. the DITA map) or 'per user' options (e.g. the reviewer name). This manager installs the context which contains the values of these options for the currently edited document on the current thread.
  Since: 16.0
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorDocumentModelContextManager](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static void [installContext](#installContext(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([AuthorDocumentModel](AuthorDocumentModel.md) documentModel)
Sets the specified document model as being edited on the current thread.
  static void [uninstallContext](#uninstallContext(ro.sync.ecss.extensions.api.webapp.AuthorDocumentModel))([AuthorDocumentModel](AuthorDocumentModel.md) documentModel)
Sets the specified document model as not being edited anymore on the current thread.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorDocumentModelContextManager

public AuthorDocumentModelContextManager()

## Method Details

### installContext

public static void installContext([AuthorDocumentModel](AuthorDocumentModel.md) documentModel)

Sets the specified document model as being edited on the current thread.
  Parameters: documentModel - The document model to set as being edited on the current thread.
### uninstallContext

public static void uninstallContext([AuthorDocumentModel](AuthorDocumentModel.md) documentModel)

Sets the specified document model as not being edited anymore on the current thread.
  Parameters: documentModel - The document model.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
