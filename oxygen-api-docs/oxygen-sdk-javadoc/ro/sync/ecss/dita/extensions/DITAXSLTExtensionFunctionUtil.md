Package [ro.sync.ecss.dita.extensions](package-summary.md)

# Class DITAXSLTExtensionFunctionUtil

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.dita.extensions.DITAXSLTExtensionFunctionUtil
   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class DITAXSLTExtensionFunctionUtil extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Utility methods used to access information about keys referenced in DITA topics. The static methods in this class can be accessed from both XSLT and XQuery scripts. They can be used for example from a Schematron schema to check the target of a key reference:
```
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron" queryBinding="xslt2">
    <sch:ns uri="java:ro.sync.ecss.dita.extensions.DITAXSLTExtensionFunctionUtil" prefix="ditaaccess"/>
    <sch:let name="doc" value="document-uri()"/>
    <sch:pattern>
        <sch:rule context="xref[@keyref][not(node())]">
            <sch:report 
                test="ditaaccess:getKeyRefInfo(@keyref, $doc) = 'PEER_MAP_KEY_HREF'">
                Peer key reference to topic: 
                <sch:value-of select="tokenize(ditaaccess:getKeyRefAbsoluteReference(@keyref, $doc), '/')[last()]"/>
            </sch:report>
        </sch:rule>
    </sch:pattern>
</sch:schema>
```

  Since: 25.1
## Constructor Summary
 Constructors
Constructor

Description
 [DITAXSLTExtensionFunctionUtil](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKeyRefAbsoluteReference](#getKeyRefAbsoluteReference(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextSystemID)
Get the URL location referenced by the defined key as a string.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getKeyRefInfo](#getKeyRefInfo(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextSystemID)
Get information about a key reference.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DITAXSLTExtensionFunctionUtil

public DITAXSLTExtensionFunctionUtil()

## Method Details

### getKeyRefInfo

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKeyRefInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextSystemID)

Get information about a key reference.
  Parameters: keyref - The keyref. contextSystemID - The context system ID Returns: a string (never null) with one of the values:
```

 CONTEXT_NOT_AVAILABLE - Usually means there is no DITA Map set in the DITA Maps Manager "Context" combo box or opened in the DITA Maps manager view.
 CONTEXT_AMBIGUOUS - The topic is referenced in multiple key scope contexts and there is not enough information to know from which context the method is called.
 PEER_MAP_KEY_HREF - Reference to a key defined in a peer referenced DITA Map. The key definition has a reference to a resource.
 PEER_MAP_KEY_NO_HREF - Reference to a key defined in a peer referenced DITA Map. The key definition does not have a reference to a resource.
 KEY_HREF - Reference to a key defined in the DITA Map context. The key definition has a reference to a resource.
 KEY_NO_HREF - Reference to a key defined in the DITA Map context. The key definition does not have a reference to a resource.
 KEY_NOT_FOUND - Key definition was not found.

```
 Sample usage from Schematron:
```
<sch:schema xmlns:sch="http://purl.oclc.org/dsdl/schematron" queryBinding="xslt2">
    <sch:ns uri="java:ro.sync.ecss.dita.extensions.DITAXSLTExtensionFunctionUtil" prefix="ditaaccess"/>
    <sch:let name="doc-uri" value="document-uri()"/>
    <sch:pattern>
        <sch:rule context="xref[@keyref][not(node())]">
            <sch:report test="ditaaccess:getKeyRefInfo(@keyref, $doc-uri) = 'PEER_MAP_KEY_HREF'">
                Peer keyref <sch:value-of select="ditaaccess:getKeyRefAbsoluteReference(@keyref, $doc-uri)"/>
            </sch:report>
        </sch:rule>
    </sch:pattern>
</sch:schema>
```
 Decision tree:  Since: 25.1
### getKeyRefAbsoluteReference

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getKeyRefAbsoluteReference([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) keyref, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) contextSystemID)

Get the URL location referenced by the defined key as a string.
  Parameters: keyref - The keyref. contextSystemID - The context system ID Returns: The URL location referenced by the defined key or null if the key does not exist or does not refer a resource. If the key reference contains an element ID like "keyName/elementID", the returned URL will have the format similar to "file:/path/to/target.xml#FIRST_TOPIC_ID/elementId" as the gathered keys do not contain information about the ID of the target topic. Since: 25.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
