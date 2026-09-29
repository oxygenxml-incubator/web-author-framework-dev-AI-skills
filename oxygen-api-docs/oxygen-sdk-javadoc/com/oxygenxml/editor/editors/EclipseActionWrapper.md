Package [com.oxygenxml.editor.editors](package-summary.md)

# Class EclipseActionWrapper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * com.oxygenxml.editor.editors.EclipseActionWrapper
   All Implemented Interfaces: [ActionListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionListener.html), [EventListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/EventListener.html), [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html)   @API(type=EXTENDABLE, src=PUBLIC) public class EclipseActionWrapper extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html)
Provides access to an Eclipse action wrapped in a swing action.
  Since: 17
## Field Summary

### Fields inherited from interface javax.swing.[Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html)
 [ACCELERATOR_KEY](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#ACCELERATOR_KEY), [ACTION_COMMAND_KEY](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#ACTION_COMMAND_KEY), [DEFAULT](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#DEFAULT), [DISPLAYED_MNEMONIC_INDEX_KEY](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#DISPLAYED_MNEMONIC_INDEX_KEY), [LARGE_ICON_KEY](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#LARGE_ICON_KEY), [LONG_DESCRIPTION](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#LONG_DESCRIPTION), [MNEMONIC_KEY](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#MNEMONIC_KEY), [NAME](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#NAME), [SELECTED_KEY](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#SELECTED_KEY), [SHORT_DESCRIPTION](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#SHORT_DESCRIPTION), [SMALL_ICON](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#SMALL_ICON)
## Constructor Summary
 Constructors
Constructor

Description
 [EclipseActionWrapper](#%3Cinit%3E(org.eclipse.jface.action.Action))(org.eclipse.jface.action.Action eclipseAction)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [actionPerformed](#actionPerformed(java.awt.event.ActionEvent))([ActionEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionEvent.html) e)

 void [addPropertyChangeListener](#addPropertyChangeListener(java.beans.PropertyChangeListener))([PropertyChangeListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/beans/PropertyChangeListener.html) listener)

 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getValue](#getValue(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

 org.eclipse.jface.action.Action [getWrappedEclipseAction](#getWrappedEclipseAction())()
Get the wrapped Eclipse action.
  boolean [isEnabled](#isEnabled())()

 void [putValue](#putValue(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)

 void [removePropertyChangeListener](#removePropertyChangeListener(java.beans.PropertyChangeListener))([PropertyChangeListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/beans/PropertyChangeListener.html) listener)

 void [setEnabled](#setEnabled(boolean))(boolean enabled)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
### Methods inherited from interface javax.swing.[Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html)
 [accept](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#accept(java.lang.Object))
## Constructor Details

### EclipseActionWrapper

public EclipseActionWrapper(org.eclipse.jface.action.Action eclipseAction)

Constructor.
  Parameters: eclipseAction - The Eclipse action.
## Method Details

### getValue

public [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
  Specified by: [getValue](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#getValue(java.lang.String)) in interface [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) See Also:
        * [Action.getValue(java.lang.String)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#getValue(java.lang.String))

### putValue

public void putValue([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) value)
  Specified by: [putValue](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#putValue(java.lang.String,java.lang.Object)) in interface [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) See Also:
        * [Action.putValue(java.lang.String, java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#putValue(java.lang.String,java.lang.Object))

### setEnabled

public void setEnabled(boolean enabled)
  Specified by: [setEnabled](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#setEnabled(boolean)) in interface [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) See Also:
        * [Action.setEnabled(boolean)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#setEnabled(boolean))

### isEnabled

public boolean isEnabled()
  Specified by: [isEnabled](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#isEnabled()) in interface [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) See Also:
        * [Action.isEnabled()](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#isEnabled())

### addPropertyChangeListener

public void addPropertyChangeListener([PropertyChangeListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/beans/PropertyChangeListener.html) listener)
  Specified by: [addPropertyChangeListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#addPropertyChangeListener(java.beans.PropertyChangeListener)) in interface [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) See Also:
        * [Action.addPropertyChangeListener(java.beans.PropertyChangeListener)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#addPropertyChangeListener(java.beans.PropertyChangeListener))

### removePropertyChangeListener

public void removePropertyChangeListener([PropertyChangeListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/beans/PropertyChangeListener.html) listener)
  Specified by: [removePropertyChangeListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#removePropertyChangeListener(java.beans.PropertyChangeListener)) in interface [Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html) See Also:
        * [Action.removePropertyChangeListener(java.beans.PropertyChangeListener)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html#removePropertyChangeListener(java.beans.PropertyChangeListener))

### actionPerformed

public void actionPerformed([ActionEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionEvent.html) e)
  Specified by: [actionPerformed](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionListener.html#actionPerformed(java.awt.event.ActionEvent)) in interface [ActionListener](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionListener.html) See Also:
        * [ActionListener.actionPerformed(java.awt.event.ActionEvent)](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/event/ActionListener.html#actionPerformed(java.awt.event.ActionEvent))

### getWrappedEclipseAction

public org.eclipse.jface.action.Action getWrappedEclipseAction()

Get the wrapped Eclipse action.
  Returns: the wrapped Eclipse action.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
