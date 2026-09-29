Package [ro.sync.document](package-summary.md)

# Class DocumentPositionedInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.document.DocumentPositionedInfo
   Direct Known Subclasses: [AuthorDocumentPositionedInfo](../ecss/component/validation/AuthorDocumentPositionedInfo.md)   @API(type=EXTENDABLE, src=PUBLIC) public class DocumentPositionedInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
This class holds information related to the document, refering to some errors, or find results. These informations hold the position in the document, the message and the systemId of the document in which they appear. If the systemId is null, then the semantics is that the info belongs to the currently edited file.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [NOT_KNOWN](#NOT_KNOWN)
If one of the components is not known, use this constant for it.
  static final int [SEVERITY_ERROR](#SEVERITY_ERROR)
Error message.
  static final int [SEVERITY_FATAL](#SEVERITY_FATAL)
Fatal error message.
  static final int [SEVERITY_INFO](#SEVERITY_INFO)
Information message.
  static final int [SEVERITY_WARN](#SEVERITY_WARN)
Warning message.

## Constructor Summary
 Constructors
Constructor

Description
 [DocumentPositionedInfo](#%3Cinit%3E(int))(int offset)
Constructor for a DPI used only to hold the current position in the editor.
  [DocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Constructor.
  [DocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String,java.lang.String))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)
Constructor.
  [DocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String,java.lang.String,int,int))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column)
Constructor.
  [DocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String,java.lang.String,int,int,int))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column, int length)
Constructor.
  [DocumentPositionedInfo](#%3Cinit%3E(int,java.lang.String,java.lang.String,int,int,int,int,java.net.URL,boolean))(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column, int length, int offset, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) additionalInfo, boolean highlightToColumn)
Constructor.
  [DocumentPositionedInfo](#%3Cinit%3E(int,ro.sync.document.MessageProvider,java.lang.String,int,int,int,int,int,int,java.net.URL,boolean))(int severity, ro.sync.document.MessageProvider messageProvider, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column, int endLine, int endColumn, int length, int offset, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) additionalInfo, boolean highlightToColumn)
Constructor.
  [DocumentPositionedInfo](#%3Cinit%3E(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asHTML](#asHTML())()
Build the HTML representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asHTML](#asHTML(boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Build the HTML representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asHTML](#asHTML(boolean,boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Builds the HTML representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asHTML](#asHTML(boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription, boolean asCompleteHTMLDocument)
Build the HTML representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asJSON](#asJSON())()
Build the JSON representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asJSON](#asJSON(boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Build the JSON representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asJSON](#asJSON(boolean,boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Build the JSON representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asText](#asText())()
Build the text representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asText](#asText(boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Build the text representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asText](#asText(boolean,boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Build the text representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asXML](#asXML())()
Build the XML representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asXML](#asXML(boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Build the XML representation of this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [asXML](#asXML(boolean,boolean,boolean,boolean,boolean,boolean,boolean))(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)
Build the XML representation of this DPI.
  boolean [equals](#equals(java.lang.Object))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)
Indicates whether some other document positioned information is "equal to" this one.
  static int [flipSeverity](#flipSeverity(int))(int severityToFlip)
Used to obtain the severity level to be used when sorting the DPIs by severity.
  protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAdditionalHtmlContent](#getAdditionalHtmlContent())()
Return the additional HTML content, if any.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getAdditionalInfo](#getAdditionalInfo())()
The URL for additional information if available.
  ro.sync.exml.editor.Anchor [getAnchor](#getAnchor())()
Get the error anchor if any.
  int [getColumn](#getColumn())()
Gets the column of the event.
  ro.sync.document.DPIData [getData](#getData())()
Getter for the user managed data.
  ro.sync.document.DetailedExceptionInfo [getDetailedExceptionInfo](#getDetailedExceptionInfo())()
Get detailed information about the problem.
  ro.sync.document.DITAAdditionalInfo [getDITAAdditionalInfo](#getDITAAdditionalInfo())()
Additional info about DITA completeness check.
  ro.sync.document.ECAdditionalInfo [getECAdditionalInfo](#getECAdditionalInfo())()
Additional info for Eclipse inner usage.
  int [getEndColumn](#getEndColumn())()
Get the highlight end column, or NOT_KNOWN if not available.
  int [getEndLine](#getEndLine())()
Get the highlight end line, or NOT_KNOWN if not available.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getEngineName](#getEngineName())()
Get the name of the engine who provided the error.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getErrorKey](#getErrorKey())()
Get the error key.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getHTMLMessage](#getHTMLMessage())()
Gets the HTML fragment to be presented when the message is displayed as HTML.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getImposedInitialPage](#getImposedInitialPage())()
Get the imposed initial page if a new editor will be opened.
  int [getLength](#getLength())()
Gets the length of the text that will be selected in the editor.
  int [getLine](#getLine())()
Gets the line attribute of the event
  int[] [getMatchRange](#getMatchRange())()
Get the match range if any.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage())()
Gets the message
  int [getMessageHighlightOffset](#getMessageHighlightOffset())()
Return the offset used to highlight the match inside the message in the results panel.
  ro.sync.document.MessageProvider [getMessageProvider](#getMessageProvider())()
The provider of messages from the current document position info.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessageWithEngine](#getMessageWithEngine())()
Gets the message prepended with the engine name, if available.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessageWithEngine](#getMessageWithEngine(boolean,boolean))(boolean includeSeverity, boolean includeErrorKey)
Gets the message prepended with the engine name, if available.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessageWithSeverity](#getMessageWithSeverity())()
Get the message with severity info as a char in the front of the message (W, E, F).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessageWithSeverity](#getMessageWithSeverity(boolean))(boolean includeEngineInformation)
Get the message with severity info as a char in the front of the message (W, E, F).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessageWithSeverity](#getMessageWithSeverity(boolean,boolean))(boolean includeEngineInformation, boolean includeErrorKey)
Gets the message with severity info as a char in the front of the message (W, E, F).
  int [getOffset](#getOffset())()
Get the event's offset.
  ro.sync.document.OperationDescription [getOperationDescription](#getOperationDescription())()
The description of an operation (that is an operation which is applied over multiple resources) that generated this DPI.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPreferredEngineName](#getPreferredEngineName())()
Get the preferred engine name who provided the error.
  int [getSeverity](#getSeverity())()
Gets the severity level.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSeverityAsString](#getSeverityAsString())()
Gets the severity level as string
  [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] [getStartEndPositions](#getStartEndPositions(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageId)
Get the temporary start and end positions for the current page.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getSystemID](#getSystemID())()
Gets the systemID attribute of the DocumentPositionedInfo object
  int [hashCode](#hashCode())()
Compute unique hash code for this object.
  boolean [isElementTarget](#isElementTarget())()
Return true if this DPI targets an XML element.
  boolean [isHighlightToColumn](#isHighlightToColumn())()
Check if the highlight must be made from column 0 to the specified column.
  void [setAdditionalInfo](#setAdditionalInfo(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Set the additional information URL if available.
  void [setAnchor](#setAnchor(ro.sync.exml.editor.Anchor))(ro.sync.exml.editor.Anchor anchor)
Set the error anchor.
  void [setColumn](#setColumn(int))(int column)
Sets the column of the event, or NOT_KNOWN if the column is not available.
  void [setData](#setData(ro.sync.document.DPIData))(ro.sync.document.DPIData data)
Setter for the user managed data.
  void [setDetailedExceptionInfo](#setDetailedExceptionInfo(ro.sync.document.DetailedExceptionInfo))(ro.sync.document.DetailedExceptionInfo detailedExceptionInfo)
Set detailed information about the problem.
  void [setDITAAdditionalInfo](#setDITAAdditionalInfo(ro.sync.document.DITAAdditionalInfo))(ro.sync.document.DITAAdditionalInfo additionalInfo)
Additional info about DITA completeness check.
  void [setECAdditionalInfo](#setECAdditionalInfo(ro.sync.document.ECAdditionalInfo))(ro.sync.document.ECAdditionalInfo additionalInfo)
Additional info for Eclipse inner usage.
  void [setElementTarget](#setElementTarget(boolean))(boolean isElementTarget)
Set true if this DPI targets an XML element.
  void [setEndColumn](#setEndColumn(int))(int endColumn)
Sets the end column of the highlight.
  void [setEndLine](#setEndLine(int))(int endLine)
Sets the end line of the highlight.
  void [setEngineName](#setEngineName(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) engineName)
Set the name of the engine who provided the error.
  void [setErrorKey](#setErrorKey(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorKey)
The error validation key.
  void [setHighlightToColumn](#setHighlightToColumn(boolean))(boolean how)
Set highlight strategy for the document positioned information visual presentation.
  void [setHtmlMessageFragment](#setHtmlMessageFragment(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) htmlMessageFragment)
Set a special HTML fragment which needs to be presented instead of the message when the DPI is serialized to HTML.
  void [setImposedInitialPage](#setImposedInitialPage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedInitialPage)
Set the imposed initial page in which to open the DPI for a new editor.
  void [setLength](#setLength(int))(int length)
Sets the length of the selected text.
  void [setLine](#setLine(int))(int line)
Sets the line of the event, or NOT_KNOWN if the line is not available.
  void [setMaskPasswordsInURLs](#setMaskPasswordsInURLs(boolean))(boolean maskPasswordsInURLs)
Set mask passwords in URLs, true by default.
  void [setMatchRange](#setMatchRange(int%5B%5D))(int[] matchRange)
Set the match range.
  void [setMessage](#setMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)
Sets the message.
  void [setMessageHighlightOffset](#setMessageHighlightOffset(int))(int messageHighlightOffset)
Set the offset used to highlight the match inside the message in the results panel.
  void [setOffset](#setOffset(int))(int offset)
Sets the event's offset.
  void [setOperationDescription](#setOperationDescription(ro.sync.document.OperationDescription))(ro.sync.document.OperationDescription operationDescription)
Sets the description of an operation (that is an operation which is applied over multiple resources) that generated this DPI.
  void [setSeverity](#setSeverity(int))(int severity)
Sets the error severity.
  void [setStartEndPositionsMap](#setStartEndPositionsMap(java.util.Map))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[]> startEndPositionsMap)
Set a new temporary positions map.
  void [setSystemID](#setSystemID(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)
Sets the systemID of the event.
  void [setTemporaryPositions](#setTemporaryPositions(javax.swing.text.Position,javax.swing.text.Position,java.lang.String))([Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) startPosition, [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) endPosition, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageId)
Set the temporary start and end positions used for keeping the DPI synchronized with the highlight range from the page.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [toString](#toString())()
Gets the string representation.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### SEVERITY_INFO

public static final int SEVERITY_INFO

Information message.
  See Also:
        * [Constant Field Values](../../../constant-values.md#ro.sync.document.DocumentPositionedInfo.SEVERITY_INFO)

### SEVERITY_WARN

public static final int SEVERITY_WARN

Warning message.
  See Also:
        * [Constant Field Values](../../../constant-values.md#ro.sync.document.DocumentPositionedInfo.SEVERITY_WARN)

### SEVERITY_ERROR

public static final int SEVERITY_ERROR

Error message.
  See Also:
        * [Constant Field Values](../../../constant-values.md#ro.sync.document.DocumentPositionedInfo.SEVERITY_ERROR)

### SEVERITY_FATAL

public static final int SEVERITY_FATAL

Fatal error message.
  See Also:
        * [Constant Field Values](../../../constant-values.md#ro.sync.document.DocumentPositionedInfo.SEVERITY_FATAL)

### NOT_KNOWN

public static final int NOT_KNOWN

If one of the components is not known, use this constant for it.
  See Also:
        * [Constant Field Values](../../../constant-values.md#ro.sync.document.DocumentPositionedInfo.NOT_KNOWN)

## Constructor Details

### DocumentPositionedInfo

public DocumentPositionedInfo(int offset)

Constructor for a DPI used only to hold the current position in the editor.
  Parameters: offset - Start of selection.
### DocumentPositionedInfo

public DocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column, int length)

Constructor.
  Parameters: severity - the severity level of the message. message - the error message. systemID - the system ID. line - the line on which the error occurred in the document. column - the column on which the error occurred. length - the length of the text to be selected.
### DocumentPositionedInfo

public DocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column, int length, int offset, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) additionalInfo, boolean highlightToColumn)

Constructor.
  Parameters: severity - the severity level of the message. message - the error message. systemID - the system ID. line - the line on which the error occurred in the document. column - the column on which the error occurred. length - the length of the text to be selected. offset - the offset in the document additionalInfo - the URL from which the user can retrieve additional info about the error. highlightToColumn - true if the opener must highlight the entire text from the 1 column to the column number. This is useful in case of error checks, like validations or well-formed.
### DocumentPositionedInfo

public DocumentPositionedInfo(int severity, ro.sync.document.MessageProvider messageProvider, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column, int endLine, int endColumn, int length, int offset, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) additionalInfo, boolean highlightToColumn)

Constructor. Uses a message provider for the cases in which composing the message takes a lot of time (e.g. XPATH).
  Parameters: severity - the severity level of the message. messageProvider - the error message provider. systemID - the system ID. line - the line on which the error occurred in the document. column - the column on which the error occurred. endLine - the highlighted text must end in this line. endColumn - the highlighted text must end in this column. length - the length of the text to be selected. offset - the offset in the document additionalInfo - the URL from which the user can retrieve additional info about the error. highlightToColumn - true if the opener must highlight the entire text from the 1 column to the column number. This is useful in case of error checks, like validations or well-formed.
### DocumentPositionedInfo

public DocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID, int line, int column)

Constructor.
  Parameters: severity - the severity level of the message. message - the error message. systemID - the system ID. line - the line on which the error occurred in the document. column - the column on which the error occurred.
### DocumentPositionedInfo

public DocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)

Constructor.
  Parameters: severity - the severity level of the message. message - the error message. systemID - the system ID.
### DocumentPositionedInfo

public DocumentPositionedInfo(int severity, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Constructor.
  Parameters: severity - the severity level of the message. message - the error message.
### DocumentPositionedInfo

public DocumentPositionedInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Constructor. Use this for IDEAccess#openAndShowLocation. Tries to identify the line and column parameters in the URL fragment.
  Parameters: url - The URL to open in the editor.
## Method Details

### flipSeverity

public static int flipSeverity(int severityToFlip)

Used to obtain the severity level to be used when sorting the DPIs by severity. This is done to allow natural sorting by severity, having the SEVERITY_FATAL to be the small value and the SEVERITY_INFO the big value.
  Parameters: severityToFlip - The severity of a DPI to be translated into natural ordering. Returns: The natural ordering value to be used for a DPI' severity level.
### equals

public boolean equals([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) obj)

Indicates whether some other document positioned information is "equal to" this one.
  Overrides: [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.equals(java.lang.Object)](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))

### hashCode

public int hashCode()

Compute unique hash code for this object. Hashcode is compatible with equals method.
  Overrides: [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) See Also:
        * [Object.hashCode()](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode())

### setSeverity

public void setSeverity(int severity)

Sets the error severity.
  Parameters: severity - The new severity value. One of: SEVERITY_INFO, SEVERITY_WARN, SEVERITY_ERROR or SEVERITY_FATAL
### setColumn

public void setColumn(int column)

Sets the column of the event, or NOT_KNOWN if the column is not available.
  Parameters: column - The column
### setLine

public void setLine(int line)

Sets the line of the event, or NOT_KNOWN if the line is not available.
  Parameters: line - The new line value, 1 based.
### setMessage

public void setMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) message)

Sets the message. It will clear any user info if there is present into the message.
  Parameters: message - The new message
### setMaskPasswordsInURLs

public void setMaskPasswordsInURLs(boolean maskPasswordsInURLs)

Set mask passwords in URLs, true by default.
  Parameters: maskPasswordsInURLs - true to mask passwords in URLs which are part of the message.
### setLength

public void setLength(int length)

Sets the length of the selected text.
  Parameters: length - The length of the selected text.
### setSystemID

public void setSystemID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemID)

Sets the systemID of the event.
  Parameters: systemID - The new systemID value
### getLength

public int getLength()

Gets the length of the text that will be selected in the editor.
  Returns: The length of the text to be selected.
### getColumn

public int getColumn()

Gets the column of the event.
  Returns: The column value, 1 based. Can be NOT_KNOWN.
### getSeverity

public int getSeverity()

Gets the severity level. One of: SEVERITY_INFO, SEVERITY_WARN, SEVERITY_ERROR or SEVERITY_FATAL
  Returns: The severity value
### getSeverityAsString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSeverityAsString()

Gets the severity level as string
  Returns: The severity value string
### getLine

public int getLine()

Gets the line attribute of the event
  Returns: The line value, 1 based. Can be NOT_KNOWN.
### getMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage()

Gets the message
  Returns: The message value
### getHTMLMessage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getHTMLMessage()

Gets the HTML fragment to be presented when the message is displayed as HTML.
  Returns: A special HTML fragment which needs to be presented when the message is presented as HTML. null if there is no HTML flavor.
### getMessageProvider

public ro.sync.document.MessageProvider getMessageProvider()

The provider of messages from the current document position info.
  Returns: Returns the message provider.
### getMessageWithEngine

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessageWithEngine()

Gets the message prepended with the engine name, if available.
  Returns: The message.
### getMessageWithEngine

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessageWithEngine(boolean includeSeverity, boolean includeErrorKey)

Gets the message prepended with the engine name, if available. Could also include the severity and the error key.
  Parameters: includeSeverity - true to include the severity level (other than INFO). includeErrorKey - true to include the error code (if available). Returns: the error message built as requested.
### getMessageWithSeverity

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessageWithSeverity()

Get the message with severity info as a char in the front of the message (W, E, F).
  Returns: The message prefixed with the severity char. For INFO we do not present such a char.
### getMessageWithSeverity

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessageWithSeverity(boolean includeEngineInformation)

Get the message with severity info as a char in the front of the message (W, E, F). Could include the engine information.
  Parameters: includeEngineInformation - true to include engine name. Returns: The message prefixed with the severity char. For INFO we do not present such a char.
### getMessageWithSeverity

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessageWithSeverity(boolean includeEngineInformation, boolean includeErrorKey)

Gets the message with severity info as a char in the front of the message (W, E, F). Could also include engine info and error code.
  Parameters: includeEngineInformation - true to include engine name. includeErrorKey - true to include error code. Returns: The message prefixed with the severity char. For INFO we do not present such a char.
### getSystemID

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getSystemID()

Gets the systemID attribute of the DocumentPositionedInfo object
  Returns: The systemID value
### setOffset

public void setOffset(int offset)

Sets the event's offset. can be NOT_KNOWN
  Parameters: offset - the new offset.
### getOffset

public int getOffset()

Get the event's offset. Can be NOT_KNOWN
  Returns: the offset
### toString

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toString()

Gets the string representation.
  Overrides: [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()) in class [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) Returns: the string representation.
### getAdditionalInfo

public [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getAdditionalInfo()

The URL for additional information if available.
  Returns: The additional information URL, or null.
### setAdditionalInfo

public void setAdditionalInfo([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Set the additional information URL if available.
  Parameters: url - The URL at which the user can find additional information.
### isHighlightToColumn

public boolean isHighlightToColumn()

Check if the highlight must be made from column 0 to the specified column.
  Returns: True if the highlight must be made from column 0 to the specified column.
### setHighlightToColumn

public void setHighlightToColumn(boolean how)

Set highlight strategy for the document positioned information visual presentation.
  Parameters: how - true if the visual part should highlight from column 0 to specified column false otherwise.
### getEndColumn

public int getEndColumn()

Get the highlight end column, or NOT_KNOWN if not available.
  Returns: the highlight end column, or NOT_KNOWN.
### getEndLine

public int getEndLine()

Get the highlight end line, or NOT_KNOWN if not available.
  Returns: the highlight end line or NOT_KNOWN.
### setEndLine

public void setEndLine(int endLine)

Sets the end line of the highlight.
  Parameters: endLine - The end line of the highlight.
### setEndColumn

public void setEndColumn(int endColumn)

Sets the end column of the highlight.
  Parameters: endColumn - The end column of the highlight.
### setData

public void setData(ro.sync.document.DPIData data)

Setter for the user managed data.
  Parameters: data - The user managed data.
### getData

public ro.sync.document.DPIData getData()

Getter for the user managed data.
  Returns: The user managed data.
### setDetailedExceptionInfo

public void setDetailedExceptionInfo(ro.sync.document.DetailedExceptionInfo detailedExceptionInfo)

Set detailed information about the problem.
  Parameters: detailedExceptionInfo - The additional detailed info.
### getDetailedExceptionInfo

public ro.sync.document.DetailedExceptionInfo getDetailedExceptionInfo()

Get detailed information about the problem.
  Returns: Returns the additional detailed info.
### setEngineName

public void setEngineName([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) engineName)

Set the name of the engine who provided the error.
  Parameters: engineName - The source engine name who provided the error.
### getEngineName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getEngineName()

Get the name of the engine who provided the error.
  Returns: Returns the source engine name who provided the error. null if no was engine set.
### getPreferredEngineName

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPreferredEngineName()

Get the preferred engine name who provided the error. For DITA the engine is given by problem type.
  Returns: Returns the source engine name who provided the error.
### asXML

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asXML()

Build the XML representation of this DPI.
  Returns: The XML representation of the DPI.
### asXML

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asXML(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Build the XML representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The XML representation of the DPI.
### asXML

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asXML(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Build the XML representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeErrorCode - true if error code should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The XML representation of the DPI.
### asJSON

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asJSON()

Build the JSON representation of this DPI.
  Returns: The JSON representation of the DPI.
### asJSON

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asJSON(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Build the JSON representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The JSON representation of the DPI.
### asJSON

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asJSON(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Build the JSON representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeErrorCode - true if error code should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The JSON representation of the DPI.
### asText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asText()

Build the text representation of this DPI.
  Returns: The text representation of this DPI.
### asText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asText(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Build the text representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The text representation of this DPI.
### asText

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asText(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Build the text representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeErrorCode - true if error code should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The text representation of this DPI.
### getImposedInitialPage

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getImposedInitialPage()

Get the imposed initial page if a new editor will be opened.
  Returns: the imposed initial page
### setImposedInitialPage

public void setImposedInitialPage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) imposedInitialPage)

Set the imposed initial page in which to open the DPI for a new editor.
  Parameters: imposedInitialPage - The imposed initial page.
### getAnchor

public ro.sync.exml.editor.Anchor getAnchor()

Get the error anchor if any.
  Returns: the error anchor if any.
### setAnchor

public void setAnchor(ro.sync.exml.editor.Anchor anchor)

Set the error anchor.
  Parameters: anchor - The anchor to set.
### getMatchRange

public int[] getMatchRange()

Get the match range if any.
  Returns: The match range if possible.
### setMatchRange

public void setMatchRange(int[] matchRange)

Set the match range.
  Parameters: matchRange - The match range.
### getMessageHighlightOffset

public int getMessageHighlightOffset()

Return the offset used to highlight the match inside the message in the results panel.
  Returns: the message highlight offset.
### setMessageHighlightOffset

public void setMessageHighlightOffset(int messageHighlightOffset)

Set the offset used to highlight the match inside the message in the results panel.
  Parameters: messageHighlightOffset - The offset to be set.
### setOperationDescription

public void setOperationDescription(ro.sync.document.OperationDescription operationDescription)

Sets the description of an operation (that is an operation which is applied over multiple resources) that generated this DPI. Can be null.
  Parameters: operationDescription - the description of an operation (that is an operation which is applied over multiple resources) that generated this DPI. Can be null.
### getOperationDescription

public ro.sync.document.OperationDescription getOperationDescription()

The description of an operation (that is an operation which is applied over multiple resources) that generated this DPI. Can be null.
  Returns: the description of an operation (that is an operation which is applied over multiple resources) that generated this DPI. Can be null.
### getDITAAdditionalInfo

public ro.sync.document.DITAAdditionalInfo getDITAAdditionalInfo()

Additional info about DITA completeness check.
  Returns: Returns additional info.
### setDITAAdditionalInfo

public void setDITAAdditionalInfo(ro.sync.document.DITAAdditionalInfo additionalInfo)

Additional info about DITA completeness check.
  Parameters: additionalInfo - Additional info about DITA completeness check.
### getECAdditionalInfo

public ro.sync.document.ECAdditionalInfo getECAdditionalInfo()

Additional info for Eclipse inner usage.
  Returns: Returns additional info.
### setECAdditionalInfo

public void setECAdditionalInfo(ro.sync.document.ECAdditionalInfo additionalInfo)

Additional info for Eclipse inner usage.
  Parameters: additionalInfo - Additional info for Elipse inner usage.
### setTemporaryPositions

public void setTemporaryPositions([Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) startPosition, [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html) endPosition, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageId)

Set the temporary start and end positions used for keeping the DPI synchronized with the highlight range from the page.
  Parameters: startPosition - The start position. endPosition - The end position. Always exclusive. pageId - The id of the page for which the positions were created, one of [EditorPageConstants](../exml/editor/EditorPageConstants.md) constants.
### getStartEndPositions

public [Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[] getStartEndPositions([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pageId)

Get the temporary start and end positions for the current page.
  Parameters: pageId - The id of the page for which we want the positions, one of [EditorPageConstants](../exml/editor/EditorPageConstants.md) constants. Returns: An arrays with two positions, representing the start and end positions of the DPI. The end position is exclusive. Can be null if the page is closed, or the DPI is not synchronized with the modifications from editor.
### setStartEndPositionsMap

public void setStartEndPositionsMap([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Position](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/Position.html)[]> startEndPositionsMap)

Set a new temporary positions map.
  Parameters: startEndPositionsMap - The temporary positions map.
### asHTML

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asHTML()

Build the HTML representation of this DPI.
  Returns: The HTML representation of this DPI.
### asHTML

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asHTML(boolean includeSeverity, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Build the HTML representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The HTML representation of this DPI.
### asHTML

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asHTML(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription)

Builds the HTML representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeErrorCode - true if error code should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. Returns: The HTML representation of this DPI.
### asHTML

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) asHTML(boolean includeSeverity, boolean includeErrorCode, boolean includeAdditionalInfo, boolean includeDescription, boolean includeSystemID, boolean includeLocation, boolean includeOperationDescription, boolean asCompleteHTMLDocument)

Build the HTML representation of this DPI.
  Parameters: includeSeverity - true if severity details should be included. includeErrorCode - true if error code should be included. includeAdditionalInfo - true if additional info details should be included. includeDescription - true if description details should be included. includeSystemID - true if system ID details should be included. includeLocation - true if location details should be included. includeOperationDescription - true if operation description details should be included. asCompleteHTMLDocument - true for a complete valid HTML document representation, including style section. The title of the HTML document is "Message". If false, then the HTML representation only consists of a 'table' inside a 'div' section, and no styling at all. Returns: The HTML representation of this DPI.
### getAdditionalHtmlContent

protected [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAdditionalHtmlContent()

Return the additional HTML content, if any.
  Returns: the additional HTML content, if any.
### setHtmlMessageFragment

public void setHtmlMessageFragment([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) htmlMessageFragment)

Set a special HTML fragment which needs to be presented instead of the message when the DPI is serialized to HTML.
  Parameters: htmlMessageFragment - The fragment to set.
### setErrorKey

public void setErrorKey([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) errorKey)

The error validation key.
  Parameters: errorKey - The error key.
### getErrorKey

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getErrorKey()

Get the error key.
  Returns: Returns the error key.
### isElementTarget

public boolean isElementTarget()

Return true if this DPI targets an XML element.
  Returns: true if this DPI targets an XML element.
### setElementTarget

public void setElementTarget(boolean isElementTarget)

Set true if this DPI targets an XML element.
  Parameters: isElementTarget - true if this DPI targets an XML element.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
