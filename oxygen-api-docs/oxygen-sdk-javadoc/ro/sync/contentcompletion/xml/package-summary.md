# Package ro.sync.contentcompletion.xml

package ro.sync.contentcompletion.xml

Objects used to offer information about what elements or attributes are allowed at a certain offset in the XML.
     All Classes and InterfacesInterfacesClassesEnum Classes
Class

Description
 [CIAttribute](CIAttribute.md)
Interface for objects holding information about attributes used in the content completion process.
  [CIAttribute.DefaultValueProvider](CIAttribute.DefaultValueProvider.md)
Default value provider for an attribute.
  [CIAttribute.EditableState](CIAttribute.EditableState.md)
The editable state of the attribute.
  [CIElement](CIElement.md)
Interface for objects holding information about element proposals used in the content completion process.
  [CIElementAdapter](CIElementAdapter.md)
A CIElement adapter.
  [CIValue](CIValue.md)
Interface for objects holding information about element or attribute values used in the content completion process.
  [Context](Context.md)
The context for a node contains: elementStack - the stack with [ContextElement](ContextElement.md) up to the root.
  [ContextElement](ContextElement.md)
Store information about an element inside a context, involved in the content completion process.
  [ExternalEntityNameValue](ExternalEntityNameValue.md)
A pair class with name and value.
  [NameValue](NameValue.md)
A pair class with name and value.
  [NodeDescription](NodeDescription.md)
Node description is in fact a collection of properties for a node.
  [SchemaManagerFilter](SchemaManagerFilter.md)
Interface for objects used to filter the editor content completion schema manager proposals.
  [SchemaManagerFilterBase](SchemaManagerFilterBase.md)
Base class for objects used to filter the editor content completion schema manager proposals.
  [StyleGuideSchemaManagerFilterBase](StyleGuideSchemaManagerFilterBase.md)
Style guide schema manager filter base.
  [WhatAttributesCanGoHereContext](WhatAttributesCanGoHereContext.md)
Used by the schema manager to find out the attributes that can be inserted in a given context.
  [WhatElementsCanGoHereContext](WhatElementsCanGoHereContext.md)
It is used to determine the elements that can be inserted in the current context.
  [WhatPossibleValuesHasAttributeContext](WhatPossibleValuesHasAttributeContext.md)
It is used to determine the possible values of the current attribute.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
