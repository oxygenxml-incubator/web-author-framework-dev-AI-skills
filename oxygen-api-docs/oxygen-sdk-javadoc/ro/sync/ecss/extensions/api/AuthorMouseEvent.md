Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorMouseEvent

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.ecss.extensions.api.AuthorInputEvent](AuthorInputEvent.md)
        * ro.sync.ecss.extensions.api.AuthorMouseEvent
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorMouseEvent extends [AuthorInputEvent](AuthorInputEvent.md)
Mouse event received by the [AuthorMouseListener](AuthorMouseListener.md).

## Field Summary
 Fields
Modifier and Type

Field

Description
 final int [button](#button)
Indicates which, if any, of the mouse buttons has changed its state.
  static final int [BUTTON1](#BUTTON1)
Indicates mouse button #1.
  static final int [BUTTON2](#BUTTON2)
Indicates mouse button #2.
  static final int [BUTTON3](#BUTTON3)
Indicates mouse button #3.
  final int [clickCount](#clickCount)
Click count.
  static final int [NOBUTTON](#NOBUTTON)
Indicates no mouse button.
  final boolean [popupTrigger](#popupTrigger)
true if this event is a pop-up trigger.
  final int [state](#state)
One of the constants [STATE_PRESSED](#STATE_PRESSED), [STATE_RELEASED](#STATE_RELEASED), [STATE_CLICKED](#STATE_CLICKED), [STATE_MOVED](#STATE_MOVED) or [STATE_DRAGGED](#STATE_DRAGGED).
  static final int [STATE_CLICKED](#STATE_CLICKED)
Mouse clicked event type.
  static final int [STATE_DRAGGED](#STATE_DRAGGED)
Mouse dragged event type.
  static final int [STATE_MOVED](#STATE_MOVED)
Mouse moved event type.
  static final int [STATE_PRESSED](#STATE_PRESSED)
Mouse pressed event type.
  static final int [STATE_RELEASED](#STATE_RELEASED)
Mouse released event type.
  static final int [STATE_WHEEL_MOVED](#STATE_WHEEL_MOVED)
Mouse wheel moved event type.
  final boolean [wheelUp](#wheelUp)
true if the mouse wheel is rotated up (away from the user), falseif the mouse wheel is rotated down (towards the user).
  final int [X](#X)
The mouse event's x coordinate.
  final int [Y](#Y)
The mouse event's y coordinate.

### Fields inherited from class ro.sync.ecss.extensions.api.[AuthorInputEvent](AuthorInputEvent.md)
 [ALT_GRAPH_PRESSED](AuthorInputEvent.md#ALT_GRAPH_PRESSED), [ALT_PRESSED](AuthorInputEvent.md#ALT_PRESSED), [consumed](AuthorInputEvent.md#consumed), [CTRL_PRESSED](AuthorInputEvent.md#CTRL_PRESSED), [META_PRESSED](AuthorInputEvent.md#META_PRESSED), [modifiers](AuthorInputEvent.md#modifiers), [SHIFT_PRESSED](AuthorInputEvent.md#SHIFT_PRESSED)
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorMouseEvent](#%3Cinit%3E(int,int,boolean,int,int,int))(int x, int y, boolean isPopupTrigger, int state, int modifiers, int clickCount)
Constructor for the author mouse event.
  [AuthorMouseEvent](#%3Cinit%3E(int,int,boolean,int,int,int,int))(int x, int y, boolean isPopupTrigger, int state, int modifiers, int clickCount, int button)
Constructor for the author mouse event.
  [AuthorMouseEvent](#%3Cinit%3E(int,int,boolean,int,int,int,int,boolean))(int x, int y, boolean isPopupTrigger, int state, int modifiers, int clickCount, int button, boolean wheelUp)
Constructor for the author mouse event.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getButton](#getButton())()
Returns which, if any, of the mouse buttons has changed state.
  int [getClickCount](#getClickCount())()
Returns the number of mouse clicks associated with this event.
  int [getState](#getState())()
Returns the state.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getStateDescription](#getStateDescription(int))(int state)

 int [getX](#getX())()
Returns the horizontal x position of the event relative to the source component.
  int [getY](#getY())()
Returns the vertical y position of the event relative to the source component.
  boolean [isPopupTrigger](#isPopupTrigger())()
Returns whether or not this mouse event is the popup menu trigger event for the platform.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class ro.sync.ecss.extensions.api.[AuthorInputEvent](AuthorInputEvent.md)
 [consume](AuthorInputEvent.md#consume()), [getModifiers](AuthorInputEvent.md#getModifiers()), [isAltGraphPressed](AuthorInputEvent.md#isAltGraphPressed()), [isAltPressed](AuthorInputEvent.md#isAltPressed()), [isCommandPressed](AuthorInputEvent.md#isCommandPressed()), [isCommandPressed](AuthorInputEvent.md#isCommandPressed(int)), [isConsumed](AuthorInputEvent.md#isConsumed()), [isCtrlPressed](AuthorInputEvent.md#isCtrlPressed()), [isMetaPressed](AuthorInputEvent.md#isMetaPressed()), [isShiftPressed](AuthorInputEvent.md#isShiftPressed())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### STATE_PRESSED

public static final int STATE_PRESSED

Mouse pressed event type. The value is 1.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.STATE_PRESSED)

### STATE_RELEASED

public static final int STATE_RELEASED

Mouse released event type. The value is 2.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.STATE_RELEASED)

### STATE_CLICKED

public static final int STATE_CLICKED

Mouse clicked event type. The value is 3.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.STATE_CLICKED)

### STATE_MOVED

public static final int STATE_MOVED

Mouse moved event type. The value is 4.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.STATE_MOVED)

### STATE_DRAGGED

public static final int STATE_DRAGGED

Mouse dragged event type. The value is 5.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.STATE_DRAGGED)

### STATE_WHEEL_MOVED

public static final int STATE_WHEEL_MOVED

Mouse wheel moved event type. The value is 6.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.STATE_WHEEL_MOVED)

### BUTTON1

public static final int BUTTON1

Indicates mouse button #1. The value is 1.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.BUTTON1)

### BUTTON2

public static final int BUTTON2

Indicates mouse button #2. The value is 2.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.BUTTON2)

### BUTTON3

public static final int BUTTON3

Indicates mouse button #3. The value is 3.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.BUTTON3)

### NOBUTTON

public static final int NOBUTTON

Indicates no mouse button. The value is 0.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.ecss.extensions.api.AuthorMouseEvent.NOBUTTON)

### X

public final int X

The mouse event's x coordinate. The x value is relative to the author page.

### Y

public final int Y

The mouse event's y coordinate. The y value is relative to the author page.

### popupTrigger

public final boolean popupTrigger

true if this event is a pop-up trigger.

### clickCount

public final int clickCount

Click count.

### button

public final int button

Indicates which, if any, of the mouse buttons has changed its state. The only legal values are the following constants: NOBUTTON, BUTTON1, BUTTON2 or BUTTON3.

### state

public final int state

One of the constants [STATE_PRESSED](#STATE_PRESSED), [STATE_RELEASED](#STATE_RELEASED), [STATE_CLICKED](#STATE_CLICKED), [STATE_MOVED](#STATE_MOVED) or [STATE_DRAGGED](#STATE_DRAGGED).

### wheelUp

public final boolean wheelUp

true if the mouse wheel is rotated up (away from the user), falseif the mouse wheel is rotated down (towards the user).

## Constructor Details

### AuthorMouseEvent

public AuthorMouseEvent(int x, int y, boolean isPopupTrigger, int state, int modifiers, int clickCount)

Constructor for the author mouse event.
  Parameters: x - The x coordinate of the mouse event. y - The y coordinate of the mouse event. isPopupTrigger - true if it is pop-up trigger. state - One of the constants [STATE_PRESSED](#STATE_PRESSED), [STATE_RELEASED](#STATE_RELEASED), [STATE_CLICKED](#STATE_CLICKED), [STATE_MOVED](#STATE_MOVED) or [STATE_DRAGGED](#STATE_DRAGGED). modifiers - Marks if CTRL, SHIFT, ALT, ALT GR, META were pressed. clickCount - Click count.
### AuthorMouseEvent

public AuthorMouseEvent(int x, int y, boolean isPopupTrigger, int state, int modifiers, int clickCount, int button)

Constructor for the author mouse event.
  Parameters: x - The x coordinate of the mouse event. y - The y coordinate of the mouse event. isPopupTrigger - true if it is pop-up trigger. state - One of the constants [STATE_PRESSED](#STATE_PRESSED), [STATE_RELEASED](#STATE_RELEASED), [STATE_CLICKED](#STATE_CLICKED), [STATE_MOVED](#STATE_MOVED) or [STATE_DRAGGED](#STATE_DRAGGED). modifiers - Marks if CTRL, SHIFT, ALT, ALT GR, META were pressed. clickCount - Click count. button - One of the constants [BUTTON1](#BUTTON1), [BUTTON2](#BUTTON2), [BUTTON3](#BUTTON3), [NOBUTTON](#NOBUTTON).
### AuthorMouseEvent

public AuthorMouseEvent(int x, int y, boolean isPopupTrigger, int state, int modifiers, int clickCount, int button, boolean wheelUp)

Constructor for the author mouse event.
  Parameters: x - The x coordinate of the mouse event. y - The y coordinate of the mouse event. isPopupTrigger - true if it is pop-up trigger. state - One of the constants [STATE_PRESSED](#STATE_PRESSED), [STATE_RELEASED](#STATE_RELEASED), [STATE_CLICKED](#STATE_CLICKED), [STATE_MOVED](#STATE_MOVED) or [STATE_DRAGGED](#STATE_DRAGGED). modifiers - Marks if CTRL, SHIFT, ALT, ALT GR, META were pressed. clickCount - Click count. button - One of the constants [BUTTON1](#BUTTON1), [BUTTON2](#BUTTON2), [BUTTON3](#BUTTON3), [NOBUTTON](#NOBUTTON). wheelUp - true if the mouse wheel is rotated up (away from the user), false if the mouse wheel is rotated down (towards the user).
## Method Details

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

### getStateDescription

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getStateDescription(int state)
  Returns: String representation for mouse state.
### getClickCount

public int getClickCount()

Returns the number of mouse clicks associated with this event.
  Returns: integer value for the number of clicks
### getButton

public int getButton()

Returns which, if any, of the mouse buttons has changed state.
  Returns: one of the following constants: NOBUTTON, BUTTON1, BUTTON2 or BUTTON3.
### isPopupTrigger

public boolean isPopupTrigger()

Returns whether or not this mouse event is the popup menu trigger event for the platform.
**Note**: Popup menus are triggered differently on different systems. Therefore, isPopupTriggershould be checked in both mousePressedand mouseReleasedfor proper cross-platform functionality.

  Returns: boolean, true if this event is the popup menu trigger for this platform
### getX

public int getX()

Returns the horizontal x position of the event relative to the source component.
  Returns: x an integer indicating horizontal position relative to the component
### getY

public int getY()

Returns the vertical y position of the event relative to the source component.
  Returns: y an integer indicating vertical position relative to the component
### getState

public int getState()

Returns the state.
  Returns: one of the following constants: STATE_PRESSED, STATE_RELEASED, STATE_CLICKED STATE_DRAGGED or STATE_MOVED.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
