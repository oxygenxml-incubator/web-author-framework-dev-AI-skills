Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface InputURLChooser
    All Superinterfaces: [ContextDescriptionProvider](ContextDescriptionProvider.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface InputURLChooserextends [ContextDescriptionProvider](ContextDescriptionProvider.md)
Interface through which the CMS can set a custom URL to any Input URL Panel from Oxygen.
  Since: 12.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [OPEN_RESOURCE](#OPEN_RESOURCE)
Open resource chooser
  static final int [OPEN_RESOURCE_DIRECTORY](#OPEN_RESOURCE_DIRECTORY)
Resource directory chooser
  static final int [SAVE_RESOURCE](#SAVE_RESOURCE)
Save resource chooser

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getBrowseMode](#getBrowseMode())()
Get the mode for which the Input URL chooser will be used (for opening or for saving resources).
  [ResourceFilter](ResourceFilter.md)[] [getResourceFilters](#getResourceFilters())()
Get the list of resource filters used for the local file chooser.
  void [urlChosen](#urlChosen(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) selectedURL)
Set in the Input URL panel combo box the new URL which was chosen from the CMS handler.

### Methods inherited from interface ro.sync.exml.workspace.api.standalone.[ContextDescriptionProvider](ContextDescriptionProvider.md)
 [getAttributeEditingContextDescription](ContextDescriptionProvider.md#getAttributeEditingContextDescription()), [getContextDescription](ContextDescriptionProvider.md#getContextDescription())
## Field Details

### SAVE_RESOURCE

static final int SAVE_RESOURCE

Save resource chooser
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.InputURLChooser.SAVE_RESOURCE)

### OPEN_RESOURCE

static final int OPEN_RESOURCE

Open resource chooser
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.InputURLChooser.OPEN_RESOURCE)

### OPEN_RESOURCE_DIRECTORY

static final int OPEN_RESOURCE_DIRECTORY

Resource directory chooser
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.standalone.InputURLChooser.OPEN_RESOURCE_DIRECTORY)

## Method Details

### urlChosen

void urlChosen([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) selectedURL)

Set in the Input URL panel combo box the new URL which was chosen from the CMS handler. When the customizer is used in places where a combo box for the URL is not present (like in the DITA Maps Manager view) this method performs the operation on the given URL.
  Parameters: selectedURL - The URL which was probably selected by the user in a custom CMS chooser.
### getBrowseMode

int getBrowseMode()

Get the mode for which the Input URL chooser will be used (for opening or for saving resources).
  Returns: One of the constants in this class: [OPEN_RESOURCE](#OPEN_RESOURCE), [SAVE_RESOURCE](#SAVE_RESOURCE) or [OPEN_RESOURCE_DIRECTORY](#OPEN_RESOURCE_DIRECTORY) Since: 12.2
### getResourceFilters

[ResourceFilter](ResourceFilter.md)[] getResourceFilters()

Get the list of resource filters used for the local file chooser. This method is useful to decide the type of files the chooser dialog wants to browse. For example if the dialog wants to select an image to add to the Author page then the resource filters will contain image extensions.
  Returns: The list of resource filters used for the local file chooser. Can be null. Since: 13.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
