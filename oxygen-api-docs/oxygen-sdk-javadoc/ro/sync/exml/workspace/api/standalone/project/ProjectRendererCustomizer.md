Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Class ProjectRendererCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.standalone.project.ProjectRendererCustomizer
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class ProjectRendererCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Base class which can be extended to customize the rendering of the files from the Project view in the stand-alone Oxygen installation.
  Since: 20
## Constructor Summary
 Constructors
Constructor

Description
 [ProjectRendererCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) [getDecorationIcon](#getDecorationIcon(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) projectFile)
Get the decoration icon for a certain file shown in the Project view.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName(java.io.File,java.lang.String))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) projectFile, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultName)
Get the custom name for a certain file shown in the Project view.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTooltip](#getTooltip(java.io.File,java.lang.String))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) projectFile, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultTooltip)
Get the custom tooltip for a certain file shown in the Project view.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ProjectRendererCustomizer

public ProjectRendererCustomizer()

## Method Details

### getDecorationIcon

public [Icon](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Icon.html) getDecorationIcon([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) projectFile)

Get the decoration icon for a certain file shown in the Project view. This callback comes very often, each time the Project Swing JTree is repainted, so the developers implementing it need to develop their own internal caches.
  Parameters: projectFile - The file in the Project view. Returns: the decoration icon or null if the default should be used instead. The decoration icon should be about 10x10 pixels.
### getTooltip

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTooltip([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) projectFile, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultTooltip)

Get the custom tooltip for a certain file shown in the Project view. This callback comes very often, each time the Project Swing JTree is repainted, so the developers implementing it need to develop their own internal caches.
  Parameters: projectFile - The file in the Project view. defaultTooltip - The default tooltip. Returns: the custom tooltip for a certain File shown in the Project view or null if the default should be used instead.
### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) projectFile, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultName)

Get the custom name for a certain file shown in the Project view. This callback comes very often, each time the Project Swing JTree is repainted, so the developers implementing it need to develop their own internal caches.
  Parameters: projectFile - The file in the Project view. defaultName - The default name. Returns: the custom name for a certain File shown in the Project view or null if the default should be used instead.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
