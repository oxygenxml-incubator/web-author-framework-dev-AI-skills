Package [ro.sync.exml.editor.quickassist](package-summary.md)

# Class QuickAssistProposalGroup

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.editor.quickassist.QuickAssistProposalGroup
   @API(type=INTERNAL, src=PUBLIC) public class QuickAssistProposalGroup extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
The group for a quick assist proposal.

## Constructor Summary
 Constructors
Constructor

Description
 [QuickAssistProposalGroup](#%3Cinit%3E(java.lang.String,java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) iconPath, boolean isQuickFix)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDisplayString](#getDisplayString())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getIconPath](#getIconPath())()

 int [hashCode](#hashCode())()

 boolean [isQuickFix](#isQuickFix())()
Checks whether it is a quick fix or a refactory group.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### QuickAssistProposalGroup

public QuickAssistProposalGroup([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) displayString, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) iconPath, boolean isQuickFix)

Constructor.
  Parameters: displayString - The display String for the group. iconPath - The path to the icon of this group. isQuickFix - true if it is a quick fix group, false if it is a refactory group.
## Method Details

### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### getDisplayString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDisplayString()
  Returns: The render string for the group.
### getIconPath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getIconPath()
  Returns: Returns the icon path.
### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### isQuickFix

public boolean isQuickFix()

Checks whether it is a quick fix or a refactory group.
  Returns: true if it is a quick fix group, false if it is a refactory group.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
