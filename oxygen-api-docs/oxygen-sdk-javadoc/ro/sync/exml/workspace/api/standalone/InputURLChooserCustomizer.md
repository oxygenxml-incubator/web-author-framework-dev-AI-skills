Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface InputURLChooserCustomizer
    @API(type=EXTENDABLE, src=PUBLIC) public interface InputURLChooserCustomizer
Customize the actions which appear in any Input URL chooser from Oxygen.
  Since: 12.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [customizeBrowseActions](#customizeBrowseActions(java.util.List,ro.sync.exml.workspace.api.standalone.InputURLChooser))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html)> existingBrowseActions, [InputURLChooser](InputURLChooser.md) chooser)
Contribute if necessary to the list of "Browse" actions which appear in any Input URL chooser for Oxygen.

## Method Details

### customizeBrowseActions

void customizeBrowseActions([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[Action](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/Action.html)> existingBrowseActions, [InputURLChooser](InputURLChooser.md) chooser)

Contribute if necessary to the list of "Browse" actions which appear in any Input URL chooser for Oxygen.
  Parameters: existingBrowseActions - The existing list of actions. The first action in the list will be the default one (performed when the drop-down button is clicked).   *Note:* If a new action is added to the browse action list, a custom icon must be set on the action for situations when its text is not used for display. For the Eclipse plugin the instances can be cast to "com.oxygenxml.editor.editors.EclipseActionWrapper" and obtain the internal Eclipse action. To add a new action, just add it inside a new EclipseActionWrapper instance. chooser - The chooser which will get called to set the new URL by the custom code after the user has chosen the new URL.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
