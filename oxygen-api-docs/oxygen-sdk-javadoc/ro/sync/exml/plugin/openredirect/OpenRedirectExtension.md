Package [ro.sync.exml.plugin.openredirect](package-summary.md)

# Interface OpenRedirectExtension
    All Superinterfaces: [PluginExtension](../PluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface OpenRedirectExtensionextends [PluginExtension](../PluginExtension.md)
Plugin extension - open redirecting for URLs

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [OpenRedirectInformation](OpenRedirectInformation.md)[] [redirect](#redirect(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
This call back can redirect an open call for an URL in different parts of Oxygen.

## Method Details

### redirect

[OpenRedirectInformation](OpenRedirectInformation.md)[] redirect([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

This call back can redirect an open call for an URL in different parts of Oxygen. For example if you want to open a certain XML file from a ZIP archive, when the callback is received for the archive URL you can return two OpenRedirectInformation objects (one with the URL of the archive and the content type of the archive browser and the other with the URL of the file inside the archive and the content type "null" for auto-detection or text/xml).
  Parameters: url - The URL which will get opened in Oxygen Returns: null if the plugin lets the default behavior take place. Empty array if the plugin chooses not to open anything An array of redirect information objects which will direct Oxygen to open them with the specified content types.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
