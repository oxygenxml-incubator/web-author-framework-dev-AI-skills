Package [ro.sync.exml.workspace.api.references](package-summary.md)

# Interface ReferenceExtractor
    All Known Implementing Classes: [ImageMapExtractor](../../../../ecss/extensions/api/webapp/references/ImageMapExtractor.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ReferenceExtractor
Interface used to extract a Reference from a node
  Since: 21.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Reference](Reference.md)> [extract](#extract(ro.sync.ecss.dom.AuthorSentinelNode))(ro.sync.ecss.dom.AuthorSentinelNode node)
Returns a Reference for the external resource

## Method Details

### extract

[Optional](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)<[Reference](Reference.md)> extract(ro.sync.ecss.dom.AuthorSentinelNode node)

Returns a Reference for the external resource
  Parameters: node - the document node Returns: reference data of the external resource associated with the node
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
