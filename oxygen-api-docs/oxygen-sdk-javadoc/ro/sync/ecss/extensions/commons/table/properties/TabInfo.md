Package [ro.sync.ecss.extensions.commons.table.properties](package-summary.md)

# Class TabInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.table.properties.TabInfo
   @API(type=INTERNAL, src=PUBLIC) public class TabInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Information associated with a tab from the 'Table Properties' dialog.

## Constructor Summary
 Constructors
Constructor

Description
 [TabInfo](#%3Cinit%3E(java.lang.String,java.util.List,java.util.List))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes)
Constructor.
  [TabInfo](#%3Cinit%3E(java.lang.String,java.util.List,java.util.List,java.util.List,javax.swing.text.Position%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragmentsToInsert, [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] offsets)
Constructor.
  [TabInfo](#%3Cinit%3E(java.lang.String,java.util.List,java.util.List,java.util.List,javax.swing.text.Position%5B%5D,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragmentsToInsert, [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextInfo)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContextInfo](#getContextInfo())()
Obtain the context information of the current tab.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> [getFragmentsToInsert](#getFragmentsToInsert())()
Get the fragments which will be inserted in the document.
  [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] [getInsertOffsets](#getInsertOffsets())()
Get the position where the fragments will be inserted.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> [getNodes](#getNodes())()
The nodes whose properties will be edited.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> [getProperties](#getProperties())()
Obtain the list with the properties which will be presented in the current tab.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTabKey](#getTabKey())()
Return the tab key name.
  void [setContextInfo](#setContextInfo(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextInfo)
Set the context information.
  void [setFragmentsToInsert](#setFragmentsToInsert(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragmentsToInsert)
Set the fragments which will be inserted in the document.
  void [setInsertOffsets](#setInsertOffsets(javax.swing.text.Position%5B%5D))([Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] positions)
Sets the position where the fragments will be inserted.
  void [setNodes](#setNodes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes)
Set the nodes whose properties will be edited.
  void [setProperties](#setProperties(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties)
Set the list with the properties which will be presented in the current tab.
  void [setTabKey](#setTabKey(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey)
Set the tab key name.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### TabInfo

public TabInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes)

Constructor.
  Parameters: key - The tab key name. If no translation for the tab, then it represents the name of the tab. properties - The list with the properties which will be presented in the current tab. nodes - The nodes whose properties will be edited.
### TabInfo

public TabInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragmentsToInsert, [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] offsets)

Constructor.
  Parameters: key - The tab key name. If no translation for the tab, then it represents the name of the tab. properties - The list with the properties which will be presented in the current tab. nodes - The nodes whose properties will be edited. fragmentsToInsert - The list of [AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)s to be inserted. offsets - The offsets where the new fragments will be inserted.
### TabInfo

public TabInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragmentsToInsert, [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] offsets, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextInfo)

Constructor.
  Parameters: key - The tab key name. If no translation for the tab, then it represents the name of the tab. properties - The list with the properties which will be presented in the current tab. nodes - The nodes whose properties will be edited. fragmentsToInsert - The fragments to be inserted. offsets - The offsets where the new fragments will be inserted. contextInfo - The context information of the current tab. If no context information, then it will be null.
## Method Details

### getTabKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTabKey()

Return the tab key name. If no translation for the tab, then it represents the name of the tab.
  Returns: Returns the tab key.
### setTabKey

public void setTabKey([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) tabKey)

Set the tab key name. If no translation for the tab, then it represents the name of the tab.
  Parameters: tabKey - The new tab Key.
### getProperties

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> getProperties()

Obtain the list with the properties which will be presented in the current tab.
  Returns: Returns the the list with the properties which will be presented in the current tab.
### setProperties

public void setProperties([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[TableProperty](TableProperty.md)> properties)

Set the list with the properties which will be presented in the current tab.
  Parameters: properties - The new properties to set.
### getNodes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> getNodes()

The nodes whose properties will be edited.
  Returns: Returns the nodes whose properties will be edited..
### setNodes

public void setNodes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorElement](../../../api/node/AuthorElement.md)> nodes)

Set the nodes whose properties will be edited.
  Parameters: nodes - The new list of nodes to set.
### getFragmentsToInsert

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> getFragmentsToInsert()

Get the fragments which will be inserted in the document.
  Returns: Returns the fragments which will be inserted in the document.
### setFragmentsToInsert

public void setFragmentsToInsert([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[AuthorDocumentFragment](../../../api/node/AuthorDocumentFragment.md)> fragmentsToInsert)

Set the fragments which will be inserted in the document.
  Parameters: fragmentsToInsert - The fragments which will be inserted in the document.
### getInsertOffsets

public [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] getInsertOffsets()

Get the position where the fragments will be inserted.
  Returns: Returns the position where the fragments will be inserted.
### setInsertOffsets

public void setInsertOffsets([Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] positions)

Sets the position where the fragments will be inserted.
  Parameters: positions - The position where the fragments will be inserted.
### getContextInfo

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContextInfo()

Obtain the context information of the current tab.
  Returns: Returns the context information.
### setContextInfo

public void setContextInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextInfo)

Set the context information.
  Parameters: contextInfo - The context information to set.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
