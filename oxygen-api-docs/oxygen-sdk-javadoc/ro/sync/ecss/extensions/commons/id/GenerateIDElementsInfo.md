Package [ro.sync.ecss.extensions.commons.id](package-summary.md)

# Class GenerateIDElementsInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo
   @API(type=INTERNAL, src=PUBLIC) public class GenerateIDElementsInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Information about the list of elements for which to generate auto ID + if the auto ID generation is activated

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DEFAULT_ID_GENERATION_PATTERN](#DEFAULT_ID_GENERATION_PATTERN)
The default id generation pattern.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [FILTER_IDS_ON_COPY_KEY](#FILTER_IDS_ON_COPY_KEY)
The key from options
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [GENERATE_ID_ELEMENTS_ACTIVE_KEY](#GENERATE_ID_ELEMENTS_ACTIVE_KEY)
The key from options
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [GENERATE_ID_ELEMENTS_KEY](#GENERATE_ID_ELEMENTS_KEY)
The key from options
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [GENERATE_ID_PATTERN_KEY](#GENERATE_ID_PATTERN_KEY)
The key from options
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [ID_PATTERN_DESCRIPTION](#ID_PATTERN_DESCRIPTION)
Description for the id pattern macro.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LOCAL_NAME_PATTERN_DESCRIPTION](#LOCAL_NAME_PATTERN_DESCRIPTION)
Description for the local name pattern macro.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LOCAL_NAME_PATTERN_MACRO](#LOCAL_NAME_PATTERN_MACRO)
Local name pattern macro.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PATTERN_TOOLTIP](#PATTERN_TOOLTIP)
The default pattern tooltip.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [UUID_PATTERN_DESCRIPTION](#UUID_PATTERN_DESCRIPTION)
Description for the uuid pattern macro.

## Constructor Summary
 Constructors
Constructor

Description
 [GenerateIDElementsInfo](#%3Cinit%3E(boolean,java.lang.String,java.lang.String%5B%5D))(boolean autoGenerateIds, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementsWithIDGeneration)
Constructor.
  [GenerateIDElementsInfo](#%3Cinit%3E(boolean,java.lang.String,java.lang.String%5B%5D,boolean))(boolean autoGenerateIds, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementsWithIDGeneration, boolean filterIDsOnCopy)
Constructor.
  [GenerateIDElementsInfo](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) defaultOptions)
Constructor.

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [generateID](#generateID(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementLocalName)
Generate an ID from a pattern for the specified element.
  static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [generateID](#generateID(java.lang.String,java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editorLocation)
Generate an ID from a pattern for the specified element.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getAttrQname](#getAttrQname())()
Get the QName of the attribute for which to generate the
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] [getElementsWithIDGeneration](#getElementsWithIDGeneration())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getIdGenerationPattern](#getIdGenerationPattern())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getPatternTooltip](#getPatternTooltip())()
Get the pattern tooltip.
  boolean [isAutoGenerateIDs](#isAutoGenerateIDs())()

 boolean [isFilterIDsOnCopy](#isFilterIDsOnCopy())()

 static [GenerateIDElementsInfo](GenerateIDElementsInfo.md) [loadDefaultsFromConfiguration](#loadDefaultsFromConfiguration(ro.sync.ecss.extensions.api.AuthorAccess,java.lang.String))([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) proposedXMLResourceName)
Load from the XML configuration.
  void [saveToOptions](#saveToOptions(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](../../api/AuthorAccess.md) authorAccess)
Save to persistent options
  void [setAutoGenerateIds](#setAutoGenerateIds(boolean))(boolean autoGenerateIds)
Set auto generate IDs.
  void [setElementsWithIDGeneration](#setElementsWithIDGeneration(java.lang.String%5B%5D))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementsWithIDGeneration)
Set a list of elements with ID generation
  void [setIdGenerationPattern](#setIdGenerationPattern(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern)
Set the ID generation pattern.
  void [setPatternTooltip](#setPatternTooltip(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) patternTooltip)
Set the pattern tooltip which will be shown in the configuration dialog.
  void [setRemoveIDsOnCopy](#setRemoveIDsOnCopy(boolean))(boolean removeIDsOnCopy)
Set the flag which controls whether the IDs will be removed on copy.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### GENERATE_ID_ELEMENTS_KEY

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) GENERATE_ID_ELEMENTS_KEY

The key from options
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.GENERATE_ID_ELEMENTS_KEY)

### GENERATE_ID_ELEMENTS_ACTIVE_KEY

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) GENERATE_ID_ELEMENTS_ACTIVE_KEY

The key from options
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.GENERATE_ID_ELEMENTS_ACTIVE_KEY)

### GENERATE_ID_PATTERN_KEY

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) GENERATE_ID_PATTERN_KEY

The key from options
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.GENERATE_ID_PATTERN_KEY)

### FILTER_IDS_ON_COPY_KEY

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) FILTER_IDS_ON_COPY_KEY

The key from options
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.FILTER_IDS_ON_COPY_KEY)

### LOCAL_NAME_PATTERN_MACRO

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LOCAL_NAME_PATTERN_MACRO

Local name pattern macro.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.LOCAL_NAME_PATTERN_MACRO)

### LOCAL_NAME_PATTERN_DESCRIPTION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LOCAL_NAME_PATTERN_DESCRIPTION

Description for the local name pattern macro.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.LOCAL_NAME_PATTERN_DESCRIPTION)

### UUID_PATTERN_DESCRIPTION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) UUID_PATTERN_DESCRIPTION

Description for the uuid pattern macro.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.UUID_PATTERN_DESCRIPTION)

### ID_PATTERN_DESCRIPTION

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) ID_PATTERN_DESCRIPTION

Description for the id pattern macro.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.ID_PATTERN_DESCRIPTION)

### DEFAULT_ID_GENERATION_PATTERN

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DEFAULT_ID_GENERATION_PATTERN

The default id generation pattern.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.DEFAULT_ID_GENERATION_PATTERN)

### PATTERN_TOOLTIP

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PATTERN_TOOLTIP

The default pattern tooltip.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.ecss.extensions.commons.id.GenerateIDElementsInfo.PATTERN_TOOLTIP)

## Constructor Details

### GenerateIDElementsInfo

public GenerateIDElementsInfo([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [GenerateIDElementsInfo](GenerateIDElementsInfo.md) defaultOptions)

Constructor.
  Parameters: authorAccess - The author access defaultOptions - The default options.
### GenerateIDElementsInfo

public GenerateIDElementsInfo(boolean autoGenerateIds, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementsWithIDGeneration)

Constructor.
  Parameters: autoGenerateIds - true to auto generate IDs. idGenerationPattern - The pattern for id generation. elementsWithIDGeneration - List of elements for which to generate IDs.
### GenerateIDElementsInfo

public GenerateIDElementsInfo(boolean autoGenerateIds, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementsWithIDGeneration, boolean filterIDsOnCopy)

Constructor.
  Parameters: autoGenerateIds - true to auto generate IDs. idGenerationPattern - The pattern for id generation. elementsWithIDGeneration - List of elements for which to generate IDs. filterIDsOnCopy - Filter IDs when copying content in the same file.
## Method Details

### isAutoGenerateIDs

public boolean isAutoGenerateIDs()
  Returns: true if auto generates IDs for elements.
### isFilterIDsOnCopy

public boolean isFilterIDsOnCopy()
  Returns: Returns true to filter IDs when copying content in the Author page.
### getIdGenerationPattern

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getIdGenerationPattern()
  Returns: Returns the pattern for id generation.
### getElementsWithIDGeneration

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] getElementsWithIDGeneration()
  Returns: Returns the elements for which to generate IDs.
### saveToOptions

public void saveToOptions([AuthorAccess](../../api/AuthorAccess.md) authorAccess)

Save to persistent options
  Parameters: authorAccess - The author access
### generateID

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) generateID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementLocalName)

Generate an ID from a pattern for the specified element.
  Parameters: idGenerationPattern - The pattern. elementLocalName - The element local name Returns: The generated ID.
### generateID

public static [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) generateID([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) elementLocalName, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) editorLocation)

Generate an ID from a pattern for the specified element.
  Parameters: idGenerationPattern - The pattern. elementLocalName - The element local name editorLocation - Editor location Returns: The generated ID.
### setAutoGenerateIds

public void setAutoGenerateIds(boolean autoGenerateIds)

Set auto generate IDs.
  Parameters: autoGenerateIds - true to auto generate IDs.
### setElementsWithIDGeneration

public void setElementsWithIDGeneration([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)[] elementsWithIDGeneration)

Set a list of elements with ID generation
  Parameters: elementsWithIDGeneration - a list of elements with ID generation
### setRemoveIDsOnCopy

public void setRemoveIDsOnCopy(boolean removeIDsOnCopy)

Set the flag which controls whether the IDs will be removed on copy.
  Parameters: removeIDsOnCopy - The filterIDsOnCopy to set.
### setIdGenerationPattern

public void setIdGenerationPattern([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) idGenerationPattern)

Set the ID generation pattern.
  Parameters: idGenerationPattern - The idGeneration pattern.
### getPatternTooltip

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getPatternTooltip()

Get the pattern tooltip. Can be overwritten to provide another tooltip.
  Returns: the pattern tooltip.
### setPatternTooltip

public void setPatternTooltip([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) patternTooltip)

Set the pattern tooltip which will be shown in the configuration dialog.
  Parameters: patternTooltip - the pattern tooltip which will be shown in the configuration dialog.
### loadDefaultsFromConfiguration

public static [GenerateIDElementsInfo](GenerateIDElementsInfo.md) loadDefaultsFromConfiguration([AuthorAccess](../../api/AuthorAccess.md) authorAccess, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) proposedXMLResourceName)

Load from the XML configuration.
  Parameters: authorAccess - The author access proposedXMLResourceName - The proposed name of the resource from which to load the configuration. Returns: The information loaded from the configuration.
### getAttrQname

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getAttrQname()

Get the QName of the attribute for which to generate the
  Returns: Returns the attrQname.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
