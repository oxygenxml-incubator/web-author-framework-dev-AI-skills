Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface WebappSchematronPhaseChooser
    @API(type=EXTENDABLE, src=PUBLIC) public interface WebappSchematronPhaseChooser
Interface that is asked to provide the schematron phase to use.
  Since: 22
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [choosePhase](#choosePhase(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) schematronSystemId)
Chooses the Schematron phase to use for a specific schematron.

## Method Details

### choosePhase

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) choosePhase([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) schematronSystemId)

Chooses the Schematron phase to use for a specific schematron. In order to obtain the available phases in that Schematron file, one can use [WebappDocumentValidator.getSchematronPhases(String)](WebappDocumentValidator.md#getSchematronPhases(java.lang.String)). Note that a call to this method needs to parse the file. Caching the phases is recommended.
  Parameters: schematronSystemId - The system ID of the Schematron file. Returns: The chosen phase.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
