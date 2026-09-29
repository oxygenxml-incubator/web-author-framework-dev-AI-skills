Package [ro.sync.exml.workspace.api.editor.page.author.css](package-summary.md)

# Class CSSGroup

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.exml.workspace.api.editor.page.author.css.CSSGroup
   @API(type=EXTENDABLE, src=PUBLIC) public class CSSGroup extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Represents a group of CSS resources that will all be used at once to style the Author interface. For example if the XML also refers to a CSS directly in the content and the document type configuration states that the directly referenced CSS should be merged with the one coming from the document type configuration, the group will contain both of them.
  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [CSSGroup](#%3Cinit%3E(java.lang.String,boolean))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, boolean isMainSource)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [addURL](#addURL(ro.sync.exml.workspace.api.editor.page.author.css.CSSResource))([CSSResource](CSSResource.md) cssRes)
Add a new css resource to the list.
  void [addURLs](#addURLs(ro.sync.exml.workspace.api.editor.page.author.css.CSSResource%5B%5D))([CSSResource](CSSResource.md)[] urlsList)
Add CSSResource(s).
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getTitle](#getTitle())()

 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSResource](CSSResource.md)> [getUrls](#getUrls())()
Get the list of CSS resources to be used.
  int [hashCode](#hashCode())()

 boolean [isMainSource](#isMainSource())()
Check if this is a main CSS styles source.
  void [removeURL](#removeURL(ro.sync.exml.workspace.api.editor.page.author.css.CSSResource))([CSSResource](CSSResource.md) cssRes)
Add remove new css resource to the list.
  void [setPreferred](#setPreferred(boolean))(boolean isMainSource)
Set this list of CSSs as a main list of CSSs.
  void [setTitle](#setTitle(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)
Set the title for this CSSgroup.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### CSSGroup

public CSSGroup([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title, boolean isMainSource)

Constructor.
  Parameters: title - The merged css title. isMainSource - true if this is a main source of CSS styles. The Styles drop down allows users to choose only one main source. false if this is an alternate source of CSS styles. The Styles drop down allows users to apply multiple alternate styles over a main source.
## Method Details

### setTitle

public void setTitle([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)

Set the title for this CSSgroup.
  Parameters: title - The new title. Since: 17.1
### isMainSource

public boolean isMainSource()

Check if this is a main CSS styles source.
  Returns: Returns true if this is a main source of CSS styles. The Styles drop down allows users to choose only one main source. false if this is an alternate source of CSS styles. The Styles drop down allows users to apply multiple alternate styles over a main source.
### getTitle

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getTitle()
  Returns: Returns the title.
### getUrls

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CSSResource](CSSResource.md)> getUrls()

Get the list of CSS resources to be used.
  Returns: Returns the list of CSS resources.
### addURLs

public void addURLs([CSSResource](CSSResource.md)[] urlsList)

Add CSSResource(s).
  Parameters: urlsList - The CSSResource(s) to be added.
### addURL

public void addURL([CSSResource](CSSResource.md) cssRes)

Add a new css resource to the list.
  Parameters: cssRes - The CSS resource to add.
### removeURL

public void removeURL([CSSResource](CSSResource.md) cssRes)

Add remove new css resource to the list.
  Parameters: cssRes - The CSS resource to add.
### setPreferred

public void setPreferred(boolean isMainSource)

Set this list of CSSs as a main list of CSSs.
  Parameters: isMainSource - true if this is a main source of CSS styles. The Styles drop down allows users to choose only one main source. false if this is an alternate source of CSS styles. The Styles drop down allows users to apply multiple alternate styles over a main source.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.toString()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
