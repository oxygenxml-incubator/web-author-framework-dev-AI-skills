Package [ro.sync.exml.workspace.api.editor.page.author.actions](package-summary.md)

# Class ActionPerformedListener

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.author.actions.ActionPerformedListener
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ActionPerformedListener extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
This listener can be registered for a certain action. The listener will be triggered before an action is performed (and will be able to reject the default code which is executed when the action is performed). The listener will also be triggered after an action is performed.
  Since: 15
## Constructor Summary
 Constructors
Constructor

Description
 [ActionPerformedListener](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [afterActionPerformed](#afterActionPerformed(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) actionEvent)
This callback will be triggered after an action is performed.
  boolean [beforeActionPerformed](#beforeActionPerformed(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) actionEvent)
This callback will be triggered before an action is performed (and will be able to reject the default code which is executed when the action is performed).

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ActionPerformedListener

public ActionPerformedListener()

## Method Details

### beforeActionPerformed

public boolean beforeActionPerformed([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) actionEvent)

This callback will be triggered before an action is performed (and will be able to reject the default code which is executed when the action is performed). If the callback rejects, the other added listeners will also not get called.
  Parameters: actionEvent - The action event. For Swing it is an instance of java.awt.event.ActionEvent. For Eclipse it is an instance of org.eclipse.swt.widgets.Event. Returns: true to let the current action code execute, false to inhibit it.
### afterActionPerformed

public void afterActionPerformed([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) actionEvent)

This callback will be triggered after an action is performed.
  Parameters: actionEvent - The action event. For Swing it is an instance of java.awt.event.ActionEvent. For Eclipse it is an instance of org.eclipse.swt.widgets.Event.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
