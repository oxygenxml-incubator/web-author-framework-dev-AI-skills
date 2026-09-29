Package [ro.sync.exml.workspace.api.editor.page](package-summary.md)

# Interface Anchor
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface Anchor
This is a marker interface for an anchor which can be created either in the Text or Author editing modes and then used to located the same content in another editing mode (Author or Text). An Anchor is usually implemented as a simple XPath expression along with a relative offset to remember the current position inside the current XML element's text content.You can serialize an Anchor to a string and back using the "ro.sync.exml.workspace.api.options.GlobalOptionsStorage.serializePersistentObject(Object)" and "ro.sync.exml.workspace.api.options.GlobalOptionsStorage.deserializePersistentObject(Object)" APIs.
  Since: 21
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
