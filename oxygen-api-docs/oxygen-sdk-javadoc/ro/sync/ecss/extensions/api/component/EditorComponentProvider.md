Package [ro.sync.ecss.extensions.api.component](package-summary.md)

# Interface EditorComponentProvider
    All Superinterfaces: [ComponentProvider](ComponentProvider.md)   All Known Implementing Classes: [AbstractComponentProvider](AbstractComponentProvider.md), [AuthorComponentProvider](AuthorComponentProvider.md), [GenericEditorComponentProvider](GenericEditorComponentProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface EditorComponentProviderextends [ComponentProvider](ComponentProvider.md)
Provides access to a created editor + helper views and additional panels. The editor might have multiple editor pages.
  Since: 14.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [ATTRIBUTES_PANEL_ID](#ATTRIBUTES_PANEL_ID)
Attributes Panel
  static final int [ELEMENTS_PANEL_ID](#ELEMENTS_PANEL_ID)
Elements Panel
  static final int [ENTITIES_PANEL_ID](#ENTITIES_PANEL_ID)
Entities Panel
  static final int [MODEL_PANEL_ID](#MODEL_PANEL_ID)
Model Panel
  static final int [OUTLINER_PANEL_ID](#OUTLINER_PANEL_ID)
Outliner Panel
  static final int [REVIEWS_PANEL_ID](#REVIEWS_PANEL_ID)
Reviews Panel

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addAuthorComponentListener](#addAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener))([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)
Adds an author component listener.
  [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) [getAdditionalEditHelper](#getAdditionalEditHelper(int))(int helperID)
Get an additional edit helper panel.
  void [removeAuthorComponentListener](#removeAuthorComponentListener(ro.sync.ecss.extensions.api.component.listeners.AuthorComponentListener))([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)
Removes an author component listener.
  void [showLocation](#showLocation(java.net.URL,java.io.Reader))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)
Show the location referenced by a given URL in the editor.

### Methods inherited from interface ro.sync.ecss.extensions.api.component.[ComponentProvider](ComponentProvider.md)
 [getEditorComponent](ComponentProvider.md#getEditorComponent()), [getStatusComponent](ComponentProvider.md#getStatusComponent()), [getWSEditorAccess](ComponentProvider.md#getWSEditorAccess()), [load](ComponentProvider.md#load(java.net.URL,java.io.Reader)), [print](ComponentProvider.md#print(boolean))
## Field Details

### OUTLINER_PANEL_ID

static final int OUTLINER_PANEL_ID

Outliner Panel
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.component.EditorComponentProvider.OUTLINER_PANEL_ID)

### ATTRIBUTES_PANEL_ID

static final int ATTRIBUTES_PANEL_ID

Attributes Panel
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.component.EditorComponentProvider.ATTRIBUTES_PANEL_ID)

### MODEL_PANEL_ID

static final int MODEL_PANEL_ID

Model Panel
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.component.EditorComponentProvider.MODEL_PANEL_ID)

### ELEMENTS_PANEL_ID

static final int ELEMENTS_PANEL_ID

Elements Panel
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.component.EditorComponentProvider.ELEMENTS_PANEL_ID)

### ENTITIES_PANEL_ID

static final int ENTITIES_PANEL_ID

Entities Panel
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.component.EditorComponentProvider.ENTITIES_PANEL_ID)

### REVIEWS_PANEL_ID

static final int REVIEWS_PANEL_ID

Reviews Panel
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.component.EditorComponentProvider.REVIEWS_PANEL_ID)

## Method Details

### showLocation

void showLocation([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url, [Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) reader)throws [AuthorComponentException](AuthorComponentException.md)

Show the location referenced by a given URL in the editor. If the document pointed by this URL is different than the document currently loaded in the editor page, this URL will be used to set the content to edit, to solve relative references (eg: images) and to show the location pointed by the URL reference part. If the document pointed by this URL is currently loaded in the editor page, only the reference part of the given URL will be used to show the corresponding location in the editor.
  Parameters: url - The URL to show location for. reader - The reader over the URL, can be null. Throws: [AuthorComponentException](AuthorComponentException.md) - When there was a load problem (eg: IOException).
### addAuthorComponentListener

void addAuthorComponentListener([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)

Adds an author component listener.
  Parameters: listener - The listener.
### removeAuthorComponentListener

void removeAuthorComponentListener([AuthorComponentListener](listeners/AuthorComponentListener.md) listener)

Removes an author component listener.
  Parameters: listener - The listener.
### getAdditionalEditHelper

[JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) getAdditionalEditHelper(int helperID)

Get an additional edit helper panel. It can be the outline, attributes, entities, elements or model helper component, depending on the ID.
  Parameters: helperID - One of:
        * ATTRIBUTES_PANEL_ID,
        * ELEMENTS_PANEL_ID,
        * ENTITIES_PANEL_ID,
        * MODEL_PANEL_ID,
        * OUTLINER_PANEL_ID constants.
 Returns: The additional component.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
