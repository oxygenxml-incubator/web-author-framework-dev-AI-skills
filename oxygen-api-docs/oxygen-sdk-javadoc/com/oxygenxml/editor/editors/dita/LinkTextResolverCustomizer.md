Package [com.oxygenxml.editor.editors.dita](package-summary.md)

# Class LinkTextResolverCustomizer

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * com.oxygenxml.editor.editors.dita.LinkTextResolverCustomizer
   @API(type=EXTENDABLE, src=PUBLIC) public class LinkTextResolverCustomizer extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Abstract class allowed as an extension point to customize the resolution of the text which appears on DITA xrefs. In your plugin in the plugin.xml you should reference it like:
```

  <extension point="oxygen.plugin.id.ditaLinkTextResolverCustomizer">
     <implementation class="my.package.CustomLinkTextResolverCustomizer"/>;
    </extension>

```

  Since: 17
## Constructor Summary
 Constructors
Constructor

Description
 [LinkTextResolverCustomizer](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [computeLinkText](#computeLinkText(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)
Compute the link text to appear on a certain DITA xref or link based on the href and base system ID values.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### LinkTextResolverCustomizer

public LinkTextResolverCustomizer()

## Method Details

### computeLinkText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) computeLinkText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) hrefValue, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) baseSystemID)throws [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)

Compute the link text to appear on a certain DITA xref or link based on the href and base system ID values.
  Parameters: hrefValue - The value of the reference. baseSystemID - The base system ID Returns: The computed link text or null to continue the default processing. Throws: [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html)
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
