Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class ECPropertiesComposite

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * org.eclipse.swt.widgets.Widget
        * org.eclipse.swt.widgets.Control
            * org.eclipse.swt.widgets.Scrollable
                * org.eclipse.swt.widgets.Composite
                    * ro.sync.ecss.extensions.commons.table.properties.ECPropertiesComposite
   All Implemented Interfaces: org.eclipse.swt.graphics.Drawable, [PropertySelectionController](PropertySelectionController.md)   @API(type=INTERNAL, src=PUBLIC) public class ECPropertiesComposite extends org.eclipse.swt.widgets.Composite implements [PropertySelectionController](PropertySelectionController.md)
Composite corresponding to a tab information. It contains all the properties that will be modified, for a type of elements.

## Field Summary

### Fields inherited from class org.eclipse.swt.widgets.Composite
 embeddedHandle
### Fields inherited from class org.eclipse.swt.widgets.Widget
 handle
## Constructor Summary
 Constructors
Constructor

Description
 [ECPropertiesComposite](#%3Cinit%3E(org.eclipse.swt.widgets.TabFolder,java.util.List,java.lang.String,ro.sync.ecss.extensions.api.AuthorResourceBundle,ro.sync.exml.workspace.api.util.ColorThemeUtilities))(org.eclipse.swt.widgets.TabFolder parent, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextInfo, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md) colorThemeUtilities)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> [getModifiedProperties](#getModifiedProperties())()
Obtain a list with all modified properties for the current panel.
  void [selectionChanged](#selectionChanged(ro.sync.ecss.extensions.commons.table.properties.TableProperty,java.lang.String))([TableProperty](TableProperty.md) property, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)
Method which controls the change of the selected key.

### Methods inherited from class org.eclipse.swt.widgets.Composite
 changed, checkSubclass, drawBackground, getBackgroundMode, getChildren, getLayout, getLayoutDeferred, getTabList, isLayoutDeferred, layout, layout, layout, layout, layout, setBackgroundMode, setFocus, setLayout, setLayoutDeferred, setTabList
### Methods inherited from class org.eclipse.swt.widgets.Scrollable
 computeTrim, getClientArea, getHorizontalBar, getScrollbarsMode, getVerticalBar
### Methods inherited from class org.eclipse.swt.widgets.Control
 addControlListener, addDragDetectListener, addFocusListener, addGestureListener, addHelpListener, addKeyListener, addMenuDetectListener, addMouseListener, addMouseMoveListener, addMouseTrackListener, addMouseWheelListener, addPaintListener, addTouchListener, addTraverseListener, computeSize, computeSize, dragDetect, dragDetect, forceFocus, getAccessible, getBackground, getBackgroundImage, getBorderWidth, getBounds, getCursor, getDragDetect, getEnabled, getFont, getForeground, getLayoutData, getLocation, getMenu, getMonitor, getOrientation, getParent, getRegion, getShell, getSize, getTextDirection, getToolTipText, getTouchEnabled, getVisible, internal_dispose_GC, internal_new_GC, isAutoScalable, isEnabled, isFocusControl, isReparentable, isVisible, moveAbove, moveBelow, pack, pack, print, redraw, redraw, removeControlListener, removeDragDetectListener, removeFocusListener, removeGestureListener, removeHelpListener, removeKeyListener, removeMenuDetectListener, removeMouseListener, removeMouseMoveListener, removeMouseTrackListener, removeMouseWheelListener, removePaintListener, removeTouchListener, removeTraverseListener, requestLayout, setBackground, setBackgroundImage, setBounds, setBounds, setCapture, setCursor, setDragDetect, setEnabled, setFont, setForeground, setLayoutData, setLocation, setLocation, setMenu, setOrientation, setParent, setRedraw, setRegion, setSize, setSize, setTextDirection, setToolTipText, setTouchEnabled, setVisible, toControl, toControl, toDisplay, toDisplay, traverse, traverse, traverse, update
### Methods inherited from class org.eclipse.swt.widgets.Widget
 addDisposeListener, addListener, checkWidget, dispose, getData, getData, getDisplay, getListeners, getStyle, isAutoDirection, isDisposed, isListening, notifyListeners, removeDisposeListener, removeListener, removeListener, reskin, setData, setData, toString
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ECPropertiesComposite

public ECPropertiesComposite(org.eclipse.swt.widgets.TabFolder parent, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextInfo, [AuthorResourceBundle](../../../api/AuthorResourceBundle.md) authorResourceBundle, [ColorThemeUtilities](../../../../../exml/workspace/api/util/ColorThemeUtilities.md) colorThemeUtilities)

Constructor.
  Parameters: parent - The tab folder. properties - The list with properties that will be presented inside the current composite. contextInfo - The context information. It contains information about what is edited inside the current composite. authorResourceBundle - The author resource bundle. colorThemeUtilities - The color theme utilities.
## Method Details

### getModifiedProperties

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> getModifiedProperties()

Obtain a list with all modified properties for the current panel.
  Returns: a [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html) with all modified properties from the current panel.
### selectionChanged

public void selectionChanged([TableProperty](TableProperty.md) property, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newValue)throws [AuthorOperationException](../../../api/AuthorOperationException.md)
 Description copied from interface: [PropertySelectionController](PropertySelectionController.md#selectionChanged(ro.sync.ecss.extensions.commons.table.properties.TableProperty,java.lang.String))
Method which controls the change of the selected key.
  Specified by: [selectionChanged](PropertySelectionController.md#selectionChanged(ro.sync.ecss.extensions.commons.table.properties.TableProperty,java.lang.String)) in interface [PropertySelectionController](PropertySelectionController.md) Parameters: property - The modified property. newValue - The new selected value of the given property Throws: [AuthorOperationException](../../../api/AuthorOperationException.md) - When the handling of selection changed cannot be performed. See Also:
        * [PropertySelectionController.selectionChanged(ro.sync.ecss.extensions.commons.table.properties.TableProperty, java.lang.String)](PropertySelectionController.md#selectionChanged(ro.sync.ecss.extensions.commons.table.properties.TableProperty,java.lang.String))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
