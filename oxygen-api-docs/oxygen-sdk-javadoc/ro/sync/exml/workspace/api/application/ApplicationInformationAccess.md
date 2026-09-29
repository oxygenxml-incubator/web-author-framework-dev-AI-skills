Package [ro.sync.exml.workspace.api.application](package-summary.md)

# Interface ApplicationInformationAccess
    All Known Subinterfaces: [AuthorWorkspaceAccess](../../../../ecss/extensions/api/access/AuthorWorkspaceAccess.md), [EclipsePluginWorkspace](../../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [PluginWorkspace](../PluginWorkspace.md), [StandalonePluginWorkspace](../standalone/StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md), [Workspace](../Workspace.md), [WorkspaceUtilities](../WorkspaceUtilities.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ApplicationInformationAccess
Access to various details about the application. One way to obtain an implementation from a plugin is:
```

 ApplicationInformationAccess info = PluginWorkspaceProvider.getPluginWorkspace();

```

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getApplicationName](#getApplicationName())()
Get the display name of the application.
  [ApplicationType](ApplicationType.md) [getApplicationType](#getApplicationType())()
Get the type of the application.
  ro.sync.exml.workspace.api.license.LicenseInformationProvider [getLicenseInformationProvider](#getLicenseInformationProvider())()
Get information about the license used in the current Oxygen application.
  [Platform](../Platform.md) [getPlatform](#getPlatform())()
Return the oXygen platform that is currently running.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPreferencesDirectory](#getPreferencesDirectory())()
Get the options directory where the Oxygen preferences are saved.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getUserInterfaceLanguage](#getUserInterfaceLanguage())()
Get the language used to display the GUI controls (buttons, label) in Oxygen.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getVersion](#getVersion())()
Get the current version of the Oxygen/Author product.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getVersionBuildID](#getVersionBuildID())()
Get the build ID of the current application.

## Method Details

### getLicenseInformationProvider

ro.sync.exml.workspace.api.license.LicenseInformationProvider getLicenseInformationProvider()

Get information about the license used in the current Oxygen application.
  Returns: The license information provider Since: 12.1
### getPreferencesDirectory

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPreferencesDirectory()

Get the options directory where the Oxygen preferences are saved. Can be used to save additional user data there.
  Returns: the directory where the Oxygen preferences are saved. Returns a string like: c:\\Documents and Settings\\username\\com.oxygenxml Since: 12.1
### getUserInterfaceLanguage

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getUserInterfaceLanguage()

Get the language used to display the GUI controls (buttons, label) in Oxygen. Examples of format: **en_US**, **fr_FR**, **de_DE**, **jp_JP**, **it_IT**, **nl_NL**
  Returns: The language used to display the GUI controls (buttons, label) in Oxygen. Since: 12.1
### getVersion

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getVersion()

Get the current version of the Oxygen/Author product. Can be used to decide if some extension functions are available or not.
  Returns: The version of the Oxygen application in which the extension runs. Returns a string like: 11.2 Since: 12
### getVersionBuildID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getVersionBuildID()

Get the build ID of the current application. It is a string with a format like "YYYYMMDDHH". Example: "2013110816". This is the same information present in the Help menu -> About dialog.
  Returns: the build ID of the current application. Since: 16
### getApplicationType

[ApplicationType](ApplicationType.md) getApplicationType()

Get the type of the application.
  Returns: the type of the application, one of the constants in the [ApplicationType](ApplicationType.md) enumeration. Since: 19
### getApplicationName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getApplicationName()

Get the display name of the application.
  Returns: the display name of the application, one of the constants in the ro.sync.ui.application.ApplicationMainFrameDescriptor interface. Since: 19
### getPlatform

[Platform](../Platform.md) getPlatform()

Return the oXygen platform that is currently running.
  Returns: [Platform.STANDALONE](../Platform.md#STANDALONE) if the code is running in the oXygen stand alone application, [Platform.ECLIPSE](../Platform.md#ECLIPSE) if the code is running in the oXygen Eclipse plugin, and [Platform.WEBAPP](../Platform.md#WEBAPP) if the code is running inside the oXygen WebApp. Since: 17
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
