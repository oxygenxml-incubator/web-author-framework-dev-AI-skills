Package [ro.sync.ecss.extensions.dita](package-summary.md)

# Class DITASpellCheckerHelper

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.dita.DITASpellCheckerHelper
   All Implemented Interfaces: [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md)   @API(type=INTERNAL, src=PUBLIC) public class DITASpellCheckerHelper extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md)
Helps identify inline elements which should be transparent to the spell checker

## Constructor Summary
 Constructors
Constructor

Description
 [DITASpellCheckerHelper](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [isInlineNodeTransparentForSpellChecking](#isInlineNodeTransparentForSpellChecking(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](../api/node/AuthorNode.md) node)
Check if this inline element is transparent for spell checking.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITASpellCheckerHelper

public DITASpellCheckerHelper()

## Method Details

### isInlineNodeTransparentForSpellChecking

public boolean isInlineNodeTransparentForSpellChecking([AuthorNode](../api/node/AuthorNode.md) node)
 Description copied from interface: [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md#isInlineNodeTransparentForSpellChecking(ro.sync.ecss.extensions.api.node.AuthorNode))
Check if this inline element is transparent for spell checking.
  Specified by: [isInlineNodeTransparentForSpellChecking](../api/spell/SpellCheckerHelper.md#isInlineNodeTransparentForSpellChecking(ro.sync.ecss.extensions.api.node.AuthorNode)) in interface [SpellCheckerHelper](../api/spell/SpellCheckerHelper.md) Parameters: node - The author node. Returns: true if this inline node is transparent and if there is content like textword2 then the spell check should consider "textword2" a word to be checked. See Also:
        * [SpellCheckerHelper.isInlineNodeTransparentForSpellChecking(ro.sync.ecss.extensions.api.node.AuthorNode)](../api/spell/SpellCheckerHelper.md#isInlineNodeTransparentForSpellChecking(ro.sync.ecss.extensions.api.node.AuthorNode))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
