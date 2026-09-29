Package [ro.sync.ecss.extensions.docbook](package-summary.md)

# Class PromoteDemoteSectionUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.docbook.PromoteDemoteSectionUtil
   @API(type=INTERNAL, src=PUBLIC) public class PromoteDemoteSectionUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility class for promote/demote actions for Docbook.

## Nested Class Summary
 Nested Classes
Modifier and Type

Class

Description
 static enum  [PromoteDemoteSectionUtil.PromoteDemote](PromoteDemoteSectionUtil.PromoteDemote.md)
Promote/demote section action.

## Constructor Summary
 Constructors
Constructor

Description
 [PromoteDemoteSectionUtil](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static boolean [nodeContainsSect5Element](#nodeContainsSect5Element(ro.sync.ecss.extensions.api.AuthorElementBaseInterface))([AuthorElementBaseInterface](../api/AuthorElementBaseInterface.md) sectionElement)
Returns true if the sect node contains a "sect5" element.
  static void [processPromoteDemote](#processPromoteDemote(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.docbook.PromoteDemoteSectionUtil.PromoteDemote))([AuthorAccess](../api/AuthorAccess.md) authorAccess, [PromoteDemoteSectionUtil.PromoteDemote](PromoteDemoteSectionUtil.PromoteDemote.md) action)
Executes the promote/demote section action.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### PromoteDemoteSectionUtil

public PromoteDemoteSectionUtil()

## Method Details

### processPromoteDemote

public static void processPromoteDemote([AuthorAccess](../api/AuthorAccess.md) authorAccess, [PromoteDemoteSectionUtil.PromoteDemote](PromoteDemoteSectionUtil.PromoteDemote.md) action)

Executes the promote/demote section action.
  Parameters: authorAccess - The author access. action - The promote/demote action.
### nodeContainsSect5Element

public static boolean nodeContainsSect5Element([AuthorElementBaseInterface](../api/AuthorElementBaseInterface.md) sectionElement)

Returns true if the sect node contains a "sect5" element.
  Parameters: sectionElement - The sect node. Returns: true if the sect node contains a "sect5" element.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
