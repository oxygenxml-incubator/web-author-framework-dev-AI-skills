Package [com.oxygenxml.editor.editors](package-summary.md)

# Class EditorAdapterContributor

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * com.oxygenxml.editor.editors.EditorAdapterContributor
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class EditorAdapterContributor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Abstract class allowed as an extension point to contribute an adapter to the XML editor. In your plugin in the plugin.xml you should reference it like:
```

  <extension point="oxygen.plugin.id.editorAdapterContributor">
     <implementation class="my.package.CustomEditorAdapterContributor"/>;
    </extension>

```

  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [EditorAdapterContributor](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAdapter](#getAdapter(ro.sync.exml.workspace.api.editor.WSEditor,java.lang.Class))([WSEditor](../../../../ro/sync/exml/workspace/api/editor/WSEditor.md) editor, [Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html) adapter)
Get the extra adapter for the editor.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### EditorAdapterContributor

public EditorAdapterContributor()

## Method Details

### getAdapter

public abstract [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAdapter([WSEditor](../../../../ro/sync/exml/workspace/api/editor/WSEditor.md) editor, [Class](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Class.html) adapter)

Get the extra adapter for the editor.
  Parameters: editor - The editor for which we need an adapter. adapter - The adapter class. Returns: the extra adapter for the editor.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
