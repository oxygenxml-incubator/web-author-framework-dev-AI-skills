# Package ro.sync.ecss.extensions.api.webapp.cc

package ro.sync.ecss.extensions.api.webapp.cc
    Related Packages
Package

Description
 [ro.sync.ecss.extensions.api.webapp](../package-summary.md)

     All Classes and InterfacesInterfacesClassesExceptions
Class

Description
 [CCItemProxy](CCItemProxy.md)
An item proposed by the content completion manager, and which can be selected by the user.
  [ContentCompletionManager](ContentCompletionManager.md)
This class offers support for actions with content completion such as: insert element, surround with tags and rename element.
  [ContentCompletionSortPriorityAssigner](ContentCompletionSortPriorityAssigner.md)
Extension that can be used to assign sorting priorities for elements. The elements in the content completion menu will be sorted according to this priority and in case of equality the display name is used. By default, all entries have priority 0 except for "Split" / "New" - type entries which have priority [CCItemProxy.SPLIT_ITEM_PRIORITY](CCItemProxy.md#SPLIT_ITEM_PRIORITY). The instance can be returned from a [WebappExtensionsProvider](../../WebappExtensionsProvider.md) implementation, by implementing the [WebappExtensionsProvider.getSortPriorityAssigner()](../../WebappExtensionsProvider.md#getSortPriorityAssigner()) method. The [WebappExtensionsProvider](../../WebappExtensionsProvider.md) instance can be returned from an [ExtensionsBundle](../../ExtensionsBundle.md) implementation, by implementing the [ExtensionsBundle.getWebappExtensionsProvier()](../../ExtensionsBundle.md#getWebappExtensionsProvier()) method.
  [ItemNotFoundException](ItemNotFoundException.md)
An exception thrown when the content completion item chosen by the user was not one of the proposed ones in the specified context.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
