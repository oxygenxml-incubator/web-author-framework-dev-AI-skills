Package [ro.sync.exml.workspace.api.process](package-summary.md)

# Interface ProcessController
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ProcessController
The process controller. Can be used to start or stop it.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [sendMessage](#sendMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Send a message to the process.
  void [start](#start())()
Start the process.
  void [stop](#stop())()
Stop the process, calls java.lang.Process.distroy().

## Method Details

### start

void start()

Start the process. This method blocks until the process ends.

### stop

void stop()

Stop the process, calls java.lang.Process.distroy(). Will also kill sub-processes.

### sendMessage

void sendMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Send a message to the process. The message will be sent "UTF-8" encoded via the java.lang.Process.getOutputStream().
  Parameters: message - The message. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) - Thrown when the process was not started for some reason.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
