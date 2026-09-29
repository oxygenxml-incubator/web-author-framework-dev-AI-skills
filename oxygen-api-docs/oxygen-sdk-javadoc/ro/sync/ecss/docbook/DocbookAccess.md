Package [ro.sync.ecss.docbook](package-summary.md)

# Class DocbookAccess

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.docbook.DocbookAccess
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public final class DocbookAccess extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Docbook access.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DOCBOOK_NS](#DOCBOOK_NS)
Docbook namespace.

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> [annotateAttributes](#annotateAttributes(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> attributes)
Annotate a list of attributes.
  static ro.sync.ecss.docbook.DocBookImageInfo [chooseImageReference](#chooseImageReference(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Allows the user to choose an image reference, which will be inserted inside the document.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [chooseLocalLink](#chooseLocalLink(ro.sync.ecss.extensions.api.AuthorAccess,boolean,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean isXref, boolean isDocbook5)
Show a dialog to choose an id.
  static [OLinkInfo](olink/OLinkInfo.md) [chooseOLink](#chooseOLink(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Choose OLink.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [chooseURLForLink](#chooseURLForLink(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)
Choose url for link.
  static void [editOLink](#editOLink(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Edit OLink.
  static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> [filterAttributeValues](#filterAttributeValues(java.util.List,ro.sync.contentcompletion.xml.WhatPossibleValuesHasAttributeContext,java.lang.String))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName)
Propose additional attribute values
  static void [insertLocalLink](#insertLocalLink(ro.sync.ecss.extensions.api.AuthorAccess,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean schemaAware)
Create and insert a local link element.
  static void [insertOLink](#insertOLink(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)
Insert OLink.
  static void [insertXInclude](#insertXInclude(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Insert an XInclude fragment.
  static void [insertXRef](#insertXRef(ro.sync.ecss.extensions.api.AuthorAccess,boolean))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean schemaAware)
Insert a xref element.
  static void [pasteContentAsLink](#pasteContentAsLink(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Paste clipboard content as <link> with @linkend attribute.
  static void [pasteContentAsXref](#pasteContentAsXref(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Paste clipboard content as <xref> with @linkend attribute.
  static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [resolveCustomHrefToMasterFile](#resolveCustomHrefToMasterFile(java.net.URL,java.lang.String,ro.sync.ecss.extensions.api.AuthorAccess))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)
Resolve an IDREF to a main file if possible.
  static void [setDocbookAccessCustomizer](#setDocbookAccessCustomizer(ro.sync.ecss.docbook.DocbookAccessCustomizer))(ro.sync.ecss.docbook.DocbookAccessCustomizer accessCustomizer)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### DOCBOOK_NS

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DOCBOOK_NS

Docbook namespace.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.ecss.docbook.DocbookAccess.DOCBOOK_NS)

## Method Details

### setDocbookAccessCustomizer

public static void setDocbookAccessCustomizer(ro.sync.ecss.docbook.DocbookAccessCustomizer accessCustomizer)
  Parameters: accessCustomizer - The accessCustomizer to set.
### chooseOLink

public static [OLinkInfo](olink/OLinkInfo.md) chooseOLink([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Choose OLink. Public, maybe users want to customize what tag name to insert.
  Parameters: authorAccess - The Author access. Returns: The OLink information, or null if the user canceled the operation.
### insertOLink

public static void insertOLink([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert OLink.
  Parameters: authorAccess - Author access namespace - Namespace Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### editOLink

public static void editOLink([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) namespace)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md), [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)

Edit OLink.
  Parameters: authorAccess - Author access namespace - Namespace Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) [BadLocationException](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/BadLocationException.html)
### filterAttributeValues

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> filterAttributeValues([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIValue](../../contentcompletion/xml/CIValue.md)> attributeValues, [WhatPossibleValuesHasAttributeContext](../../contentcompletion/xml/WhatPossibleValuesHasAttributeContext.md) context, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) documentTypeName)

Propose additional attribute values
  Parameters: attributeValues - The attribute values context - The context documentTypeName -  Returns: The enriched list
### annotateAttributes

public static [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> annotateAttributes([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[CIAttribute](../../contentcompletion/xml/CIAttribute.md)> attributes)

Annotate a list of attributes.
  Parameters: attributes - The attributes list. Returns: The list of attributes with annotations.
### insertXInclude

public static void insertXInclude([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert an XInclude fragment.
  Parameters: authorAccess - The author access. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### insertLocalLink

public static void insertLocalLink([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean schemaAware)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Create and insert a local link element.
  Parameters: authorAccess - The Author access. schemaAware - true to insert with schema aware, false otherwise. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### chooseLocalLink

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) chooseLocalLink([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean isXref, boolean isDocbook5)

Show a dialog to choose an id.
  Parameters: authorAccess - The author access. isXref - If true it will be inserted an xref element. isDocbook5 - If true the current file is Docbook 5. Returns: The chosen id or null if the user canceled the dialog. Since: 18
### chooseURLForLink

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) chooseURLForLink([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) title)

Choose url for link.
  Parameters: authorAccess - The author access. title - The dialog title. Returns: The chosen url. Since: 18
### insertXRef

public static void insertXRef([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess, boolean schemaAware)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Insert a xref element.
  Parameters: authorAccess - The Author access. schemaAware - true to insert with schema aware, false otherwise. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md)
### resolveCustomHrefToMasterFile

public static [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resolveCustomHrefToMasterFile([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) currentEditorURL, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) linkHref, [AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Resolve an IDREF to a main file if possible.
  Parameters: currentEditorURL - The current editor URL linkHref - The link href authorAccess - The author access Returns: The resolved URL if any.
### pasteContentAsLink

public static void pasteContentAsLink([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Paste clipboard content as <link> with @linkend attribute.
  Parameters: authorAccess - The author access.
### pasteContentAsXref

public static void pasteContentAsXref([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)

Paste clipboard content as <xref> with @linkend attribute.
  Parameters: authorAccess - The author access.
### chooseImageReference

public static ro.sync.ecss.docbook.DocBookImageInfo chooseImageReference([AuthorAccess](../extensions/api/AuthorAccess.md) authorAccess)throws [AuthorOperationException](../extensions/api/AuthorOperationException.md)

Allows the user to choose an image reference, which will be inserted inside the document.
  Parameters: authorAccess - Access to the Author-specific functions. Returns: An object containing all the properties for the image that will be inserted. Throws: [AuthorOperationException](../extensions/api/AuthorOperationException.md) - When the operation cannot be performed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
