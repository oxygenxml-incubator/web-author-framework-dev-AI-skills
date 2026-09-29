Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class ReferenceResolverException

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [java.lang.Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
        * [java.lang.Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
            * [java.lang.RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html)
                * ro.sync.ecss.extensions.api.ReferenceResolverException
   All Implemented Interfaces: [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)   @API(type=EXTENDABLE, src=PUBLIC) public class ReferenceResolverException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html)
Exception thrown if the reference resolver could not resolve a target.
  See Also:
* [Serialized Form](../../../../../serialized-form.md#ro.sync.ecss.extensions.api.ReferenceResolverException)

## Constructor Summary
 Constructors
Constructor

Description
 [ReferenceResolverException](#%3Cinit%3E(java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage, boolean showInResultsPanel, boolean reportAsError)
Constructor.
  [ReferenceResolverException](#%3Cinit%3E(java.lang.String,java.lang.String,boolean,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortErrorMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) originalErrorMessage, boolean showInResultsPanel, boolean reportAsError)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [ReferenceErrorResolver](ReferenceErrorResolver.md) [getErrorResolver](#getErrorResolver())()
Gets a possible solution for the user.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getShortMessage](#getShortMessage())()
Obtain the exception short message.
  boolean [isReportAsError](#isReportAsError())()
Check if the exception should be reported as an error.
  boolean [isShowInResultsPanel](#isShowInResultsPanel())()
Check if should also show the message in a results panel.
  void [setErrorResolver](#setErrorResolver(ro.sync.ecss.extensions.api.ReferenceErrorResolver))([ReferenceErrorResolver](ReferenceErrorResolver.md) errorResolver)
Sets a possible solution for the user.

### Methods inherited from class java.lang.[Throwable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html)
 [addSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#addSuppressed(java.lang.Throwable)), [fillInStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#fillInStackTrace()), [getCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getCause()), [getLocalizedMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getLocalizedMessage()), [getMessage](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getMessage()), [getStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getStackTrace()), [getSuppressed](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#getSuppressed()), [initCause](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#initCause(java.lang.Throwable)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace()), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintStream)), [printStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#printStackTrace(java.io.PrintWriter)), [setStackTrace](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#setStackTrace(java.lang.StackTraceElement%5B%5D)), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Throwable.html#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ReferenceResolverException

public ReferenceResolverException([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorMessage, boolean showInResultsPanel, boolean reportAsError)

Constructor.
  Parameters: errorMessage - The error message. showInResultsPanel - true to also show the message in a results panel. reportAsError - true to report as error, false to report as warning.
### ReferenceResolverException

public ReferenceResolverException([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) shortErrorMessage, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) originalErrorMessage, boolean showInResultsPanel, boolean reportAsError)

Constructor.
  Parameters: shortErrorMessage - The short error message. Sometimes the message which will be presented first time to the user is shorter than the original message. originalErrorMessage - The exception original message. showInResultsPanel - true to also show the message in a results panel. reportAsError - true to report as error, false to report as warning.
## Method Details

### isShowInResultsPanel

public boolean isShowInResultsPanel()

Check if should also show the message in a results panel.
  Returns: Returns true to also show the message in a results panel.
### isReportAsError

public boolean isReportAsError()

Check if the exception should be reported as an error.
  Returns: Returns true to report as error, false to report as warning.
### setErrorResolver

public void setErrorResolver([ReferenceErrorResolver](ReferenceErrorResolver.md) errorResolver)

Sets a possible solution for the user.
  Parameters: errorResolver - The errorResolver to set.
### getErrorResolver

public [ReferenceErrorResolver](ReferenceErrorResolver.md) getErrorResolver()

Gets a possible solution for the user.
  Returns: Returns a possible solution for the user.
### getShortMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getShortMessage()

Obtain the exception short message.
  Returns: Returns the short message.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
