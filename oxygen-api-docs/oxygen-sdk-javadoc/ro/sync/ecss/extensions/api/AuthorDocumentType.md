Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class AuthorDocumentType

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.AuthorDocumentType
   All Implemented Interfaces: [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorDocumentType extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [Cloneable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Cloneable.html)
Author structure representing DOCTYPE information as present in the Author document.

## Constructor Summary
 Constructors
Constructor

Description
 [AuthorDocumentType](#%3Cinit%3E(java.lang.String,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) publicID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypeContent)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorDocumentType](AuthorDocumentType.md) [clone](#clone())()
Clones this doctype.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContent](#getContent())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getName](#getName())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPublicId](#getPublicId())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSystemId](#getSystemId())()

 int [hashCode](#hashCode())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [serializeDoctype](#serializeDoctype())()
Serialize the doctype
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorDocumentType

public AuthorDocumentType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) publicID, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) doctypeContent)

Constructor.
  Parameters: name - The DOCTYPE name. systemID - The systemID. publicID - Public id. doctypeContent - The DOCTYPE content Example for creating a Docbook AuthorDocumentType:
```

 AuthorDocumentType doctype = new AuthorDocumentType(
     "article", 
     "http://www.docbook.org/xml/4.4/docbookx.dtd", 
     "-//OASIS//DTD DocBook XML V4.4//EN",
     "<!DOCTYPE article PUBLIC \"-//OASIS//DTD DocBook XML V4.4//EN\"\n" + 
     "             \"http://www.docbook.org/xml/4.4/docbookx.dtd\"[\n" + 
     " <!ENTITY ent 'this is an entity'>\n" + 
     "]>");

```

## Method Details

### getName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getName()
  Returns: The name of DTD; i.e., the name immediately following the DOCTYPE keyword.
### getPublicId

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPublicId()
  Returns: The public identifier of the external subset.
### getSystemId

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSystemId()
  Returns: The system identifier of the external subset. This may be an absolute URI or not.
### getContent

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContent()
  Returns: The whole content of the DOCTYPE for serialization Example:
```

 <!DOCTYPE article PUBLIC "-//OASIS//DTD DocBook XML V4.4//EN"
                      "http://www.docbook.org/xml/4.4/docbookx.dtd"[
   <!ENTITY ent 'this is an entity'>
 ]>

```

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

### serializeDoctype

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) serializeDoctype()

Serialize the doctype
  Returns: The serialized doctype
### clone

public [AuthorDocumentType](AuthorDocumentType.md) clone()

Clones this doctype.
  Overrides: [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.clone()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone())

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
