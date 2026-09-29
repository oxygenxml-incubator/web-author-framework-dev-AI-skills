Package [ro.sync.ecss.component.validation](package-summary.md)

# Class AuthorDocumentPositionedInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * [ro.sync.document.DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md)
        * ro.sync.ecss.component.validation.AuthorDocumentPositionedInfo
   All Implemented Interfaces: [IAuthorDocumentPositionedInfo](IAuthorDocumentPositionedInfo.md)   @API(type=EXTENDABLE, src=PUBLIC) public class AuthorDocumentPositionedInfo extends [DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md)implements [IAuthorDocumentPositionedInfo](IAuthorDocumentPositionedInfo.md)
A document position info usually needs a line and column for the error. This extension allows you to specify either the problem AuthorNode or an offset/length interval in the Author content.

## Field Summary

### Fields inherited from class ro.sync.document.[DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md)
 [NOT_KNOWN](../../../document/DocumentPositionedInfo.md#NOT_KNOWN), [SEVERITY_ERROR](../../../document/DocumentPositionedInfo.md#SEVERITY_ERROR), [SEVERITY_FATAL](../../../document/DocumentPositionedInfo.md#SEVERITY_FATAL), [SEVERITY_INFO](../../../document/DocumentPositionedInfo.md#SEVERITY_INFO), [SEVERITY_WARN](../../../document/DocumentPositionedInfo.md#SEVERITY_WARN)
### Fields inherited from interface ro.sync.ecss.component.validation.[IAuthorDocumentPositionedInfo](IAuthorDocumentPositionedInfo.md)
 [CONTENT_DATA](IAuthorDocumentPositionedInfo.md#CONTENT_DATA)
## Constructor Summary
 Constructors
Constructor

Description
 [AuthorDocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String,java.lang.String,int,int))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int startOffset, int length)
Constructor.
  [AuthorDocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../extensions/api/node/AuthorNode.md) node)
Constructor.
  [AuthorDocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String,ro.sync.ecss.extensions.api.node.AuthorNode))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [AuthorNode](../../extensions/api/node/AuthorNode.md) node)
Constructor.
  [AuthorDocumentPositionedInfo](#%3Cinit%3E(ro.sync.document.DocumentPositionedInfo,ro.sync.ecss.extensions.api.node.AuthorNode))([DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md) dpi, [AuthorNode](../../extensions/api/node/AuthorNode.md) node)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorNode](../../extensions/api/node/AuthorNode.md) [getNode](#getNode())()

 boolean [isSelectEntireNode](#isSelectEntireNode())()
Checks if the entire node should be selected.
  void [setSelectEntireNode](#setSelectEntireNode(boolean))(boolean selectEntireNode)
Sets if the entire node should be selected or not.

### Methods inherited from class ro.sync.document.[DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md)
 [asHTML](../../../document/DocumentPositionedInfo.md#asHTML()), [asHTML](../../../document/DocumentPositionedInfo.md#asHTML(boolean,boolean,boolean,boolean,boolean,boolean)), [asHTML](../../../document/DocumentPositionedInfo.md#asHTML(boolean,boolean,boolean,boolean,boolean,boolean,boolean)), [asHTML](../../../document/DocumentPositionedInfo.md#asHTML(boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean)), [asJSON](../../../document/DocumentPositionedInfo.md#asJSON()), [asJSON](../../../document/DocumentPositionedInfo.md#asJSON(boolean,boolean,boolean,boolean,boolean,boolean)), [asJSON](../../../document/DocumentPositionedInfo.md#asJSON(boolean,boolean,boolean,boolean,boolean,boolean,boolean)), [asText](../../../document/DocumentPositionedInfo.md#asText()), [asText](../../../document/DocumentPositionedInfo.md#asText(boolean,boolean,boolean,boolean,boolean,boolean)), [asText](../../../document/DocumentPositionedInfo.md#asText(boolean,boolean,boolean,boolean,boolean,boolean,boolean)), [asXML](../../../document/DocumentPositionedInfo.md#asXML()), [asXML](../../../document/DocumentPositionedInfo.md#asXML(boolean,boolean,boolean,boolean,boolean,boolean)), [asXML](../../../document/DocumentPositionedInfo.md#asXML(boolean,boolean,boolean,boolean,boolean,boolean,boolean)), [equals](../../../document/DocumentPositionedInfo.md#equals(java.lang.Object)), [flipSeverity](../../../document/DocumentPositionedInfo.md#flipSeverity(int)), [getAdditionalHtmlContent](../../../document/DocumentPositionedInfo.md#getAdditionalHtmlContent()), [getAdditionalInfo](../../../document/DocumentPositionedInfo.md#getAdditionalInfo()), [getAnchor](../../../document/DocumentPositionedInfo.md#getAnchor()), [getColumn](../../../document/DocumentPositionedInfo.md#getColumn()), [getData](../../../document/DocumentPositionedInfo.md#getData()), [getDetailedExceptionInfo](../../../document/DocumentPositionedInfo.md#getDetailedExceptionInfo()), [getDITAAdditionalInfo](../../../document/DocumentPositionedInfo.md#getDITAAdditionalInfo()), [getECAdditionalInfo](../../../document/DocumentPositionedInfo.md#getECAdditionalInfo()), [getEndColumn](../../../document/DocumentPositionedInfo.md#getEndColumn()), [getEndLine](../../../document/DocumentPositionedInfo.md#getEndLine()), [getEngineName](../../../document/DocumentPositionedInfo.md#getEngineName()), [getErrorKey](../../../document/DocumentPositionedInfo.md#getErrorKey()), [getHTMLMessage](../../../document/DocumentPositionedInfo.md#getHTMLMessage()), [getImposedInitialPage](../../../document/DocumentPositionedInfo.md#getImposedInitialPage()), [getLength](../../../document/DocumentPositionedInfo.md#getLength()), [getLine](../../../document/DocumentPositionedInfo.md#getLine()), [getMatchRange](../../../document/DocumentPositionedInfo.md#getMatchRange()), [getMessage](../../../document/DocumentPositionedInfo.md#getMessage()), [getMessageHighlightOffset](../../../document/DocumentPositionedInfo.md#getMessageHighlightOffset()), [getMessageProvider](../../../document/DocumentPositionedInfo.md#getMessageProvider()), [getMessageWithEngine](../../../document/DocumentPositionedInfo.md#getMessageWithEngine()), [getMessageWithEngine](../../../document/DocumentPositionedInfo.md#getMessageWithEngine(boolean,boolean)), [getMessageWithSeverity](../../../document/DocumentPositionedInfo.md#getMessageWithSeverity()), [getMessageWithSeverity](../../../document/DocumentPositionedInfo.md#getMessageWithSeverity(boolean)), [getMessageWithSeverity](../../../document/DocumentPositionedInfo.md#getMessageWithSeverity(boolean,boolean)), [getOffset](../../../document/DocumentPositionedInfo.md#getOffset()), [getOperationDescription](../../../document/DocumentPositionedInfo.md#getOperationDescription()), [getPreferredEngineName](../../../document/DocumentPositionedInfo.md#getPreferredEngineName()), [getSeverity](../../../document/DocumentPositionedInfo.md#getSeverity()), [getSeverityAsString](../../../document/DocumentPositionedInfo.md#getSeverityAsString()), [getStartEndPositions](../../../document/DocumentPositionedInfo.md#getStartEndPositions(java.lang.String)), [getSystemID](../../../document/DocumentPositionedInfo.md#getSystemID()), [hashCode](../../../document/DocumentPositionedInfo.md#hashCode()), [isElementTarget](../../../document/DocumentPositionedInfo.md#isElementTarget()), [isHighlightToColumn](../../../document/DocumentPositionedInfo.md#isHighlightToColumn()), [setAdditionalInfo](../../../document/DocumentPositionedInfo.md#setAdditionalInfo(java.net.URL)), [setAnchor](../../../document/DocumentPositionedInfo.md#setAnchor(ro.sync.exml.editor.Anchor)), [setColumn](../../../document/DocumentPositionedInfo.md#setColumn(int)), [setData](../../../document/DocumentPositionedInfo.md#setData(ro.sync.document.DPIData)), [setDetailedExceptionInfo](../../../document/DocumentPositionedInfo.md#setDetailedExceptionInfo(ro.sync.document.DetailedExceptionInfo)), [setDITAAdditionalInfo](../../../document/DocumentPositionedInfo.md#setDITAAdditionalInfo(ro.sync.document.DITAAdditionalInfo)), [setECAdditionalInfo](../../../document/DocumentPositionedInfo.md#setECAdditionalInfo(ro.sync.document.ECAdditionalInfo)), [setElementTarget](../../../document/DocumentPositionedInfo.md#setElementTarget(boolean)), [setEndColumn](../../../document/DocumentPositionedInfo.md#setEndColumn(int)), [setEndLine](../../../document/DocumentPositionedInfo.md#setEndLine(int)), [setEngineName](../../../document/DocumentPositionedInfo.md#setEngineName(java.lang.String)), [setErrorKey](../../../document/DocumentPositionedInfo.md#setErrorKey(java.lang.String)), [setHighlightToColumn](../../../document/DocumentPositionedInfo.md#setHighlightToColumn(boolean)), [setHtmlMessageFragment](../../../document/DocumentPositionedInfo.md#setHtmlMessageFragment(java.lang.String)), [setImposedInitialPage](../../../document/DocumentPositionedInfo.md#setImposedInitialPage(java.lang.String)), [setLength](../../../document/DocumentPositionedInfo.md#setLength(int)), [setLine](../../../document/DocumentPositionedInfo.md#setLine(int)), [setMaskPasswordsInURLs](../../../document/DocumentPositionedInfo.md#setMaskPasswordsInURLs(boolean)), [setMatchRange](../../../document/DocumentPositionedInfo.md#setMatchRange(int%5B%5D)), [setMessage](../../../document/DocumentPositionedInfo.md#setMessage(java.lang.String)), [setMessageHighlightOffset](../../../document/DocumentPositionedInfo.md#setMessageHighlightOffset(int)), [setOffset](../../../document/DocumentPositionedInfo.md#setOffset(int)), [setOperationDescription](../../../document/DocumentPositionedInfo.md#setOperationDescription(ro.sync.document.OperationDescription)), [setSeverity](../../../document/DocumentPositionedInfo.md#setSeverity(int)), [setStartEndPositionsMap](../../../document/DocumentPositionedInfo.md#setStartEndPositionsMap(java.util.Map)), [setSystemID](../../../document/DocumentPositionedInfo.md#setSystemID(java.lang.String)), [setTemporaryPositions](../../../document/DocumentPositionedInfo.md#setTemporaryPositions(javax.swing.text.Position,javax.swing.text.Position,java.lang.String)), [toString](../../../document/DocumentPositionedInfo.md#toString())
### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### AuthorDocumentPositionedInfo

public AuthorDocumentPositionedInfo([DocumentPositionedInfo](../../../document/DocumentPositionedInfo.md) dpi, [AuthorNode](../../extensions/api/node/AuthorNode.md) node)

Constructor.
  Parameters: dpi - The document positioned info to copy. node - The author node. The node base URL will be used as a system ID location.
### AuthorDocumentPositionedInfo

public AuthorDocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [AuthorNode](../../extensions/api/node/AuthorNode.md) node)

Constructor.
  Parameters: severity - Severity. One of the severity constants from class DocumentPositionedInfo: SEVERITY_ERROR, SEVERITY_FATAL, SEVERITY_INFO , SEVERITY_WARN. message - Error message. node - The author node. The node base URL will be used as a system ID location.
### AuthorDocumentPositionedInfo

public AuthorDocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, [AuthorNode](../../extensions/api/node/AuthorNode.md) node)

Constructor.
  Parameters: severity - Severity. One of the severity constants from class DocumentPositionedInfo: SEVERITY_ERROR, SEVERITY_FATAL, SEVERITY_INFO , SEVERITY_WARN. message - Error message. systemID - System ID node - The author node.
### AuthorDocumentPositionedInfo

public AuthorDocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int startOffset, int length)

Constructor.
  Parameters: severity - Severity. One of the severity constants from class DocumentPositionedInfo: SEVERITY_ERROR, SEVERITY_FATAL, SEVERITY_INFO , SEVERITY_WARN. message - Error message. systemID - System ID startOffset - The start offset of the problem, mapped in the Author content. length - The length of the problem, mapped in the Author content.
## Method Details

### getNode

public [AuthorNode](../../extensions/api/node/AuthorNode.md) getNode()
  Specified by: [getNode](IAuthorDocumentPositionedInfo.md#getNode()) in interface [IAuthorDocumentPositionedInfo](IAuthorDocumentPositionedInfo.md) Returns: The node to locate the message.
### setSelectEntireNode

public void setSelectEntireNode(boolean selectEntireNode)

Sets if the entire node should be selected or not.
  Parameters: selectEntireNode - true if the entire node should be selected.
### isSelectEntireNode

public boolean isSelectEntireNode()

Checks if the entire node should be selected.
  Specified by: [isSelectEntireNode](IAuthorDocumentPositionedInfo.md#isSelectEntireNode()) in interface [IAuthorDocumentPositionedInfo](IAuthorDocumentPositionedInfo.md) Returns: true if the entire node should be selected.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
