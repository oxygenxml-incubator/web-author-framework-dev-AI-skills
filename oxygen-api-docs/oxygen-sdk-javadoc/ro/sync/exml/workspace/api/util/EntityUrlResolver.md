Package [ro.sync.exml.workspace.api.util](package-summary.md)

# Interface EntityUrlResolver
    All Superinterfaces: [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface EntityUrlResolverextends [EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html)
Extended interface to be implemented by an EntityResolver to receive a special callback when Oxygen is not interested in the content of the entity but just in its URL. This method can be more efficient than the resolveEntity method in the parent interface.
  Since: 22
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [resolveEntityUrl](#resolveEntityUrl(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) publicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)
Resolve the URL of external entities (including the external DTD subset and external parameter entities).

### Methods inherited from interface org.xml.sax.[EntityResolver](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html)
 [resolveEntity](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/EntityResolver.html#resolveEntity(java.lang.String,java.lang.String))
## Method Details

### resolveEntityUrl

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) resolveEntityUrl([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) publicId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)

Resolve the URL of external entities (including the external DTD subset and external parameter entities).
  Parameters: publicId - The public identifier of the external entity being referenced, or null if none was supplied. systemId - The system identifier of the external entity being referenced. Returns: The URL of the external entity to be used. null means that the entity could not be resolved. See: EntityResolver#resolveEntity(String, String)
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
