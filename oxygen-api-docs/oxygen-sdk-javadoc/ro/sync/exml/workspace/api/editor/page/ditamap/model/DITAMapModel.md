Package [ro.sync.exml.workspace.api.editor.page.ditamap.model](package-summary.md)

# Interface DITAMapModel
    @API(type=NOT_EXTENDABLE, src=PRIVATE) public interface DITAMapModel
The DITA Map Model.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [AuthorDocumentController](../../../../../../../ecss/extensions/api/AuthorDocumentController.md) [getController](#getController())()

 [ContextKeyManager](../../../../../../../ecss/dita/ContextKeyManager.md) [getKeysManager](#getKeysManager())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getProfilingStylesForNode](#getProfilingStylesForNode(ro.sync.ecss.extensions.api.node.AuthorElement))([AuthorElement](../../../../../../../ecss/extensions/api/node/AuthorElement.md) node)

 [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getUrl](#getUrl())()

## Method Details

### getController

[AuthorDocumentController](../../../../../../../ecss/extensions/api/AuthorDocumentController.md) getController()
  Returns: The document controller for the current DITA map.
### getKeysManager

[ContextKeyManager](../../../../../../../ecss/dita/ContextKeyManager.md) getKeysManager()
  Returns: The keys manager that resolves keys based on the current DITA map.
### getUrl

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getUrl()
  Returns: The URL of the DITA Map.
### getProfilingStylesForNode

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getProfilingStylesForNode([AuthorElement](../../../../../../../ecss/extensions/api/node/AuthorElement.md) node)
  Parameters: node - A node element. Returns: The styles from profiling conditions that should be applied to the given node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
