Package [ro.sync.ecss.imagemap](package-summary.md)

# Class ImageMapUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.imagemap.ImageMapUtil
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class ImageMapUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Image Map Utilities.

## Constructor Summary
 Constructors
Constructor

Description
 [ImageMapUtil](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static int [convertLUToPixels](#convertLUToPixels(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String,int,int))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lu, int refWidth, int fontOfTheNodeSize)
Convert lexical units sizes to pixels.
  static int [getFontOfNodeSize](#getFontOfNodeSize(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [AuthorNode](../extensions/api/node/AuthorNode.md) authorNode)
Get the size of the node's font.
  static void [setLexicalUnitEvaluatorForTests](#setLexicalUnitEvaluatorForTests(ro.sync.ecss.css.LexicalUnitEvaluator))(ro.sync.ecss.css.LexicalUnitEvaluator lexicalUnitEvaluatorForTests)
Not API ! Used only for tests !

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ImageMapUtil

public ImageMapUtil()

## Method Details

### setLexicalUnitEvaluatorForTests

public static void setLexicalUnitEvaluatorForTests(ro.sync.ecss.css.LexicalUnitEvaluator lexicalUnitEvaluatorForTests)

Not API ! Used only for tests !
  Parameters: lexicalUnitEvaluatorForTests - A lexical unit evaluator to be used for computing imposed sizes or scales.
### convertLUToPixels

public static int convertLUToPixels([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) lu, int refWidth, int fontOfTheNodeSize)

Convert lexical units sizes to pixels.
  Parameters: authorAccess - The author access. lu - The lexical unit. refWidth - The reference width (the original width of the item). fontOfTheNodeSize - The size of the containing font. Returns: The computed imposed size.
### getFontOfNodeSize

public static int getFontOfNodeSize([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [AuthorNode](../extensions/api/node/AuthorNode.md) authorNode)

Get the size of the node's font.
  Parameters: authorAccess - The author access. authorNode - The author node. Returns: The size of the node's font.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
