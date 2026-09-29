Package [ro.sync.ecss.extensions.api.spell](package-summary.md)

# Interface SpellCheckerHelper
    All Known Implementing Classes: [DITASpellCheckerHelper](../../dita/DITASpellCheckerHelper.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface SpellCheckerHelper
Helper utilties for the spell checker.
  Since: 26.1
## Method Summary
  All MethodsInstance MethodsDefault Methods
Modifier and Type

Method

Description
 default boolean [isInlineNodeTransparentForSpellChecking](#isInlineNodeTransparentForSpellChecking(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../node/AuthorNode.md) node)
Check if this inline element is transparent for spell checking.

## Method Details

### isInlineNodeTransparentForSpellChecking

default boolean isInlineNodeTransparentForSpellChecking([AuthorNode](../node/AuthorNode.md) node)

Check if this inline element is transparent for spell checking.
  Parameters: node - The author node. Returns: true if this inline node is transparent and if there is content like textword2 then the spell check should consider "textword2" a word to be checked.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
