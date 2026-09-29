Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorMouseAdapter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorMouseAdapter
   All Implemented Interfaces: [AuthorMouseListener](AuthorMouseListener.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorMouseAdapter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [AuthorMouseListener](AuthorMouseListener.md)
Empty implementation of the [AuthorMouseListener](AuthorMouseListener.md).

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorMouseAdapter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [mouseClicked](#mouseClicked(ro.sync.ecss.extensions.api.AuthorMouseEvent))([AuthorMouseEvent](AuthorMouseEvent.md) e)
Invoked when the mouse button has been clicked (pressed and released) on the author page.
  void [mouseDragged](#mouseDragged(ro.sync.ecss.extensions.api.AuthorMouseEvent))([AuthorMouseEvent](AuthorMouseEvent.md) e)
Invoked when a mouse button is pressed on the author page and then dragged.
  void [mouseMoved](#mouseMoved(ro.sync.ecss.extensions.api.AuthorMouseEvent))([AuthorMouseEvent](AuthorMouseEvent.md) e)
Invoked when the mouse cursor has been moved onto the author page but no buttons have been pressed.
  void [mousePressed](#mousePressed(ro.sync.ecss.extensions.api.AuthorMouseEvent))([AuthorMouseEvent](AuthorMouseEvent.md) e)
Invoked when a mouse button has been pressed on the author page.
  void [mouseReleased](#mouseReleased(ro.sync.ecss.extensions.api.AuthorMouseEvent))([AuthorMouseEvent](AuthorMouseEvent.md) e)
Invoked when a mouse button has been released on the author page.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorMouseAdapter

public AuthorMouseAdapter()

## Method Details

### mouseClicked

public void mouseClicked([AuthorMouseEvent](AuthorMouseEvent.md) e)
 Description copied from interface: [AuthorMouseListener](AuthorMouseListener.md#mouseClicked(ro.sync.ecss.extensions.api.AuthorMouseEvent))
Invoked when the mouse button has been clicked (pressed and released) on the author page.
  Specified by: [mouseClicked](AuthorMouseListener.md#mouseClicked(ro.sync.ecss.extensions.api.AuthorMouseEvent)) in interface [AuthorMouseListener](AuthorMouseListener.md) Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md). See Also:
        * [AuthorMouseListener.mouseClicked(ro.sync.ecss.extensions.api.AuthorMouseEvent)](AuthorMouseListener.md#mouseClicked(ro.sync.ecss.extensions.api.AuthorMouseEvent))

### mouseDragged

public void mouseDragged([AuthorMouseEvent](AuthorMouseEvent.md) e)
 Description copied from interface: [AuthorMouseListener](AuthorMouseListener.md#mouseDragged(ro.sync.ecss.extensions.api.AuthorMouseEvent))
Invoked when a mouse button is pressed on the author page and then dragged. MOUSE_DRAGGED events will continue to be delivered to the author page where the drag originated until the mouse button is released (regardless of whether the mouse position is within the bounds of the author page).
  Specified by: [mouseDragged](AuthorMouseListener.md#mouseDragged(ro.sync.ecss.extensions.api.AuthorMouseEvent)) in interface [AuthorMouseListener](AuthorMouseListener.md) Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md). See Also:
        * [AuthorMouseListener.mouseDragged(ro.sync.ecss.extensions.api.AuthorMouseEvent)](AuthorMouseListener.md#mouseDragged(ro.sync.ecss.extensions.api.AuthorMouseEvent))

### mouseMoved

public void mouseMoved([AuthorMouseEvent](AuthorMouseEvent.md) e)
 Description copied from interface: [AuthorMouseListener](AuthorMouseListener.md#mouseMoved(ro.sync.ecss.extensions.api.AuthorMouseEvent))
Invoked when the mouse cursor has been moved onto the author page but no buttons have been pressed.
  Specified by: [mouseMoved](AuthorMouseListener.md#mouseMoved(ro.sync.ecss.extensions.api.AuthorMouseEvent)) in interface [AuthorMouseListener](AuthorMouseListener.md) Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md). See Also:
        * [AuthorMouseListener.mouseMoved(ro.sync.ecss.extensions.api.AuthorMouseEvent)](AuthorMouseListener.md#mouseMoved(ro.sync.ecss.extensions.api.AuthorMouseEvent))

### mousePressed

public void mousePressed([AuthorMouseEvent](AuthorMouseEvent.md) e)
 Description copied from interface: [AuthorMouseListener](AuthorMouseListener.md#mousePressed(ro.sync.ecss.extensions.api.AuthorMouseEvent))
Invoked when a mouse button has been pressed on the author page.
  Specified by: [mousePressed](AuthorMouseListener.md#mousePressed(ro.sync.ecss.extensions.api.AuthorMouseEvent)) in interface [AuthorMouseListener](AuthorMouseListener.md) Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md). See Also:
        * [AuthorMouseListener.mousePressed(ro.sync.ecss.extensions.api.AuthorMouseEvent)](AuthorMouseListener.md#mousePressed(ro.sync.ecss.extensions.api.AuthorMouseEvent))

### mouseReleased

public void mouseReleased([AuthorMouseEvent](AuthorMouseEvent.md) e)
 Description copied from interface: [AuthorMouseListener](AuthorMouseListener.md#mouseReleased(ro.sync.ecss.extensions.api.AuthorMouseEvent))
Invoked when a mouse button has been released on the author page.
  Specified by: [mouseReleased](AuthorMouseListener.md#mouseReleased(ro.sync.ecss.extensions.api.AuthorMouseEvent)) in interface [AuthorMouseListener](AuthorMouseListener.md) Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md). See Also:
        * [AuthorMouseListener.mouseReleased(ro.sync.ecss.extensions.api.AuthorMouseEvent)](AuthorMouseListener.md#mouseReleased(ro.sync.ecss.extensions.api.AuthorMouseEvent))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
