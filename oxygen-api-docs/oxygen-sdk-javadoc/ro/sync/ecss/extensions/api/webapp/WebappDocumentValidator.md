Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface WebappDocumentValidator
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappDocumentValidator
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [SCHEMATRON_IMPOSED_PHASE_ATTR_NAME](#SCHEMATRON_IMPOSED_PHASE_ATTR_NAME)
Editing session context attribute name.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DPILocation](DPILocation.md)> [getDPILocations](#getDPILocations(java.util.List))([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> dpInfo)
Compute for the given list of document position info the content offsets.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getSchematronPhases](#getSchematronPhases(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)
Get the phases defined in a Schematron file.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.editor.scenario.BaseScenario> [getValidationScenarios](#getValidationScenarios())()
Get validation scenarios associated with the document.
  [Callable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/concurrent/Callable.html)<[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)>> [getValidationTask](#getValidationTask())()
A task that tries to validate the document according to its schema and returns the list of found errors.
  void [setSchematronPhaseChooser](#setSchematronPhaseChooser(ro.sync.ecss.extensions.api.webapp.WebappSchematronPhaseChooser))([WebappSchematronPhaseChooser](WebappSchematronPhaseChooser.md) phaseChooser)
Sets a phase chooser which will be asked each time a Schematron validation that does not specify a phase is run.

## Field Details

### SCHEMATRON_IMPOSED_PHASE_ATTR_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) SCHEMATRON_IMPOSED_PHASE_ATTR_NAME

Editing session context attribute name. Its value would be used to impose a phase with that name in any Schematron file used for validation.
  Since: 22 See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.WebappDocumentValidator.SCHEMATRON_IMPOSED_PHASE_ATTR_NAME)

## Method Details

### getValidationTask

[Callable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/concurrent/Callable.html)<[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)>> getValidationTask()

A task that tries to validate the document according to its schema and returns the list of found errors.
  Returns: The validation task for the current document.
### getDPILocations

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DPILocation](DPILocation.md)> getDPILocations([List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentPositionedInfo](../../../../document/DocumentPositionedInfo.md)> dpInfo)

Compute for the given list of document position info the content offsets.
  Parameters: dpInfo - The list of document position info. Returns: The corresponding list of DPI location info.
### getValidationScenarios

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<ro.sync.exml.editor.scenario.BaseScenario> getValidationScenarios()

Get validation scenarios associated with the document.
  Returns: Validation scenarios associated with the document.
### getSchematronPhases

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getSchematronPhases([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) systemId)

Get the phases defined in a Schematron file.
  Parameters: systemId - The system ID of the Schematron file. Returns: The list of phases. Since: 22
### setSchematronPhaseChooser

void setSchematronPhaseChooser([WebappSchematronPhaseChooser](WebappSchematronPhaseChooser.md) phaseChooser)

Sets a phase chooser which will be asked each time a Schematron validation that does not specify a phase is run.
  Parameters: phaseChooser - The phase chooser. Since: 22
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
