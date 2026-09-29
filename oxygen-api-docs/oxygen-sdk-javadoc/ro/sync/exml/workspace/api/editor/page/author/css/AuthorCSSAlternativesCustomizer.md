Package [ro.sync.exml.workspace.api.editor.page.author.css](package-summary.md)

# Class AuthorCSSAlternativesCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.author.css.AuthorCSSAlternativesCustomizer
   @API(type=EXTENDABLE, src=PUBLIC) public abstract class AuthorCSSAlternativesCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Provides the list of CSS alternatives which can be selected in the Styles drop-down by the end user.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorCSSAlternativesCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [cssGroupsAboutToBeChanged](#cssGroupsAboutToBeChanged(ro.sync.exml.workspace.api.editor.page.author.WSAuthorEditorPage,java.util.List,java.util.List))([WSAuthorEditorPage](../WSAuthorEditorPage.md) authorPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> proposedCSSGroupsToApply, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> allAvailableCSSGroups)
Callback when the styles are changed by the user using the GUI in the CSS-driven visual editing mode.
  void [customizeAvailableCSSGroups](#customizeAvailableCSSGroups(ro.sync.exml.workspace.api.editor.page.author.WSAuthorEditorPage,java.util.List))([WSAuthorEditorPage](../WSAuthorEditorPage.md) authorPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> availableCSSGroups)
Get the list of CSS groups from which the user can choose when editing an XML document.
  void [customizeCSSGroupsToApply](#customizeCSSGroupsToApply(ro.sync.exml.workspace.api.editor.page.author.WSAuthorEditorPage,java.util.List,java.util.List))([WSAuthorEditorPage](../WSAuthorEditorPage.md) authorPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> proposedCSSGroupsToApply, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> allAvailableCSSGroups)
Get the list of CSS Groups to apply when the document is opened in order to render the XML in the CSS-driven visual editing mode.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorCSSAlternativesCustomizer

public AuthorCSSAlternativesCustomizer()

## Method Details

### customizeAvailableCSSGroups

public void customizeAvailableCSSGroups([WSAuthorEditorPage](../WSAuthorEditorPage.md) authorPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> availableCSSGroups)

Get the list of CSS groups from which the user can choose when editing an XML document. The groups are presented by the application in the Styles drop-down chooser. Each CSS group has a title and a set of CSS documents which can be applied.
  Parameters: authorPage - The page for which we request the CSS groups. This can be null if the method is called outside an Editor context. (case: transforming to PDF (with Price CSS) of a topic or map directly from the project, without opening it.) availableCSSGroups - The groups which would be presented by the application in the Styles drop-down chooser if not changed by this customizer. Each group is presented as a separate entry.
### customizeCSSGroupsToApply

public void customizeCSSGroupsToApply([WSAuthorEditorPage](../WSAuthorEditorPage.md) authorPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> proposedCSSGroupsToApply, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> allAvailableCSSGroups)

Get the list of CSS Groups to apply when the document is opened in order to render the XML in the CSS-driven visual editing mode.
  Parameters: authorPage - The page for which we request the CSS groups. proposedCSSGroupsToApply - The CSS groups which will be applied on the loaded XML by the application if the customizer does not perform modifications. allAvailableCSSGroups - The list of all available CSS groups (the groups also available in the Styles drop-down).
### cssGroupsAboutToBeChanged

public void cssGroupsAboutToBeChanged([WSAuthorEditorPage](../WSAuthorEditorPage.md) authorPage, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> proposedCSSGroupsToApply, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSGroup](CSSGroup.md)> allAvailableCSSGroups)

Callback when the styles are changed by the user using the GUI in the CSS-driven visual editing mode.
  Parameters: authorPage - The page for which we request the CSS groups. proposedCSSGroupsToApply - The CSS groups which will be applied on the XML by the application if the customizer does not perform modifications. allAvailableCSSGroups - The list of all available CSS groups (the groups also available in the Styles drop-down).
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
