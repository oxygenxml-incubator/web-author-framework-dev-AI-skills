Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface URLStreamHandlerWithLockPluginExtension
    All Superinterfaces: [LockHandlerFactoryPluginExtension](LockHandlerFactoryPluginExtension.md), [PluginExtension](../PluginExtension.md), [URLStreamHandlerPluginExtension](URLStreamHandlerPluginExtension.md), [URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface URLStreamHandlerWithLockPluginExtensionextends [URLStreamHandlerPluginExtension](URLStreamHandlerPluginExtension.md), [LockHandlerFactoryPluginExtension](LockHandlerFactoryPluginExtension.md)
An URLStreamHandler with lock support plugin extension.

## Field Summary

### Fields inherited from interface ro.sync.exml.plugin.urlstreamhandler.[URLStreamHandlerPluginExtensionConstants](URLStreamHandlerPluginExtensionConstants.md)
 [ADVICE_CLOSE](URLStreamHandlerPluginExtensionConstants.md#ADVICE_CLOSE), [ADVICE_RELOAD](URLStreamHandlerPluginExtensionConstants.md#ADVICE_RELOAD), [LOCATION_HEADER](URLStreamHandlerPluginExtensionConstants.md#LOCATION_HEADER), [OXYGEN_ACTION_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_ACTION_HEADER), [OXYGEN_READ_ONLY_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_HEADER), [OXYGEN_READ_ONLY_REASON_CODE_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_REASON_CODE_HEADER), [OXYGEN_READ_ONLY_REASON_HEADER](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_READ_ONLY_REASON_HEADER), [OXYGEN_SAVE_TYPE](URLStreamHandlerPluginExtensionConstants.md#OXYGEN_SAVE_TYPE), [SAVE_AS](URLStreamHandlerPluginExtensionConstants.md#SAVE_AS), [SAVE_AUTO](URLStreamHandlerPluginExtensionConstants.md#SAVE_AUTO)
## Method Summary

### Methods inherited from interface ro.sync.exml.plugin.urlstreamhandler.[LockHandlerFactoryPluginExtension](LockHandlerFactoryPluginExtension.md)
 [getLockHandler](LockHandlerFactoryPluginExtension.md#getLockHandler()), [isLockingSupported](LockHandlerFactoryPluginExtension.md#isLockingSupported(java.lang.String))
### Methods inherited from interface ro.sync.exml.plugin.urlstreamhandler.[URLStreamHandlerPluginExtension](URLStreamHandlerPluginExtension.md)
 [getURLStreamHandler](URLStreamHandlerPluginExtension.md#getURLStreamHandler(java.lang.String))
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
