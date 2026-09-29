Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface InplaceEditingTraversalListener
    All Known Subinterfaces: [InplaceEditingListener](InplaceEditingListener.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface InplaceEditingTraversalListener
Gets notified about focus traversal keys TAB and SHIFT-TAB. The next edit position will be computed and edititng will be started. If the editor is a SWING implementation it will only have to provide these notifications if it declares itself a focus cycle root using {Container#setFocusCycleRoot(boolean)}. Otherwise the author panel will intercept this cycle events and handle them automatically. If the editor is a SWT implementation it will have to add a org.eclipse.swt.events.TraverseListener and forward SWT.TRAVERSE_TAB_NEXT and SWT.TRAVERSE_TAB_PREVIOUS events.
  Since: 14.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [nextEditLocationRequested](#nextEditLocationRequested())()
The user requested the next editing location, usually by using the TAB key.
  void [previousEditLocationRequested](#previousEditLocationRequested())()
The user requested the previous editing location, usually by using the SHIFT-TAB key.

## Method Details

### nextEditLocationRequested

void nextEditLocationRequested()

The user requested the next editing location, usually by using the TAB key.

### previousEditLocationRequested

void previousEditLocationRequested()

The user requested the previous editing location, usually by using the SHIFT-TAB key.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
