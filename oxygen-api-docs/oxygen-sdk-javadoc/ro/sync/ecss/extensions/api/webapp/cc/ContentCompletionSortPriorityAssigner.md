Package [ro.sync.ecss.extensions.api.webapp.cc](package-summary.md)

# Interface ContentCompletionSortPriorityAssigner
    @API(type=EXTENDABLE, src=PUBLIC) public interface ContentCompletionSortPriorityAssigner
Extension that can be used to assign sorting priorities for elements. The elements in the content completion menu will be sorted according to this priority and in case of equality the display name is used. By default, all entries have priority 0 except for "Split" / "New" - type entries which have priority [CCItemProxy.SPLIT_ITEM_PRIORITY](CCItemProxy.md#SPLIT_ITEM_PRIORITY). The instance can be returned from a [WebappExtensionsProvider](../../WebappExtensionsProvider.md) implementation, by implementing the [WebappExtensionsProvider.getSortPriorityAssigner()](../../WebappExtensionsProvider.md#getSortPriorityAssigner()) method. The [WebappExtensionsProvider](../../WebappExtensionsProvider.md) instance can be returned from an [ExtensionsBundle](../../ExtensionsBundle.md) implementation, by implementing the [ExtensionsBundle.getWebappExtensionsProvier()](../../ExtensionsBundle.md#getWebappExtensionsProvier()) method.
  Since: 21.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [getImposedSortPriority](#getImposedSortPriority(ro.sync.contentcompletion.xml.WhatElementsCanGoHereContext,ro.sync.ecss.extensions.api.webapp.cc.CCItemProxy))([WhatElementsCanGoHereContext](../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context, [CCItemProxy](CCItemProxy.md) ccItem)
Return the imposed sort priority for the given content completion item.

## Method Details

### getImposedSortPriority

int getImposedSortPriority([WhatElementsCanGoHereContext](../../../../../contentcompletion/xml/WhatElementsCanGoHereContext.md) context, [CCItemProxy](CCItemProxy.md) ccItem)

Return the imposed sort priority for the given content completion item.
  Parameters: context - Context in which the content completion is invoked. ccItem - A proxy to the content completion item. Returns: A number, specifying the sorting priority. Larger number means higher in the list.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
