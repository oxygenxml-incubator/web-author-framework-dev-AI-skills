Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorMouseListener
    All Known Implementing Classes: [AuthorMouseAdapter](AuthorMouseAdapter.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorMouseListener
Interface for the author mouse listeners.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
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

## Method Details

### mouseClicked

void mouseClicked([AuthorMouseEvent](AuthorMouseEvent.md) e)

Invoked when the mouse button has been clicked (pressed and released) on the author page.
  Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md).
### mousePressed

void mousePressed([AuthorMouseEvent](AuthorMouseEvent.md) e)

Invoked when a mouse button has been pressed on the author page.
  Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md).
### mouseReleased

void mouseReleased([AuthorMouseEvent](AuthorMouseEvent.md) e)

Invoked when a mouse button has been released on the author page.
  Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md).
### mouseDragged

void mouseDragged([AuthorMouseEvent](AuthorMouseEvent.md) e)

Invoked when a mouse button is pressed on the author page and then dragged. MOUSE_DRAGGED events will continue to be delivered to the author page where the drag originated until the mouse button is released (regardless of whether the mouse position is within the bounds of the author page).
  Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md).
### mouseMoved

void mouseMoved([AuthorMouseEvent](AuthorMouseEvent.md) e)

Invoked when the mouse cursor has been moved onto the author page but no buttons have been pressed.
  Parameters: e - The [AuthorMouseEvent](AuthorMouseEvent.md).
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
