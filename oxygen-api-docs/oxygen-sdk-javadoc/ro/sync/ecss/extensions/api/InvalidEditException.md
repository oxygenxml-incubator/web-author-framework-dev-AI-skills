Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class InvalidEditException

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
        * [java.lang.Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
            * ro.sync.ecss.extensions.api.InvalidEditException
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(type=EXTENDABLE, src=PUBLIC) public class InvalidEditException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
Exception thrown by [AuthorSchemaAwareEditingHandler](AuthorSchemaAwareEditingHandler.md) methods when an edit is considered invalid and must be rejected.
  See Also:
* [Serialized Form](../../../../../serialized-form.md#ro.sync.ecss.extensions.api.InvalidEditException)

## Constructor Summary
 Constructors
Constructor

Description
 [InvalidEditException](#%3Cinit%3E(java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, boolean presentToUser)
Constructor.
  [InvalidEditException](#%3Cinit%3E(java.lang.String,java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, boolean presentToUser, boolean showLinkToSchemaAwarePreferences)
Constructor.
  [InvalidEditException](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.Throwable,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) cause, boolean presentToUser)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHtmlMessage](#getHtmlMessage())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()

 boolean [isPresentToUser](#isPresentToUser())()

 boolean [isShowLinkToSchemaAwarePreferences](#isShowLinkToSchemaAwarePreferences())()

 void [setHtmlMessage](#setHtmlMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) htmlMessage)

 void [setPresentToUser](#setPresentToUser(boolean))(boolean presentToUser)
Choose not to present the exception to the user.
  void [setShowLinkToSchemaAwarePreferences](#setShowLinkToSchemaAwarePreferences(boolean))(boolean showLinkToSchemaAwarePreferences)

### Methods inherited from class java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
 [addSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#addSuppressed(java.lang.Throwable)), [fillInStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#fillInStackTrace()), [getCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getCause()), [getLocalizedMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getLocalizedMessage()), [getMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getMessage()), [getStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getStackTrace()), [getSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getSuppressed()), [initCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#initCause(java.lang.Throwable)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace()), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintStream)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintWriter)), [setStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#setStackTrace(java.lang.StackTraceElement%5B%5D)), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### InvalidEditException

public InvalidEditException([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, boolean presentToUser, boolean showLinkToSchemaAwarePreferences)

Constructor.
  Parameters: title - Title to be presented to the user. description - Error message. presentToUser - true if the error message must be presented to the user. showLinkToSchemaAwarePreferences - If true when the error message is presented to the user a link to the Schema Aware preference page will be added.
### InvalidEditException

public InvalidEditException([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, boolean presentToUser)

Constructor.
  Parameters: title - Title to be presented to the user. description - Error message. presentToUser - true if the error message must be presented to the user.
### InvalidEditException

public InvalidEditException([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) description, [Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html) cause, boolean presentToUser)

Constructor.
  Parameters: title - Title to be presented to the user. description - Error message. cause - The exception cause. A null value is permitted, and indicates that the cause is nonexistent or unknown. presentToUser - true if the error message must be presented to the user.
## Method Details

### isPresentToUser

public boolean isPresentToUser()
  Returns: true if the error message should be presented to the user.
### getTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()
  Returns: Returns the title.
### setHtmlMessage

public void setHtmlMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) htmlMessage)
  Parameters: htmlMessage - An error message that uses HTML elements for styling.
### getHtmlMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHtmlMessage()
  Returns: Returns the error message using HTML elements to style. null if a styled message is not available.
### setShowLinkToSchemaAwarePreferences

public void setShowLinkToSchemaAwarePreferences(boolean showLinkToSchemaAwarePreferences)
  Parameters: showLinkToSchemaAwarePreferences - The showLinkToSchemaAwarePreferences to set.
### isShowLinkToSchemaAwarePreferences

public boolean isShowLinkToSchemaAwarePreferences()
  Returns: Returns the showLinkToSchemaAwarePreferences.
### setPresentToUser

public void setPresentToUser(boolean presentToUser)

Choose not to present the exception to the user.
  Parameters: presentToUser - The presentToUser to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
