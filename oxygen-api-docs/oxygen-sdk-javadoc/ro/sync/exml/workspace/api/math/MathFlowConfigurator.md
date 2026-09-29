Package [ro.sync.exml.workspace.api.math](package-summary.md)

# Interface MathFlowConfigurator
    All Known Subinterfaces: [EclipsePluginWorkspace](../../../../../../com/oxygenxml/workspace/api/eclipse/EclipsePluginWorkspace.md), [StandalonePluginWorkspace](../standalone/StandalonePluginWorkspace.md), [WebappPluginWorkspace](../../../../ecss/extensions/api/webapp/access/WebappPluginWorkspace.md)   All Known Implementing Classes: [AuthorComponentFactory](../../../../ecss/extensions/api/component/AuthorComponentFactory.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface MathFlowConfigurator
Provide access to MathFlow specific methods.
  Since: 15.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [setMathFlowFixedLicenseFile](#setMathFlowFixedLicenseFile(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) licenseFile)
Set the path to a license file.
  void [setMathFlowFixedLicenseKeyForComposer](#setMathFlowFixedLicenseKeyForComposer(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)
Set a fixed key for licensing the MathFlow composer used to view embedded MathML equations.
  void [setMathFlowFixedLicenseKeyForEditor](#setMathFlowFixedLicenseKeyForEditor(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)
Set a fixed key for licensing the MathFlow editor dialog used to edit embedded MathML equations.
  void [setMathFlowInstallationFolder](#setMathFlowInstallationFolder(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder)
Set the path to the MathFlow installation folder.

## Method Details

### setMathFlowFixedLicenseKeyForEditor

void setMathFlowFixedLicenseKeyForEditor([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)

Set a fixed key for licensing the MathFlow editor dialog used to edit embedded MathML equations.
  Parameters: fixedKey - The fixed key. The key needs to be obtained from MathFlow: http://dessci.com/ and has the following format: MFSCKKK-KKKKKK-KKKKK If no editor key will be given then MathFlow will be used neither for editing nor for rendering. Since: 14
### setMathFlowFixedLicenseKeyForComposer

void setMathFlowFixedLicenseKeyForComposer([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) fixedKey)

Set a fixed key for licensing the MathFlow composer used to view embedded MathML equations.
  Parameters: fixedKey - The fixed key. The key needs to be obtained from MathFlow: http://dessci.com/ and has the following format: MFSEKKK-KKKKKK-KKKKK If no composer key will be given then the fallback for rendering will be the Apache JEuclid library. Since: 14
### setMathFlowFixedLicenseFile

void setMathFlowFixedLicenseFile([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) licenseFile)

Set the path to a license file.
  Parameters: licenseFile - The path to the MathFlow license file. If the file contains both a license for the composer and for the editor, then both rendering and editing is supported. If the file contains a license only for the editor, rendering will be done using the open source JEuclid library. Since: 16
### setMathFlowInstallationFolder

void setMathFlowInstallationFolder([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) installationFolder)

Set the path to the MathFlow installation folder.
  Parameters: installationFolder - The MathFlow installation folder Since: 16
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
