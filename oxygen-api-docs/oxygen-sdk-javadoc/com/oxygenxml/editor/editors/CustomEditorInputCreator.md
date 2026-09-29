Package [com.oxygenxml.editor.editors](package-summary.md)

# Class CustomEditorInputCreator

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * com.oxygenxml.editor.editors.CustomEditorInputCreator
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class CustomEditorInputCreator extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Abstract class allowed as an extension point to create a custom editor input for resources that the Oxygen plugin tries to open (by clicking on a link in the Author page for example). In your plugin in the plugin.xml you should reference it like:
```

  <extension point="oxygen.plugin.id.customEditorInputCreator">
     <implementation class="my.package.CustomAEditorInputCreatorImpl"/>;
    </extension>

```

  Since: 14.2
## Constructor Summary
 Constructors
Constructor

Description
 [CustomEditorInputCreator](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract org.eclipse.ui.IEditorInput [createCustomEditorInput](#createCustomEditorInput(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) resource)
Create a custom editor input over a certain resource.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CustomEditorInputCreator

public CustomEditorInputCreator()

## Method Details

### createCustomEditorInput

public abstract org.eclipse.ui.IEditorInput createCustomEditorInput([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) resource)

Create a custom editor input over a certain resource.
  Parameters: resource - The resource over which we need to build the editor input. Usually an implementation or instance of: org.eclipse.core.filesystem.IFileStore java.net.URL org.eclipse.core.resources.IStorage Returns: The created editor input or null to go with the default creation procedure.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
