Package [ro.sync.ecss.dita](package-summary.md)

# Interface DITAKeyNameGenerator
    @API(type=EXTENDABLE, src=PUBLIC) public interface DITAKeyNameGenerator
Used to generate key names based on file names.
  Since: 23
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [generateKeyName](#generateKeyName(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resourceURL)
Generate a key name based on the given URL.

## Method Details

### generateKeyName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) generateKeyName([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) resourceURL)

Generate a key name based on the given URL.
  Parameters: resourceURL - The URL of a resource. Returns: the generated key name. If null, Oxygen will take care of the key name generation.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
