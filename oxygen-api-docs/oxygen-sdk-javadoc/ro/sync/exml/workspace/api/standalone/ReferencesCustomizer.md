Package [ro.sync.exml.workspace.api.standalone](package-summary.md)

# Interface ReferencesCustomizer
    All Known Subinterfaces: [EclipsePluginWorkspace](../../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [PluginWorkspace](../PluginWorkspace.md), [StandalonePluginWorkspace](StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md)   All Known Implementing Classes: [AuthorComponentFactory](../../../../ecss/extensions/api/component/AuthorComponentFactory.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ReferencesCustomizer
Contains methods for customizing the Input URL Choosers and for computing relative paths from URLs in an implementation specific manner.
  Since: 13
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addInputURLChooserCustomizer](#addInputURLChooserCustomizer(ro.sync.exml.workspace.api.standalone.InputURLChooserCustomizer))([InputURLChooserCustomizer](InputURLChooserCustomizer.md) inputURLChooserCustomizer)
Adds a customizer which can modify the list of "Browse" actions.
  void [addRelativeReferencesResolver](#addRelativeReferencesResolver(java.lang.String,ro.sync.exml.workspace.api.util.RelativeReferenceResolver))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [RelativeReferenceResolver](../util/RelativeReferenceResolver.md) resolver)
Add a relative reference resolver for a certain URL protocol.

## Method Details

### addInputURLChooserCustomizer

void addInputURLChooserCustomizer([InputURLChooserCustomizer](InputURLChooserCustomizer.md) inputURLChooserCustomizer)

Adds a customizer which can modify the list of "Browse" actions. These actions are available in Oxygen, in any control or dialog that contains an URL input box.  **IMPORTANT** This customizer must be set early, when the plugin extension's **applicationStarted** method gets called or after the AuthorComponentFactory was initialized (if running the Author component).  *Example:* If a CMS developer wants the user to choose the URL from their custom CMS chooser then it will add a new action (possibly removing the others). When the new action gets called the custom code shows the custom chooser and at the end it can call the **ro.sync.exml.workspace.api.standalone.InputURLChooser** interface to set the new URL in the combo box.
  Parameters: inputURLChooserCustomizer - The input URL chooser customizer. Since: 12.1
### addRelativeReferencesResolver

void addRelativeReferencesResolver([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol, [RelativeReferenceResolver](../util/RelativeReferenceResolver.md) resolver)

Add a relative reference resolver for a certain URL protocol. This method can be used by a CMS implementor to take control over the way Oxygen is computing relative references for a certain URL protocol. For example when inserting in a DITA Topic a reference to an image Oxygen will try to make the reference relative to the current XML document. If the DITA Topic is opened using your custom URL protocol you can take control over they way in which the relative path is computed.
  Parameters: protocol - The URL protocol for which you want to take control over the relativization. resolver - The custom resolver. Since: 12.2
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
