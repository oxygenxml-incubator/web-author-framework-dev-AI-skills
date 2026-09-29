Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface URLStreamHandlerPluginExtensionConstants
    All Known Subinterfaces: [TargetedURLStreamHandlerPluginExtension](TargetedURLStreamHandlerPluginExtension.md), [URLStreamHandlerPluginExtension](URLStreamHandlerPluginExtension.md), [URLStreamHandlerWithLockPluginExtension](URLStreamHandlerWithLockPluginExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface URLStreamHandlerPluginExtensionConstants
Constants used from URLStreamHandler provider plugin extensions.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADVICE_CLOSE](#ADVICE_CLOSE)
"oxygen-action" header value instructing Oxygen to close the editor.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ADVICE_RELOAD](#ADVICE_RELOAD)
"oxygen-action" header value instructing Oxygen to reload editor's content from the provided location.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LOCATION_HEADER](#LOCATION_HEADER)
The location header key.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXYGEN_ACTION_HEADER](#OXYGEN_ACTION_HEADER)
The oxygen-action header key.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXYGEN_READ_ONLY_HEADER](#OXYGEN_READ_ONLY_HEADER)
"oxygen_read_only" header used to check if a connection is read-only.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXYGEN_READ_ONLY_REASON_CODE_HEADER](#OXYGEN_READ_ONLY_REASON_CODE_HEADER)
"oxygen_read_only_reason_code" header used to specify a code for the reason for the document being read-only.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXYGEN_READ_ONLY_REASON_HEADER](#OXYGEN_READ_ONLY_REASON_HEADER)
"oxygen_read_only_reason" header used to specify a reason for the document being read-only.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [OXYGEN_SAVE_TYPE](#OXYGEN_SAVE_TYPE)
A header indicating the type of the save action performed.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SAVE_AS](#SAVE_AS)
Value for the [OXYGEN_SAVE_TYPE](#OXYGEN_SAVE_TYPE) header, indicating that the user performed a Save As action.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SAVE_AUTO](#SAVE_AUTO)
Value for the [OXYGEN_SAVE_TYPE](#OXYGEN_SAVE_TYPE) header, indicating that an automatic save was performed.

## Field Details

### LOCATION_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LOCATION_HEADER

The location header key. When saving the content through an URLConnection you can set the "location" header field to a specific value. Together with the "oxygen-action" header field value, this will instruct Oxygen to refresh the editor content from the specified location or to close the editor, after performing the save operation.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.LOCATION_HEADER)

### OXYGEN_ACTION_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXYGEN_ACTION_HEADER

The oxygen-action header key. Use case: After saving content to certain CMSs, the content may be changed by the CMS or even the location can be relocated. After closing the output stream, Oxygen will check the header keys of the URLConnection for the "location" and "oxygen-action" keys. If the "oxygen-action" key is found and the value is a supported one: "reload" or "close" values, Oxygen will act accordingly.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.OXYGEN_ACTION_HEADER)

### ADVICE_RELOAD

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADVICE_RELOAD

"oxygen-action" header value instructing Oxygen to reload editor's content from the provided location.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.ADVICE_RELOAD)

### ADVICE_CLOSE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ADVICE_CLOSE

"oxygen-action" header value instructing Oxygen to close the editor.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.ADVICE_CLOSE)

### OXYGEN_READ_ONLY_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXYGEN_READ_ONLY_HEADER

"oxygen_read_only" header used to check if a connection is read-only.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.OXYGEN_READ_ONLY_HEADER)

### OXYGEN_READ_ONLY_REASON_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXYGEN_READ_ONLY_REASON_HEADER

"oxygen_read_only_reason" header used to specify a reason for the document being read-only.
  Since: 18.0 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.OXYGEN_READ_ONLY_REASON_HEADER)

### OXYGEN_READ_ONLY_REASON_CODE_HEADER

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXYGEN_READ_ONLY_REASON_CODE_HEADER

"oxygen_read_only_reason_code" header used to specify a code for the reason for the document being read-only.
  Since: 19.1 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.OXYGEN_READ_ONLY_REASON_CODE_HEADER)

### OXYGEN_SAVE_TYPE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) OXYGEN_SAVE_TYPE

A header indicating the type of the save action performed. If absent, a normal save was performed.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.OXYGEN_SAVE_TYPE)

### SAVE_AS

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SAVE_AS

Value for the [OXYGEN_SAVE_TYPE](#OXYGEN_SAVE_TYPE) header, indicating that the user performed a Save As action.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.SAVE_AS)

### SAVE_AUTO

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SAVE_AUTO

Value for the [OXYGEN_SAVE_TYPE](#OXYGEN_SAVE_TYPE) header, indicating that an automatic save was performed.
  Since: 21.1 See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.plugin.urlstreamhandler.URLStreamHandlerPluginExtensionConstants.SAVE_AUTO)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
