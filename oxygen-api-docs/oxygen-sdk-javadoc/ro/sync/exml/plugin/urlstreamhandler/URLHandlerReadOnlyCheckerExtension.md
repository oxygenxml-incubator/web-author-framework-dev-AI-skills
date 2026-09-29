Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface URLHandlerReadOnlyCheckerExtension
    @API(type=EXTENDABLE, src=PUBLIC) public interface URLHandlerReadOnlyCheckerExtension
This interface can be called to decide if an URL is read-only or not.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [canCheckReadOnly](#canCheckReadOnly(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)
Returns true if the implementor should be asked about the read-only status for URL's of a certain protocol.
  boolean [isReadOnly](#isReadOnly(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Decide if a given URL is read-only or writable to.

## Method Details

### isReadOnly

boolean isReadOnly([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Decide if a given URL is read-only or writable to. If an URL is marked as read-only Oxygen will present it with a read-only lock icon on the tab. The user will also be able to specify through the user interface that an opened editor over a read-only URL can be edited. Also when saving in Oxygen and the URL is marked as read-only the Save As dialog will be shown instead. This call back will usually be received often, each time focus is gained by the current editor. WARNING: It is advisable to cache the calls for recognized URLs as this method might be called quite often.
  Parameters: url - The URL for which the implementor will decide if it is read-only or not. Returns: true if a given URL should be regarded by Oxygen as read-only.
### canCheckReadOnly

boolean canCheckReadOnly([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) protocol)

Returns true if the implementor should be asked about the read-only status for URL's of a certain protocol. This call back will usually be received often, each time focus is gained by the current editor.
  Parameters: protocol - The URL protocol (like "http" or "file") Returns: true if the implementor should be asked about the read-only status for URL's of a certain protocol. For example if you want to decide if "http" URLs are read-only or not you should return true if the protocol is "http" Then, the other callback will be called and you will be able to decide the read-only status for the URL.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
