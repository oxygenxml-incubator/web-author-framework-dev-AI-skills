Package [ro.sync.ecss.component](package-summary.md)

# Interface RenderingInfoChangedListener
    All Superinterfaces: [BatchEditListener](BatchEditListener.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface RenderingInfoChangedListenerextends [BatchEditListener](BatchEditListener.md)
Listener that is notified when the rendering info for a node is changed. The rendering info includes the style of the node, as computed from the associated CSS or its content. When the info is changed for a node it means that all its descendants need to be rendered again.
  Since: 15.2
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [renderingInfoChanged](#renderingInfoChanged(ro.sync.ecss.extensions.api.node.AuthorParentNode,ro.sync.ecss.component.RenderingInfoChangeType))([AuthorParentNode](../extensions/api/node/AuthorParentNode.md) element, [RenderingInfoChangeType](RenderingInfoChangeType.md) type)
Method to be called when the rendering info is changed for a node.

### Methods inherited from interface ro.sync.ecss.component.[BatchEditListener](BatchEditListener.md)
 [beginEdit](BatchEditListener.md#beginEdit()), [endEdit](BatchEditListener.md#endEdit())
## Method Details

### renderingInfoChanged

void renderingInfoChanged([AuthorParentNode](../extensions/api/node/AuthorParentNode.md) element, [RenderingInfoChangeType](RenderingInfoChangeType.md) type)

Method to be called when the rendering info is changed for a node.
  Parameters: element - The element whose information was changed. type - The type of the change.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
