Package [ro.sync.document](package-summary.md)

# Interface ReportableDocumentPositionedInfo
    @API(type=EXTENDABLE, src=PUBLIC) public interface ReportableDocumentPositionedInfo
Interface used to mark the [DocumentPositionedInfo](DocumentPositionedInfo.md) that can be reported as a problem by using the "Report Problem" oXygen dialog. If the selection contains at least one [DocumentPositionedInfo](DocumentPositionedInfo.md) that implements this interface, the contextual menu will contain the "Report problem..." action. The text returned by the [getReport()](#getReport()) method will be set ad the problem description in the report problem dialog.
  Since: 19.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getReport](#getReport())()
Get the text to be used when reporting the problems associated with this [DocumentPositionedInfo](DocumentPositionedInfo.md).

## Method Details

### getReport

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getReport()

Get the text to be used when reporting the problems associated with this [DocumentPositionedInfo](DocumentPositionedInfo.md).
  Returns: The report text.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
