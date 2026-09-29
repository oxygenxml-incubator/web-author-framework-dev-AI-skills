Package [ro.sync.exml.workspace.api.process](package-summary.md)

# Class ProcessListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.process.ProcessListener
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ProcessListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The process listener. Listens on an executed process.
  Since: 12.1
## Constructor Summary
 Constructors
Constructor

Description
 [ProcessListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete MethodsDeprecated Methods
Modifier and Type

Method

Description
 void [newErrorLine](#newErrorLine(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) line)
Called when the process outputs a line in the System.err
  void [newOutputLine](#newOutputLine(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) line)
Called when the process outputs a line in the System.out
  void [processAboutToStart](#processAboutToStart(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) processName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullCommand)
Called when the process is about to start.
  void [processCouldNotStart](#processCouldNotStart(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Called when the system could not exec the process.
  void [processEnded](#processEnded(int))(int exitCode)
Called when the process ends.
  void [processStarted](#processStarted(java.lang.Process))([Process](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Process.html) process)
Called when the process is started.
  void [processStarted](#processStarted(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) processName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullCommand)  Deprecated.
replaced with processAboutToStart in version 23.1.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProcessListener

public ProcessListener()

## Method Details

### newOutputLine

public void newOutputLine([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) line)

Called when the process outputs a line in the System.out
  Parameters: line - The output line.
### newErrorLine

public void newErrorLine([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) line)

Called when the process outputs a line in the System.err
  Parameters: line - The error line.
### processEnded

public void processEnded(int exitCode)

Called when the process ends.
  Parameters: exitCode - The exit code of the process.
### processStarted

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public void processStarted([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) processName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullCommand)
 Deprecated.
replaced with processAboutToStart in version 23.1.

Called when the process is about to start.
  Parameters: fullCommand - The full command line. processName - The name of process.
### processAboutToStart

public void processAboutToStart([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) processName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fullCommand)

Called when the process is about to start.
  Parameters: fullCommand - The full command line. processName - The name of process. Since: 23.1
### processStarted

public void processStarted([Process](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Process.html) process)

Called when the process is started.
  Parameters: process - The process which started Since: 23.1
### processCouldNotStart

public void processCouldNotStart([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Called when the system could not exec the process.
  Parameters: message - The error message.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
