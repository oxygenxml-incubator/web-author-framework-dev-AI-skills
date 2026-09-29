Package [ro.sync.ecss.extensions.api.link](package-summary.md)

# Interface IDTypeVerifier
    @API(type=EXTENDABLE, src=PUBLIC) public interface IDTypeVerifier
Interface used to check if an attribute has the ID type.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [hasIDType](#hasIDType(java.lang.String,java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs)
Check if the provided attribute has the ID type.

## Method Details

### hasIDType

boolean hasIDType([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementNs, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) attrNs)

Check if the provided attribute has the ID type.
  Parameters: elementName - The local name of the attribute parent element. elementNs - The namespace of the attribute parent element. attrName - The local name of the attribute. attrNs - The namespace of the attribute. Returns: true if the given attribute has the ID type.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
