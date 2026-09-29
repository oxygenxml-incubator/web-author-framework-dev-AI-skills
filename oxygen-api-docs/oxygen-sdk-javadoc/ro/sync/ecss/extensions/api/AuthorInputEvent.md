Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorInputEvent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorInputEvent
   Direct Known Subclasses: [AuthorMouseEvent](AuthorMouseEvent.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public abstract class AuthorInputEvent extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Base class for Author input events.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [ALT_GRAPH_PRESSED](#ALT_GRAPH_PRESSED)
This flag indicates that the AltGraph key was down when the event occurred.
  static final int [ALT_PRESSED](#ALT_PRESSED)
This flag indicates that the Alt key was down when the event occurred.
  boolean [consumed](#consumed)
States whether or not the event has been consumed.
  static final int [CTRL_PRESSED](#CTRL_PRESSED)
This flag indicates that the Control key was down when the event occurred.
  static final int [META_PRESSED](#META_PRESSED)
This flag indicates that the Meta key was down when the event occurred.
  final int [modifiers](#modifiers)
The state of the modifier mask at the time the input event was fired.
  static final int [SHIFT_PRESSED](#SHIFT_PRESSED)
This flag indicates that the Shift key was down when the event occurred.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorInputEvent](#%3Cinit%3E(int))(int modifiers)
Constructor for author input event.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [consume](#consume())()
Set the consumed flag for the event.
  int [getModifiers](#getModifiers())()

 final boolean [isAltGraphPressed](#isAltGraphPressed())()

 final boolean [isAltPressed](#isAltPressed())()

 final boolean [isCommandPressed](#isCommandPressed())()
Check if META is pressed on Mac or CTRL is pressed on Windows.
  static boolean [isCommandPressed](#isCommandPressed(int))(int modifiers)
Check if META is pressed on Mac or CTRL is pressed on Windows.
  final boolean [isConsumed](#isConsumed())()

 final boolean [isCtrlPressed](#isCtrlPressed())()

 final boolean [isMetaPressed](#isMetaPressed())()

 boolean [isShiftPressed](#isShiftPressed())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### SHIFT_PRESSED

public static final int SHIFT_PRESSED

This flag indicates that the Shift key was down when the event occurred. The value is 1 << 0.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorInputEvent.SHIFT_PRESSED)

### CTRL_PRESSED

public static final int CTRL_PRESSED

This flag indicates that the Control key was down when the event occurred. The value is 1 << 1.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorInputEvent.CTRL_PRESSED)

### META_PRESSED

public static final int META_PRESSED

This flag indicates that the Meta key was down when the event occurred. The value is 1 << 2.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorInputEvent.META_PRESSED)

### ALT_PRESSED

public static final int ALT_PRESSED

This flag indicates that the Alt key was down when the event occurred. The value is 1 << 3.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorInputEvent.ALT_PRESSED)

### ALT_GRAPH_PRESSED

public static final int ALT_GRAPH_PRESSED

This flag indicates that the AltGraph key was down when the event occurred. The value is 1 << 5.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorInputEvent.ALT_GRAPH_PRESSED)

### modifiers

public final int modifiers

The state of the modifier mask at the time the input event was fired.

### consumed

public boolean consumed

States whether or not the event has been consumed.

## Constructor Details

### AuthorInputEvent

public AuthorInputEvent(int modifiers)

Constructor for author input event.
  Parameters: modifiers - The modifiers.
## Method Details

### consume

public void consume()

Set the consumed flag for the event.

### isConsumed

public final boolean isConsumed()
  Returns: true if the event was consumed.
### isShiftPressed

public boolean isShiftPressed()
  Returns: true if SHIFT key was pressed.
### isCtrlPressed

public final boolean isCtrlPressed()
  Returns: true if CTRL key was pressed.
### isAltPressed

public final boolean isAltPressed()
  Returns: true if ALT key was pressed.
### isAltGraphPressed

public final boolean isAltGraphPressed()
  Returns: true if ALT GR key was pressed.
### isMetaPressed

public final boolean isMetaPressed()
  Returns: true if META key was pressed.
### getModifiers

public int getModifiers()
  Returns: Returns the keyboard modifiers associated with the event.
### isCommandPressed

public final boolean isCommandPressed()

Check if META is pressed on Mac or CTRL is pressed on Windows.
  Returns: true if META is pressed on Mac or CTRL is pressed on Windows.
### isCommandPressed

public static boolean isCommandPressed(int modifiers)

Check if META is pressed on Mac or CTRL is pressed on Windows.
  Parameters: modifiers - The modifiers Returns: true if META is pressed on Mac or CTRL is pressed on Windows.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
