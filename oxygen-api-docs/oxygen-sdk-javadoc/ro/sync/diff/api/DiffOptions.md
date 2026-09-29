Package [ro.sync.diff.api](package-summary.md)

# Class DiffOptions

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.diff.api.DiffOptions
   @API(type=EXTENDABLE, src=PUBLIC) public class DiffOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Holds options needed to decide which diff algorithm and which diff options will be used.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [AUTO](#AUTO)
The algorithm is automatically chosen based on content type, text length, options etc.
  static final int [CHARACTERS_COMPARE](#CHARACTERS_COMPARE)
Algorithm based on characters comparison.
  static final int [LINES_COMPARE](#LINES_COMPARE)
Algorithm based on line by line comparison.
  static final int [SYNTAX_AWARE](#SYNTAX_AWARE)
Algorithm based on comparing the syntax tokens.
  static final int [WORDS_COMPARE](#WORDS_COMPARE)
Algorithm based on words comparison.
  static final int [XML_ACCURATE](#XML_ACCURATE)
XML accurate diff based on Sasha and Zhang algorithm.
  static final int [XML_FAST](#XML_FAST)
Fast XML hybrid heuristic algorithm.

## Constructor Summary
 Constructors
Constructor

Description
 [DiffOptions](#%3Cinit%3E())()
Default constructor for default options.
  [DiffOptions](#%3Cinit%3E(int,boolean,int,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean,boolean))(int algorithm, boolean ignoreWhitespaces, int maxNumberOfDiffs, boolean ignorePI, boolean ignoreComments, boolean ignoreCDATA, boolean ignoreDOCTYPE, boolean ignoreText, boolean ignoreAttributesOrder, boolean ignorePrefixes, boolean ignoreNamespaces, boolean ignoreNamespaceDeclarations, boolean ignoreEntities, boolean mergeAdjacentDifferences, boolean markEndTagsAsDifferent, boolean ignoreStateOfEmptyElements)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 int [getAlgorithm](#getAlgorithm())()

 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDefaultXPath](#getDefaultXPath())()
Get the default XPath that will be used to ignore nodes from comparison it no XPath is specified in XPath combo from DIFF Files toolbar.
  int [getMaxNumberOfDiffs](#getMaxNumberOfDiffs())()

 boolean [isEnableHierarchicalDiff](#isEnableHierarchicalDiff())()

 boolean [isIgnoreAttributesOrder](#isIgnoreAttributesOrder())()

 boolean [isIgnoreCDATA](#isIgnoreCDATA())()

 boolean [isIgnoreComments](#isIgnoreComments())()

 boolean [isIgnoreDOCTYPE](#isIgnoreDOCTYPE())()

 boolean [isIgnoreEntities](#isIgnoreEntities())()

 boolean [isIgnoreNamespaceDeclarations](#isIgnoreNamespaceDeclarations())()

 boolean [isIgnoreNamespaces](#isIgnoreNamespaces())()

 boolean [isIgnoreNodesByXPath](#isIgnoreNodesByXPath())()
Check if the default XPath should be used to ignore nodes from comparison if no XPath is specified in XPath combo from DIFF Files toolbar
  boolean [isIgnorePI](#isIgnorePI())()

 boolean [isIgnorePrefixes](#isIgnorePrefixes())()

 boolean [isIgnoreStateOfEmptyElements](#isIgnoreStateOfEmptyElements())()

 boolean [isIgnoreText](#isIgnoreText())()

 boolean [isIgnoreWhitespaces](#isIgnoreWhitespaces())()

 boolean [isMarkEndTagsAsDifferent](#isMarkEndTagsAsDifferent())()

 boolean [isMergeAdjacentDifferences](#isMergeAdjacentDifferences())()

 void [setAlgorithm](#setAlgorithm(int))(int algorithm)

 void [setDefaultXPath](#setDefaultXPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultXPath)
Set default XPath that will be used to ignore nodes from comparison it no XPath is specified in XPath combo from DIFF Files toolbar.
  void [setEnableHierarchicalDiff](#setEnableHierarchicalDiff(boolean))(boolean enableHierarchicalDiff)
Enable or disable hierarchical diff.
  void [setIgnoreAttributesOrder](#setIgnoreAttributesOrder(boolean))(boolean ignoreAttributesOrder)

 void [setIgnoreCDATA](#setIgnoreCDATA(boolean))(boolean ignoreCDATA)

 void [setIgnoreComments](#setIgnoreComments(boolean))(boolean ignoreComments)

 void [setIgnoreDOCTYPE](#setIgnoreDOCTYPE(boolean))(boolean ignoreDOCTYPE)

 void [setIgnoreEntities](#setIgnoreEntities(boolean))(boolean ignoreEntities)

 void [setIgnoreNamespaceDeclarations](#setIgnoreNamespaceDeclarations(boolean))(boolean ignoreNamespaceDeclarations)

 void [setIgnoreNamespaces](#setIgnoreNamespaces(boolean))(boolean ignoreNamespaces)

 void [setIgnoreNodesByXPath](#setIgnoreNodesByXPath(boolean))(boolean ignoreNodesByXPath)
Set if the default XPath should be used to ignore nodes from comparison if no XPath is specified in XPath combo from DIFF Files toolbar
  void [setIgnorePI](#setIgnorePI(boolean))(boolean ignorePI)

 void [setIgnorePrefixes](#setIgnorePrefixes(boolean))(boolean ignorePrefixes)

 void [setIgnoreStateOfEmptyElements](#setIgnoreStateOfEmptyElements(boolean))(boolean ignoreStateOfEmptyElements)

 void [setIgnoreText](#setIgnoreText(boolean))(boolean ignoreText)

 void [setIgnoreWhitespaces](#setIgnoreWhitespaces(boolean))(boolean ignoreWhitespaces)

 void [setMarkEndTagsAsDifferent](#setMarkEndTagsAsDifferent(boolean))(boolean markEndTagsAsDifferent)

 void [setMaxNumberOfDiffs](#setMaxNumberOfDiffs(int))(int maxNumberOfDiffs)

 void [setMergeAdjacentDifferences](#setMergeAdjacentDifferences(boolean))(boolean mergeAdjacentDifferences)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### AUTO

public static final int AUTO

The algorithm is automatically chosen based on content type, text length, options etc.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.DiffOptions.AUTO)

### CHARACTERS_COMPARE

public static final int CHARACTERS_COMPARE

Algorithm based on characters comparison.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.DiffOptions.CHARACTERS_COMPARE)

### WORDS_COMPARE

public static final int WORDS_COMPARE

Algorithm based on words comparison.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.DiffOptions.WORDS_COMPARE)

### LINES_COMPARE

public static final int LINES_COMPARE

Algorithm based on line by line comparison.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.DiffOptions.LINES_COMPARE)

### SYNTAX_AWARE

public static final int SYNTAX_AWARE

Algorithm based on comparing the syntax tokens.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.DiffOptions.SYNTAX_AWARE)

### XML_FAST

public static final int XML_FAST

Fast XML hybrid heuristic algorithm.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.DiffOptions.XML_FAST)

### XML_ACCURATE

public static final int XML_ACCURATE

XML accurate diff based on Sasha and Zhang algorithm.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.diff.api.DiffOptions.XML_ACCURATE)

## Constructor Details

### DiffOptions

public DiffOptions(int algorithm, boolean ignoreWhitespaces, int maxNumberOfDiffs, boolean ignorePI, boolean ignoreComments, boolean ignoreCDATA, boolean ignoreDOCTYPE, boolean ignoreText, boolean ignoreAttributesOrder, boolean ignorePrefixes, boolean ignoreNamespaces, boolean ignoreNamespaceDeclarations, boolean ignoreEntities, boolean mergeAdjacentDifferences, boolean markEndTagsAsDifferent, boolean ignoreStateOfEmptyElements)

Constructor.
  Parameters: algorithm - The used algorithm, one of the constants:
        * [AUTO](#AUTO)
        * [CHARACTERS_COMPARE](#CHARACTERS_COMPARE)
        * [LINES_COMPARE](#LINES_COMPARE)
        * [SYNTAX_AWARE](#SYNTAX_AWARE)
        * [WORDS_COMPARE](#WORDS_COMPARE)
        * [XML_ACCURATE](#XML_ACCURATE)
        * [XML_FAST](#XML_FAST)
 ignoreWhitespaces - true if differences consisting only in whitespaces should be ignored. maxNumberOfDiffs - The maximum number of modifications you are interested in. If the document contain a larger number of differences the diff will only signal that they are different and stop after reaching the limit. ignorePI - true if processing instructions should be ignored. It applies when using XML aware algorithms. ignoreComments - true if comments should be ignored. It applies when using XML aware algorithms. ignoreCDATA - true if CDATA sections should be ignored. It applies when using XML aware algorithms. ignoreDOCTYPE - true if DOCTYPE sections should be ignored. It applies when using XML aware algorithms. ignoreText - true if differences in the text content should be ignored. It applies when using XML aware algorithms. ignoreAttributesOrder - true if the order of the attributes should be ignored. It applies when using XML aware algorithms. ignorePrefixes - true if the prefixes should be ignored. Even if this is set the comparing takes into account the namespacea. It applies when using XML aware algorithms. ignoreNamespaces - true if namespaces should be ignored. It applies when using XML aware algorithms. ignoreNamespaceDeclarations - true if the namespace declaration ("xmlns" attributes) should be ignored. It applies when using XML aware algorithms. ignoreEntities - true if entity content should be ignored. It applies when using XML aware algorithms. mergeAdjacentDifferences - true if adjacent differences should be merged and present as a single difference. Applies when using XML aware algorithms. markEndTagsAsDifferent - true if end tags with the same name for elements that are different in other sense will be shown as different also. It applies when using XML aware algorithms. ignoreStateOfEmptyElements - true if sequences representing empty elements like <a/> and <a></a>  will be considered identical. It applies when using XML aware algorithms.
### DiffOptions

public DiffOptions()

Default constructor for default options.

## Method Details

### getAlgorithm

public int getAlgorithm()
  Returns: Returns The used algorithm, one of the constants:
        * [AUTO](#AUTO)
        * [CHARACTERS_COMPARE](#CHARACTERS_COMPARE)
        * [LINES_COMPARE](#LINES_COMPARE)
        * [SYNTAX_AWARE](#SYNTAX_AWARE)
        * [WORDS_COMPARE](#WORDS_COMPARE)
        * [XML_ACCURATE](#XML_ACCURATE)
        * [XML_FAST](#XML_FAST)

### setAlgorithm

public void setAlgorithm(int algorithm)
  Parameters: algorithm - The algorithm to use, one of the constants:
        * [AUTO](#AUTO)
        * [CHARACTERS_COMPARE](#CHARACTERS_COMPARE)
        * [LINES_COMPARE](#LINES_COMPARE)
        * [SYNTAX_AWARE](#SYNTAX_AWARE)
        * [WORDS_COMPARE](#WORDS_COMPARE)
        * [XML_ACCURATE](#XML_ACCURATE)
        * [XML_FAST](#XML_FAST)

### getMaxNumberOfDiffs

public int getMaxNumberOfDiffs()
  Returns: Returns The maximum number of modifications you are interested in. If the document contain a larger number of differences the diff will only signal that they are different and stop after reaching the limit.
### setMaxNumberOfDiffs

public void setMaxNumberOfDiffs(int maxNumberOfDiffs)
  Parameters: maxNumberOfDiffs - The maximum number of modifications you are interested in. If the document contain a larger number of differences the diff will only signal that they are different and stop after reaching the limit.
### isIgnoreWhitespaces

public boolean isIgnoreWhitespaces()
  Returns: Returns true if differences consisting only in whitespaces will be ignored.
### setIgnoreWhitespaces

public void setIgnoreWhitespaces(boolean ignoreWhitespaces)
  Parameters: ignoreWhitespaces - true if differences consisting only in whitespaces should be ignored.
### isIgnorePI

public boolean isIgnorePI()
  Returns: Returns true if processing instructions are ignored. It applies when using XML aware algorithms.
### setIgnorePI

public void setIgnorePI(boolean ignorePI)
  Parameters: ignorePI - true if processing instructions should be ignored. It applies when using XML aware algorithms.
### isIgnoreComments

public boolean isIgnoreComments()
  Returns: Returns true if comments are be ignored. It applies when using XML aware algorithms.
### setIgnoreComments

public void setIgnoreComments(boolean ignoreComments)
  Parameters: ignoreComments - true if comments should be ignored. It applies when using XML aware algorithms.
### isIgnoreCDATA

public boolean isIgnoreCDATA()
  Returns: Returns true if CDATA sections are ignored. It applies when using XML aware algorithms.
### setIgnoreCDATA

public void setIgnoreCDATA(boolean ignoreCDATA)
  Parameters: ignoreCDATA - true if CDATA sections should be ignored. It applies when using XML aware algorithms.
### isIgnoreDOCTYPE

public boolean isIgnoreDOCTYPE()
  Returns: Returns true if DOCTYPE sections are ignored. It applies when using XML aware algorithms.
### setIgnoreDOCTYPE

public void setIgnoreDOCTYPE(boolean ignoreDOCTYPE)
  Parameters: ignoreDOCTYPE - true if DOCTYPE sections should be ignored. It applies when using XML aware algorithms.
### isIgnoreText

public boolean isIgnoreText()
  Returns: Returns true if differences in the text content is ignored. It applies when using XML aware algorithms.
### setIgnoreText

public void setIgnoreText(boolean ignoreText)
  Parameters: ignoreText - true if differences in the text content should be ignored. It applies when using XML aware algorithms.
### isIgnoreAttributesOrder

public boolean isIgnoreAttributesOrder()
  Returns: Returns true if the order of the attributes is ignored. It applies when using XML aware algorithms.
### setIgnoreAttributesOrder

public void setIgnoreAttributesOrder(boolean ignoreAttributesOrder)
  Parameters: ignoreAttributesOrder - true if the order of the attributes should be ignored. It applies when using XML aware algorithms.
### isIgnorePrefixes

public boolean isIgnorePrefixes()
  Returns: Returns true if the prefixes are ignored. Even if this is set the comparing takes into account the namespaces. It applies when using XML aware algorithms.
### setIgnorePrefixes

public void setIgnorePrefixes(boolean ignorePrefixes)
  Parameters: ignorePrefixes - true if the prefixes should be ignored. Even if this is set the comparing takes into account the namespaces. It applies when using XML aware algorithms.
### isIgnoreNamespaces

public boolean isIgnoreNamespaces()
  Returns: Returns true if namespaces are ignored. It applies when using XML aware algorithms.
### setIgnoreNamespaces

public void setIgnoreNamespaces(boolean ignoreNamespaces)
  Parameters: ignoreNamespaces - true if namespaces should be ignored. It applies when using XML aware algorithms.
### isIgnoreNamespaceDeclarations

public boolean isIgnoreNamespaceDeclarations()
  Returns: Returns true if the namespace declarations ("xmlns" attributes) are ignored. It applies when using XML aware algorithms.
### setIgnoreNamespaceDeclarations

public void setIgnoreNamespaceDeclarations(boolean ignoreNamespaceDeclarations)
  Parameters: ignoreNamespaceDeclarations - true if the namespace declarations ("xmlns" attributes) should be ignored. It applies when using XML aware algorithms.
### isIgnoreEntities

public boolean isIgnoreEntities()
  Returns: Returns true if entity content is ignored. It applies when using XML aware algorithms.
### setIgnoreEntities

public void setIgnoreEntities(boolean ignoreEntities)
  Parameters: ignoreEntities - true if entity content should be ignored. It applies when using XML aware algorithms.
### isIgnoreStateOfEmptyElements

public boolean isIgnoreStateOfEmptyElements()
  Returns: Returns true if sequences representing empty elements like <a/> and <a></a>  are considered identical. It applies when using XML aware algorithms.
### setIgnoreStateOfEmptyElements

public void setIgnoreStateOfEmptyElements(boolean ignoreStateOfEmptyElements)
  Parameters: ignoreStateOfEmptyElements - true if sequences representing empty elements like <a/> and <a></a>  will be considered identical. It applies when using XML aware algorithms.
### isMergeAdjacentDifferences

public boolean isMergeAdjacentDifferences()
  Returns: Returns true if adjacent differences are merged and present as a single difference. It applies when using XML aware algorithms.
### setMergeAdjacentDifferences

public void setMergeAdjacentDifferences(boolean mergeAdjacentDifferences)
  Parameters: mergeAdjacentDifferences - true if adjacent differences should be merged and present as a single difference. It applies when using XML aware algorithms.
### isMarkEndTagsAsDifferent

public boolean isMarkEndTagsAsDifferent()
  Returns: Returns true if end tags with the same name for elements that are different in other sense are shown as different also. It applies when using XML aware algorithms.
### setMarkEndTagsAsDifferent

public void setMarkEndTagsAsDifferent(boolean markEndTagsAsDifferent)
  Parameters: markEndTagsAsDifferent - true if end tags with the same name for elements that are different in other sense will be shown as different also. It applies when using XML aware algorithms.
### isIgnoreNodesByXPath

public boolean isIgnoreNodesByXPath()

Check if the default XPath should be used to ignore nodes from comparison if no XPath is specified in XPath combo from DIFF Files toolbar
  Returns: true if the default XPath expression should be used to ignore nodes from comparison if no other XPath is specified in XPath combo from DIFF Files toolbar
### setIgnoreNodesByXPath

public void setIgnoreNodesByXPath(boolean ignoreNodesByXPath)

Set if the default XPath should be used to ignore nodes from comparison if no XPath is specified in XPath combo from DIFF Files toolbar
  Parameters: ignoreNodesByXPath - true to use the default XPath should be used to ignore nodes from comparison if no XPath is specified in XPath combo from DIFF Files toolbar
### getDefaultXPath

public [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDefaultXPath()

Get the default XPath that will be used to ignore nodes from comparison it no XPath is specified in XPath combo from DIFF Files toolbar.
  Returns: The default XPath that will be used to ignore nodes from comparison it no XPath is specified in XPath combo from DIFF Files toolbar.
### setDefaultXPath

public void setDefaultXPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) defaultXPath)

Set default XPath that will be used to ignore nodes from comparison it no XPath is specified in XPath combo from DIFF Files toolbar.
  Parameters: defaultXPath - The default XPath that will be used to ignore nodes from comparison it no XPath is specified in XPath combo from DIFF Files toolbar.
### setEnableHierarchicalDiff

public void setEnableHierarchicalDiff(boolean enableHierarchicalDiff)

Enable or disable hierarchical diff.
  Parameters: enableHierarchicalDiff - If true differences from the same line or adjacent lines will be grouped and added in a parent difference. If false, no parent difference will be set for the created differences.
### isEnableHierarchicalDiff

public boolean isEnableHierarchicalDiff()
  Returns: Returns true if differences from the same line or adjacent lines will be grouped and added in a parent difference. false, if no parent difference will be set for the created differences. This option is available only for Text difference performer.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
