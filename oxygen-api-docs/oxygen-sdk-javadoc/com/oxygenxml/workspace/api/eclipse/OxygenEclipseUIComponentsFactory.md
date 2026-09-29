Package [com.oxygenxml.workspace.api.eclipse](package-summary.md)

# Class OxygenEclipseUIComponentsFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * com.oxygenxml.workspace.api.eclipse.OxygenEclipseUIComponentsFactory
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class OxygenEclipseUIComponentsFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Eclipse UI components factory.
  Since: 27.1
## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static void [changeContentType](#changeContentType(org.eclipse.jface.text.source.SourceViewer,java.lang.String))(org.eclipse.jface.text.source.SourceViewer viewer, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)
Change content type if ppossible.
  static org.eclipse.jface.text.source.SourceViewer [createSourceViewer](#createSourceViewer(org.eclipse.swt.widgets.Composite,java.lang.String,boolean,boolean,boolean,boolean,boolean))(org.eclipse.swt.widgets.Composite parent, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentype, boolean wrap, boolean readOnly, boolean verticalScroll, boolean horizontalScroll, boolean border)
Create a source viewer with a specified content type.
  static [TreeModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreeModel.html) [getTreeModel](#getTreeModel(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) tree)
Get the tree model.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### createSourceViewer

public static org.eclipse.jface.text.source.SourceViewer createSourceViewer(org.eclipse.swt.widgets.Composite parent, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentype, boolean wrap, boolean readOnly, boolean verticalScroll, boolean horizontalScroll, boolean border)

Create a source viewer with a specified content type.
  Parameters: parent - The parent composite. contentype - The content type. wrap - If true content wil be wrapped. readOnly - If true the ontent is read only. verticalScroll - If true vertical scroll is visible. horizontalScroll - If true horizontal scroll is visible. border - If true border will be painted. Returns: The source viewer.
### changeContentType

public static void changeContentType(org.eclipse.jface.text.source.SourceViewer viewer, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contentType)

Change content type if ppossible.
  Parameters: viewer - The source viewer. contentType - The new content type.
### getTreeModel

public static [TreeModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/TreeModel.html) getTreeModel([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) tree)

Get the tree model.
  Parameters: tree - The tree. Returns: The model.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
