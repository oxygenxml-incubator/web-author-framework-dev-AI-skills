# Serialized Form

## Package [ro.sync.contentcompletion.editor](ro/sync/contentcompletion/editor/package-summary.md)

### Class ro.sync.contentcompletion.editor.CCCellRenderer

class CCCellRenderer extends [JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### forAuthor

```
boolean forAuthor
```

##### nodeCustomizer

```
XMLNodeRendererCustomizer nodeCustomizer
```

##### recentlyUsedEntries

```
ro.sync.contentcompletion.editor.MRUPromoter recentlyUsedEntries
```

##### showRecentlyUsedEntries

```
boolean showRecentlyUsedEntries
```

### Class ro.sync.contentcompletion.editor.CCDocumentationWindow

class CCDocumentationWindow extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### componentResizer

```
ro.sync.ui.ComponentResizer componentResizer
```

##### currentFocusOwner

```
JComponent currentFocusOwner
```

##### currentTextComponent

```
JTextComponent currentTextComponent
```

##### focusAdapter

```
FocusAdapter focusAdapter
```

##### helper

```
ro.sync.options.PropertiesHelper helper
```

##### hideWindowListener

```
AWTEventListener hideWindowListener
```

##### htmlEditorPane

```
ro.sync.ui.application.ApplicationEditorPane htmlEditorPane
```

##### labelF2

```
JLabel labelF2
```

##### labelPanel

```
JPanel labelPanel
```

##### originalDocumentation

```
String originalDocumentation
```

##### parentComponent

```
JComponent parentComponent
```

##### scrollPane

```
ro.sync.ui.application.ApplicationScrollPane scrollPane
```

##### showEntireTooltipMessageKeyListener

```
KeyAdapter showEntireTooltipMessageKeyListener
```

##### textArea

```
ro.sync.ui.application.ApplicationTextArea textArea
```

### Class ro.sync.contentcompletion.editor.CCEditorBase

class CCEditorBase extends ro.sync.contentcompletion.editor.NonCCEditor implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### ccSupport

```
ro.sync.contentcompletion.editor.CCSupport ccSupport
```

##### hyperlinkManager

```
ro.sync.exml.editor.hyperlink.HyperlinkManager hyperlinkManager
```

##### indentOptionsProvider

```
ro.sync.exml.editor.prettyprint.IndentOptionsProvider indentOptionsProvider
```

##### matchingTagHighlighter

```
ro.sync.exml.editor.xmleditor.TagHighlighter matchingTagHighlighter
```

##### multipleIntervalsRenamer

```
ro.sync.ui.textcomponent.MultipleIntervalsRenamer multipleIntervalsRenamer
```

##### pasteEffector

```
ro.sync.contentcompletion.editor.PasteEffector pasteEffector
```

##### quickAssistManager

```
ro.sync.exml.editor.quickassist.QuickAssistManager quickAssistManager
```

##### quickAssistStripe

```
ro.sync.ui.stripes.QuickAssistStripe quickAssistStripe
```

##### quickAssistWindow

```
ro.sync.exml.editor.quickassist.impl.QuickAssistWindow quickAssistWindow
```

##### rangePositions

```
List<Integer> rangePositions
```

##### renameHighlightPainter

```
Highlighter.HighlightPainter renameHighlightPainter
```

##### renameHighlightPainterProvider

```
ro.sync.ui.ruler.RangeHighlightPainterProvider renameHighlightPainterProvider
```

##### renameInplaceRanges

```
List<? extends ro.sync.ui.ruler.AbstractRange> renameInplaceRanges
```

##### renameInplaceRangesClass

```
ro.sync.ui.ruler.RangeClass renameInplaceRangesClass
```

##### renameRangeRenderer

```
ro.sync.ui.ruler.RangeRulerRenderer renameRangeRenderer
```

##### renamerHighlightsHelper

```
ro.sync.ui.textcomponent.RenamerHighlightsHelper renamerHighlightsHelper
```

##### skipRangeModelEvents

```
boolean skipRangeModelEvents
```

##### usedFont

```
Font usedFont
```

### Class ro.sync.contentcompletion.editor.CCEditorTooltip

class CCEditorTooltip extends ro.sync.contentcompletion.editor.CCEditorBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### lastEndTooltipPos

```
int lastEndTooltipPos
```

##### lastPoint

```
Point lastPoint
```

##### lastStartTooltipPos

```
int lastStartTooltipPos
```

##### showAnnotationsAsTooltip

```
boolean showAnnotationsAsTooltip
```

##### timerTask

```
ro.sync.ui.application.ApplicationTimerTask timerTask
```

##### tooltipWindow

```
ro.sync.contentcompletion.editor.CCDocumentationWindow tooltipWindow
```

##### tooltipWindowCloseSuperviser

```
ro.sync.contentcompletion.editor.TooltipWindowCloseSuperviser tooltipWindowCloseSuperviser
```

### Class ro.sync.contentcompletion.editor.CCSupport.CaretEventImpl

class CaretEventImpl extends [CaretEvent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/event/CaretEvent.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.contentcompletion.editor.CCTableCellRenderer

class CCTableCellRenderer extends [JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### forAuthor

```
boolean forAuthor
```

##### nodeCustomizer

```
XMLNodeRendererCustomizer nodeCustomizer
```

### Class ro.sync.contentcompletion.editor.CCTextField

class CCTextField extends ro.sync.syntaxhighlight.textfield.SHTextField implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### ccSupport

```
ro.sync.contentcompletion.editor.CCSupport ccSupport
```

### Class ro.sync.contentcompletion.editor.CCTextFieldWithValidation

class CCTextFieldWithValidation extends ro.sync.ui.OverlayableComponent implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.contentcompletion.editor.CCWindow

class CCWindow extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### cellRenderer

```
ro.sync.contentcompletion.editor.CCCellRenderer cellRenderer
```

##### componentResizer

```
ro.sync.ui.ComponentResizer componentResizer
```

##### documentationWindow

```
ro.sync.contentcompletion.editor.CCDocumentationWindow documentationWindow
```

##### forbiddenLineStripe

```
Rectangle forbiddenLineStripe
```

##### helper

```
ro.sync.options.PropertiesHelper helper
```

##### lastDimension

```
Dimension lastDimension
```

##### lastExaminedPrefix

```
String lastExaminedPrefix
```

##### list

```
ro.sync.contentcompletion.editor.CCWindow.CustomizedProposalsList list
```

##### listeners

```
List listeners
```

##### maxRecentlyUsed

```
int maxRecentlyUsed
```

##### nodeCustomizer

```
XMLNodeRendererCustomizer nodeCustomizer
```

##### owner

```
JComponent owner
```

##### recentlyUsedEntries

```
ro.sync.contentcompletion.editor.MRUPromoter recentlyUsedEntries
```

##### scrollPane

```
ro.sync.ui.application.ApplicationScrollPane scrollPane
```

##### showRecentEntries

```
boolean showRecentEntries
```

##### verticalMargin

```
int verticalMargin
```

##### visibleRowCount

```
int visibleRowCount
```

##### warningTooltip

```
ro.sync.ecss.component.WarningTooltipWindow warningTooltip
```

### Class ro.sync.contentcompletion.editor.CCWindow.CustomizedProposalsList

class CustomizedProposalsList extends [JList](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JList.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.contentcompletion.editor.DualCCEditor

class DualCCEditor extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### activeEditor

```
ro.sync.contentcompletion.editor.SimpleCCEditor activeEditor
```

##### autoSpellChecker

```
ro.sync.azcheck.ui.JTextAutoSpellCheck autoSpellChecker
```

##### breakPointCreator

```
ro.sync.ui.marks.BreakPointsManager breakPointCreator
```

##### caretListeners

```
List<CaretListener> caretListeners
```

##### caretListenersMap

```
Map<String,ro.sync.syntaxhighlight.InhibitableCaretListener> caretListenersMap
```

##### commonDocument

```
Document commonDocument
```

##### createXMLStripes

```
boolean createXMLStripes
```

##### defaultDividerSize

```
int defaultDividerSize
```

##### dropHandlerListeners

```
List dropHandlerListeners
```

##### enableAdjustmentListener

```
boolean enableAdjustmentListener
```

##### firstCCEditor

```
ro.sync.contentcompletion.editor.SimpleCCEditor firstCCEditor
```

##### firstEditorUpdateViewPortPositionListener

```
ro.sync.contentcompletion.editor.DualCCEditor.UpdateViewPortPositionListener firstEditorUpdateViewPortPositionListener
```

##### focusListeners

```
List focusListeners
```

##### keyListeners

```
List<KeyListener> keyListeners
```

##### markCreatorAnyName

```
ro.sync.ui.marks.MarkCreatorAnyName markCreatorAnyName
```

##### operationOnMatchingTagsAllowed

```
boolean operationOnMatchingTagsAllowed
```

##### pasteEffector

```
ro.sync.contentcompletion.editor.PasteEffector pasteEffector
```

##### popupListeners

```
List popupListeners
```

##### quickAssistManager

```
ro.sync.exml.editor.quickassist.QuickAssistManager quickAssistManager
```

##### rangeModel

```
ro.sync.ui.ruler.FilterRangeModel rangeModel
```

##### restoreViewportPositionDocListener

```
DocumentListener restoreViewportPositionDocListener
```

##### secondCCEditor

```
ro.sync.contentcompletion.editor.SimpleCCEditor secondCCEditor
```

##### secondEditorFocusListener

```
ro.sync.contentcompletion.editor.DualCCEditor.SetActiveEditorFocusListener secondEditorFocusListener
```

##### secondEditorUpdateViewPortPositionListener

```
ro.sync.contentcompletion.editor.DualCCEditor.UpdateViewPortPositionListener secondEditorUpdateViewPortPositionListener
```

##### showMarkAlways

```
boolean showMarkAlways
```

##### splitPane

```
ro.sync.contentcompletion.editor.DualCCEditor.DividerSizeIgnoreSplitPane splitPane
```

##### tooltipWindowCloseSuperviser

```
ro.sync.contentcompletion.editor.TooltipWindowCloseSuperviser tooltipWindowCloseSuperviser
```

##### undoSelectionRestorer

```
ro.sync.contentcompletion.editor.UndoSelectionRestorer undoSelectionRestorer
```

##### validationStatusPanel

```
ro.sync.exml.editor.validate.ValidationStatusPanel validationStatusPanel
```

### Class ro.sync.contentcompletion.editor.NonCCEditor

class NonCCEditor extends ro.sync.syntaxhighlight.LineNumberedEditor implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### beginLineAction

```
Action beginLineAction
```

##### currentHighlightsMap

```
Map<String,Set> currentHighlightsMap
```

##### endLineAction

```
Action endLineAction
```

##### fireCaretUpdate

```
boolean fireCaretUpdate
```

##### foldStripe

```
ro.sync.ui.stripes.text.fold.FoldStripe foldStripe
```

##### i18NPropertyListener

```
PropertyChangeListener i18NPropertyListener
```

##### i18PropertySet

```
boolean i18PropertySet
```

##### indentOnEnter

```
boolean indentOnEnter
```

##### indentOnPaste

```
boolean indentOnPaste
```

##### leftArrowAction

```
Action leftArrowAction
```

##### originalLeftArrowAction

```
Action originalLeftArrowAction
```

##### originalRightArrowAction

```
Action originalRightArrowAction
```

##### rangeModel

```
ro.sync.ui.ruler.RangeModel rangeModel
```

##### rangeRuler

```
ro.sync.ui.ruler.RangeRuler rangeRuler
```

##### rangeRulerValidationResultsRenderer

```
ro.sync.contentcompletion.errors.ErrorsRangeRulerRenderer rangeRulerValidationResultsRenderer
```

##### rightArrowAction

```
Action rightArrowAction
```

##### selectionBeginLineAction

```
Action selectionBeginLineAction
```

##### selectionEndLineAction

```
Action selectionEndLineAction
```

##### selectionIsChanging

```
boolean selectionIsChanging
```

##### selectRangeNearCaretTimer

```
Timer selectRangeNearCaretTimer
```

##### shiftTabAction

```
Action shiftTabAction
```

##### showFoldStripe

```
boolean showFoldStripe
```

##### synchronizedHighlighter

```
ro.sync.ui.PriorityHighlighter synchronizedHighlighter
```

##### validationResultsHighlighter

```
ro.sync.contentcompletion.editor.NonCCEditor.ProblemsHighlighter validationResultsHighlighter
```

##### zoomSupport

```
ro.sync.exml.view.zoom.FontZoomSupport zoomSupport
```

### Class ro.sync.contentcompletion.editor.SimpleCCEditor

class SimpleCCEditor extends ro.sync.contentcompletion.editor.CCEditorTooltip implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### functionArgumentsPresenter

```
ro.sync.contentcompletion.editor.functionsignature.FSPresenter functionArgumentsPresenter
```

### Class ro.sync.contentcompletion.editor.SimpleCCEditorWithSearch

class SimpleCCEditorWithSearch extends ro.sync.contentcompletion.editor.SimpleCCEditor implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.contentcompletion.editor.SimpleCCEditorWithValidation

class SimpleCCEditorWithValidation extends ro.sync.ui.OverlayableComponent implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.contentcompletion.xsl](ro/sync/contentcompletion/xsl/package-summary.md)

### Class ro.sync.contentcompletion.xsl.XSLResultSchemaInfo

class XSLResultSchemaInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### detectSchema

```
boolean detectSchema
```

##### schemaType

```
String schemaType
```

##### systemID

```
String systemID
```

## Package [ro.sync.diff.api](ro/sync/diff/api/package-summary.md)

### Exception [ro.sync.diff.api.DiffException](ro/sync/diff/api/DiffException.md)

class DiffException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.diff.factory](ro/sync/diff/factory/package-summary.md)

### Exception [ro.sync.diff.factory.CannotHandleException](ro/sync/diff/factory/CannotHandleException.md)

class CannotHandleException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### systemId

```
String systemId
```

The system ID of the file that cannot be handled.

### Class ro.sync.diff.factory.DiffInfo

class DiffInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### algorithm

```
int algorithm
```

##### algorithm3Way

```
int algorithm3Way
```

##### defaultXPath

```
String defaultXPath
```

##### ignoreAttributesOrder

```
boolean ignoreAttributesOrder
```

##### ignoreCDATA

```
boolean ignoreCDATA
```

##### ignoreComments

```
boolean ignoreComments
```

##### ignoreDOCTYPE

```
boolean ignoreDOCTYPE
```

##### ignoreEntities

```
boolean ignoreEntities
```

##### ignoreNamespaceDeclarations

```
boolean ignoreNamespaceDeclarations
```

##### ignoreNamespaces

```
boolean ignoreNamespaces
```

##### ignoreNodesByXPath

```
boolean ignoreNodesByXPath
```

##### ignorePI

```
boolean ignorePI
```

##### ignorePrefixes

```
boolean ignorePrefixes
```

##### ignoreStateOfEmptyElements

```
boolean ignoreStateOfEmptyElements
```

##### ignoreText

```
boolean ignoreText
```

##### ignoreWhitespaces

```
boolean ignoreWhitespaces
```

##### markEndTagsAsDifferent

```
boolean markEndTagsAsDifferent
```

##### maxNoOfDiffs

```
int maxNoOfDiffs
```

##### maxNoOfDiffs3Way

```
int maxNoOfDiffs3Way
```

##### mergeAdjacentDifferences

```
boolean mergeAdjacentDifferences
```

## Package [ro.sync.diff.merge.api](ro/sync/diff/merge/api/package-summary.md)

### Exception [ro.sync.diff.merge.api.MergeFilesException](ro/sync/diff/merge/api/MergeFilesException.md)

class MergeFilesException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.document](ro/sync/document/package-summary.md)

### Class ro.sync.document.CompoundEditDocument

class CompoundEditDocument extends ro.sync.document.TagsAwareDocument implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.document.CompoundEditUndoManager

class CompoundEditUndoManager extends [AuthorUndoManager](ro/sync/ecss/extensions/api/AuthorUndoManager.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### commitNextEdit

```
boolean commitNextEdit
```

##### editWhenLastSaveOperationOccurred

```
UndoableEdit editWhenLastSaveOperationOccurred
```

##### inProgressCompoundEdit

```
CompoundEdit inProgressCompoundEdit
```

##### lastEdit

```
UndoableEdit lastEdit
```

##### lastProcessedMasteredCompoundEdit

```
UndoableEdit lastProcessedMasteredCompoundEdit
```

##### lastSource

```
Object lastSource
```

##### listeners

```
Vector<UndoableEditListener> listeners
```

##### markSavedOperationEdit

```
boolean markSavedOperationEdit
```

##### savedAtEndOfEdits

```
boolean savedAtEndOfEdits
```

### Class ro.sync.document.CustomCompoundEdit

class CustomCompoundEdit extends [CompoundEdit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/CompoundEdit.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### atomicListener

```
ro.sync.document.AtomicEditListener atomicListener
```

### Exception ro.sync.document.DPIToGenericNodeMapper.MappingDoneException

class MappingDoneException extends [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.document.EditableDocument

class EditableDocument extends ro.sync.document.OxygenPlainDocument implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### editInReadOnlyListeners

```
List<ro.sync.document.EditInReadOnlyContentListener> editInReadOnlyListeners
```

##### isEditable

```
boolean isEditable
```

##### isForcedEditable

```
boolean isForcedEditable
```

### Class ro.sync.document.EditorUndoManager

class EditorUndoManager extends ro.sync.document.CompoundEditUndoManager implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### listeners

```
List<ro.sync.document.EditorUndoManager.AttemptedUndoOnEmptyEditsListener> listeners
```

### Class ro.sync.document.FoldDocumentImpl

class FoldDocumentImpl extends ro.sync.document.HardWrapDocument implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### foldModel

```
ro.sync.document.fold.FoldModel foldModel
```

##### foldSerializer

```
ro.sync.document.fold.FoldSerializer foldSerializer
```

##### foldVerifier

```
ro.sync.document.fold.FoldVerifier foldVerifier
```

### Class ro.sync.document.HardWrapDocument

class HardWrapDocument extends ro.sync.document.MarkDocument implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### hardWrap

```
boolean hardWrap
```

##### maxLineWidth

```
int maxLineWidth
```

### Class ro.sync.document.LineDocumentImpl

class LineDocumentImpl extends ro.sync.document.UndoableDocumentImpl implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### docReadStateListeners

```
List<ro.sync.document.DocumentReadStateListener> docReadStateListeners
```

##### ignoreCR

```
boolean ignoreCR
```

##### indentOnEnter

```
boolean indentOnEnter
```

##### lastNotifiedListeners

```
List<DocumentListener> lastNotifiedListeners
```

##### preserveLineStartSpaces

```
boolean preserveLineStartSpaces
```

##### processStringForCR

```
boolean processStringForCR
```

##### useSpacesInsteadTab

```
boolean useSpacesInsteadTab
```

### Class ro.sync.document.MarkDocument

class MarkDocument extends ro.sync.document.LineDocumentImpl implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### marksManager

```
ro.sync.ui.marks.MarksManager marksManager
```

### Class ro.sync.document.MasteredCompoundEdit

class MasteredCompoundEdit extends ro.sync.document.CustomCompoundEdit implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### offsetRedo

```
int offsetRedo
```

##### offsetUndo

```
int offsetUndo
```

##### redoSelection

```
int[] redoSelection
```

##### undoSelection

```
int[] undoSelection
```

### Class ro.sync.document.OxygenPlainDocument

class OxygenPlainDocument extends [AbstractDocument](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/AbstractDocument.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### added

```
Vector added
```

##### bidiActivated

```
boolean bidiActivated
```

##### bidiDocumentLimit

```
int bidiDocumentLimit
```

##### bidiEnabled

```
boolean bidiEnabled
```

##### bidiLimitReached

```
boolean bidiLimitReached
```

##### defaultRoot

```
AbstractDocument.AbstractElement defaultRoot
```

##### propertyChangeListeners

```
ConcurrentLinkedQueue<PropertyChangeListener> propertyChangeListeners
```

##### removed

```
Vector removed
```

### Class ro.sync.document.SyntaxDocumentImpl

class SyntaxDocumentImpl extends ro.sync.document.FoldDocumentImpl implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### checkBidi

```
boolean checkBidi
```

##### damageRepairListeners

```
List<ro.sync.document.DamageRepairListener> damageRepairListeners
```

##### ghostTextProvider

```
GhostTextProvider ghostTextProvider
```

##### ltm

```
ro.sync.outline.LiveTreeModel ltm
```

##### oldIndent

```
boolean oldIndent
```

##### tokenMarker

```
ro.sync.syntaxhighlight.marker.TokenMarker tokenMarker
```

### Class ro.sync.document.TagsAwareDocument

class TagsAwareDocument extends ro.sync.document.SyntaxDocumentImpl implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### amtr

```
ro.sync.document.AbstractMatchingTagRenamer amtr
```

##### editTagsEnabled

```
boolean editTagsEnabled
```

##### renameTagsEnabled

```
boolean renameTagsEnabled
```

### Class ro.sync.document.UndoableDocumentImpl

class UndoableDocumentImpl extends ro.sync.document.EditableDocument implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### disableBIDIChecking

```
boolean disableBIDIChecking
```

## Package [ro.sync.ecss.component](ro/sync/ecss/component/package-summary.md)

### Class ro.sync.ecss.component.AuthorAdditionalDockableViewer

class AuthorAdditionalDockableViewer extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### caretAndDocListener

```
ro.sync.ecss.component.AuthorCoalescingDocumentAndCaretListener caretAndDocListener
```

##### viewport

```
ro.sync.ecss.component.AuthorViewport viewport
```

### Class ro.sync.ecss.component.AuthorClipboardObject

class AuthorClipboardObject extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
  serialVersionUID: 6031409352129925303L
#### Serialization Methods

##### readObject

private void readObject([ObjectInputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/ObjectInputStream.html) arg0)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [ClassNotFoundException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassNotFoundException.html)
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [ClassNotFoundException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassNotFoundException.html)
##### writeObject

private void writeObject([ObjectOutputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/ObjectOutputStream.html) arg0)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

#### Serialized Fields

##### fragments

```
ro.sync.ecss.component.AuthorDocumentFragmentClipboardObject[] fragments
```

##### htmlContent

```
String htmlContent
```

##### metadata

```
AuthorContentMetadata metadata
```

##### objectID

```
String objectID
```

##### originalDocInfo

```
ro.sync.ecss.component.AuthorDocumentInfo originalDocInfo
```

##### purposeID

```
int purposeID
```

##### textContent

```
String textContent
```

##### visualRepresentation

```
SelectionInterpretationMode visualRepresentation
```

### Class ro.sync.ecss.component.AuthorSchemaAwareOptions

class AuthorSchemaAwareOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### enableSmartDelete

```
boolean enableSmartDelete
```

##### enableSmartPaste

```
boolean enableSmartPaste
```

##### enableSmartTyping

```
boolean enableSmartTyping
```

##### insertOnlyAttributeValuesFromCCList

```
boolean insertOnlyAttributeValuesFromCCList
```

##### insertOnlyElemensFromCCList

```
boolean insertOnlyElemensFromCCList
```

##### isVerifyDeleteElementTagsAction

```
boolean isVerifyDeleteElementTagsAction
```

##### isVerifyJoinAction

```
boolean isVerifyJoinAction
```

##### isVerifyPasteAndDNDAction

```
boolean isVerifyPasteAndDNDAction
```

##### isVerifyTypingAction

```
boolean isVerifyTypingAction
```

##### isVerifyUnwrapAction

```
boolean isVerifyUnwrapAction
```

##### schemaAwareEditingMode

```
String schemaAwareEditingMode
```

##### showAllPossibleElementsInCCList

```
boolean showAllPossibleElementsInCCList
```

##### showAvailableCCItemsOnEnter

```
boolean showAvailableCCItemsOnEnter
```

### Class ro.sync.ecss.component.AuthorTransferredObject

class AuthorTransferredObject extends ro.sync.ecss.component.AuthorClipboardObject implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### fragmentsIntervals

```
List<int[]> fragmentsIntervals
```

### Class ro.sync.ecss.component.CaretInfoWindow

class CaretInfoWindow extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### accessibilityInfoTextField

```
ro.sync.ui.UndoableTextField accessibilityInfoTextField
```

##### caretInfoTooltip

```
ro.sync.ecss.component.CaretInfoTooltip caretInfoTooltip
```

##### ghost

```
boolean ghost
```

##### hideTimer

```
Timer hideTimer
```

##### parent

```
ro.sync.ecss.component.SwingAuthorHostComponent parent
```

##### rootPane

```
JRootPane rootPane
```

##### shownOnRequest

```
boolean shownOnRequest
```

##### swingGraphicsWrapper

```
ro.sync.exml.view.SwingGraphicsWrapper swingGraphicsWrapper
```

##### windowInteractor

```
ro.sync.ecss.component.CaretInfoWindowInteractor windowInteractor
```

### Class ro.sync.ecss.component.FloatingToolbarWindow

class FloatingToolbarWindow extends ro.sync.ecss.component.RoundShadowPanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### authorExtensionBuilderProvider

```
ro.sync.ecss.extensions.AuthorExtensionBuilderProvider authorExtensionBuilderProvider
```

##### authorHostComp

```
ro.sync.ecss.component.SwingAuthorHostComponent authorHostComp
```

##### authorViewport

```
ro.sync.ecss.component.AuthorViewport authorViewport
```

##### floatingToolbarEditingHelper

```
ro.sync.ecss.component.editor.FloatingToolbarEditingHelper floatingToolbarEditingHelper
```

##### inplaceEditorFactory

```
ro.sync.ecss.component.editor.AuthorInplaceEditorFactory inplaceEditorFactory
```

##### interactor

```
ro.sync.ecss.component.FloatingToolbarInteractor interactor
```

##### rootPane

```
JRootPane rootPane
```

##### updateAndShowToolbarTimer

```
ro.sync.exml.editor.helpers.SwingTimer updateAndShowToolbarTimer
```

##### wasAddedInLayeredPane

```
boolean wasAddedInLayeredPane
```

### Class ro.sync.ecss.component.RoundShadowPanel

class RoundShadowPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### arcRadius

```
int arcRadius
```

##### shadowColor

```
Color shadowColor
```

##### shadowDepth

```
int shadowDepth
```

### Class ro.sync.ecss.component.SwingAuthorHostComponent

class SwingAuthorHostComponent extends ro.sync.exml.view.SwingHostComponentBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### accessibleContext

```
AccessibleContext accessibleContext
```

##### authorDropHandler

```
ro.sync.ecss.component.AuthorDropHandler authorDropHandler
```

##### caretPositionInfoWindow

```
ro.sync.ecss.component.CaretInfoWindow caretPositionInfoWindow
```

##### ccSupport

```
ro.sync.ecss.component.ui.context.AuthorCCSupport ccSupport
```

##### componentHeightResizeListener

```
ro.sync.ecss.component.CoalescingComponentResizeListener componentHeightResizeListener
```

##### componentResizeListener

```
ro.sync.ecss.component.CoalescingComponentResizeListener componentResizeListener
```

##### dropManager

```
ro.sync.ui.dnd.MultiHandlerDropManager dropManager
```

##### floatingToolbarWindow

```
ro.sync.ecss.component.FloatingToolbarWindow floatingToolbarWindow
```

##### heavyFormControlHelper

```
ro.sync.ecss.component.editor.heavy.HeavyFormControlManager heavyFormControlHelper
```

##### imageCacher

```
ro.sync.ecss.images.ImageCacher imageCacher
```

##### initialNoOfVisibleWindows

```
int initialNoOfVisibleWindows
```

##### inplaceEditorHelper

```
ro.sync.ecss.component.editor.AuthorInplaceEditorHelper inplaceEditorHelper
```

##### inplaceRendererHelper

```
ro.sync.ecss.component.editor.AuthorInplaceRendererHelper inplaceRendererHelper
```

##### inputMethodRequestsHandler

```
ro.sync.ecss.component.InputMethodRequestsHandler inputMethodRequestsHandler
```

##### lastHeight

```
int lastHeight
```

##### lastWidth

```
int lastWidth
```

##### saHighlightsWidgetHelper

```
ro.sync.ecss.component.SAHighlightsWidgetHelper saHighlightsWidgetHelper
```

##### textLayoutFactory

```
ro.sync.ecss.component.TextLayoutFactory textLayoutFactory
```

##### viewportLayoutInProgress

```
boolean viewportLayoutInProgress
```

##### warningTooltipWindow

```
ro.sync.ecss.component.WarningTooltipWindow warningTooltipWindow
```

### Class ro.sync.ecss.component.WarningTooltipWindow

class WarningTooltipWindow extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### goToOptionsPanel

```
JPanel goToOptionsPanel
```

##### hideTimer

```
Timer hideTimer
```

##### linkLabel

```
ro.sync.exml.LinkLabel linkLabel
```

##### optionPageKey

```
String optionPageKey
```

##### suggestionArea

```
ro.sync.ui.application.ApplicationTextArea suggestionArea
```

##### titleLabel

```
JLabel titleLabel
```

##### warningTitlePanel

```
JPanel warningTitlePanel
```

## Package [ro.sync.ecss.component.editor](ro/sync/ecss/component/editor/package-summary.md)

### Class ro.sync.ecss.component.editor.InplaceEditingHelper.AccessibleInJavascriptHashMap

class AccessibleInJavascriptHashMap extends [HashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/HashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.component.validation](ro/sync/ecss/component/validation/package-summary.md)

### Class ro.sync.ecss.component.validation.AuthorRangeRuler

class AuthorRangeRuler extends ro.sync.ui.ruler.RangeRulerBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### host

```
ro.sync.ecss.component.SwingAuthorHostComponent host
```

## Package [ro.sync.ecss.conditions](ro/sync/ecss/conditions/package-summary.md)

### Class ro.sync.ecss.conditions.AbstractSearchableTableModel

class AbstractSearchableTableModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ecss.conditions.ConditionPanel

class ConditionPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### changeValuesBgColor

```
Color changeValuesBgColor
```

##### collapsedProfilingAttributes

```
Set<String> collapsedProfilingAttributes
```

##### condition

```
ProfileConditionInfoPO condition
```

##### containsNewValues

```
boolean containsNewValues
```

##### ditavalStyleProvider

```
ro.sync.ecss.conditions.DITAVALStyleProvider ditavalStyleProvider
```

##### docTypeName

```
String docTypeName
```

##### fakeRadioButton

```
JRadioButton fakeRadioButton
```

##### filterText

```
String filterText
```

##### groupsButtons

```
Map<String,ro.sync.ecss.conditions.ConditionButtonsInfo> groupsButtons
```

##### keepCurrentValues

```
boolean keepCurrentValues
```

##### showProfilingStyles

```
boolean showProfilingStyles
```

### Class ro.sync.ecss.conditions.ConditionsPanel

class ConditionsPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### newValuesAreDisplayed

```
boolean newValuesAreDisplayed
```

##### panels

```
ArrayList<ro.sync.ecss.conditions.ConditionPanel> panels
```

### Class ro.sync.ecss.conditions.EditProfilingAttributesPanel

class EditProfilingAttributesPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### bgColor

```
Color bgColor
```

##### collapseAllAction

```
ro.sync.ui.application.action.TaggedAction collapseAllAction
```

##### conditionsPanel

```
ro.sync.ecss.conditions.ConditionsPanel conditionsPanel
```

##### conditionsPanelParent

```
JPanel conditionsPanelParent
```

##### conditionsProvider

```
ro.sync.ecss.conditions.ConditionsProvider conditionsProvider
```

##### expandAllAction

```
ro.sync.ui.application.action.TaggedAction expandAllAction
```

##### filterPanel

```
ro.sync.ui.FilterPanel filterPanel
```

##### firstComponentInWindow

```
boolean firstComponentInWindow
```

##### lastFilter

```
String lastFilter
```

##### noAttributesMessageArea

```
ro.sync.ui.application.ApplicationTextArea noAttributesMessageArea
```

##### notInConfigLabel

```
JLabel notInConfigLabel
```

##### notInConfigLabelParent

```
JPanel notInConfigLabelParent
```

##### recomputeConditions

```
boolean recomputeConditions
```

##### showProfilingStyles

```
boolean showProfilingStyles
```

### Class ro.sync.ecss.conditions.ProfileAppliedConditionSetPO

class ProfileAppliedConditionSetPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### conditionSetName

```
String conditionSetName
```

##### documentTypePattern

```
String documentTypePattern
```

### Class [ro.sync.ecss.conditions.ProfileConditionGroupPO](ro/sync/ecss/conditions/ProfileConditionGroupPO.md)

class ProfileConditionGroupPO extends [ProfileConditionValuePO](ro/sync/ecss/conditions/ProfileConditionValuePO.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### groupAttribute

```
String groupAttribute
```

The attribute of the group.

### Class [ro.sync.ecss.conditions.ProfileConditionInfoPO](ro/sync/ecss/conditions/ProfileConditionInfoPO.md)

class ProfileConditionInfoPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allowedValues

```
ProfileConditionValuePO[] allowedValues
```

Allowed values for this attribute.

##### allowsMultipleValues

```
boolean allowsMultipleValues
```

True if multiple values are allowed for this attribute

##### attributeName

```
String attributeName
```

Conditional attribute name.

##### attributeRenderName

```
String attributeRenderName
```

Attribute render name.

##### documentTypePattern

```
String documentTypePattern
```

Document type pattern. If specified, the condition will be used only for the document types that match it.

##### valuesSeparator

```
String valuesSeparator
```

Condition values separator. By default, is " "

### Class [ro.sync.ecss.conditions.ProfileConditionsSetInfoPO](ro/sync/ecss/conditions/ProfileConditionsSetInfoPO.md)

class ProfileConditionsSetInfoPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### conditions

```
ro.sync.options.SerializableLinkedHashMap<String,String[]> conditions
```

Map between attributes and profile values.

##### conditionSetName

```
String conditionSetName
```

Condition set name.

##### ditavalFile

```
String ditavalFile
```

The DITAVAL location used instead of the UI defined conditions.

##### documentTypePattern

```
String documentTypePattern
```

Document type pattern. If specified, the conditions set will be used only for the document types that match it.

##### shortcut

```
String shortcut
```

The condition set key stroke.

##### useDITAVAL

```
boolean useDITAVAL
```

true if the DITAVAL file should be used instead of condition set.

### Class [ro.sync.ecss.conditions.ProfileConditionValuePO](ro/sync/ecss/conditions/ProfileConditionValuePO.md)

class ProfileConditionValuePO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### description

```
String description
```

Condition attribute value description

##### level

```
int level
```

The level in the hierarchy of Subject Scheme values this condition is located on.

##### renderName

```
String renderName
```

The render name of the profiling condition value

##### value

```
String value
```

Condition attribute value

### Exception ro.sync.ecss.conditions.ProfileContentException

class ProfileContentException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### exceptionType

```
ro.sync.ecss.conditions.ProfileContentException.ProfileExceptionType exceptionType
```

### Class [ro.sync.ecss.conditions.ProfilingAttributesPresentingColorsPO](ro/sync/ecss/conditions/ProfilingAttributesPresentingColorsPO.md)

class ProfilingAttributesPresentingColorsPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### backgroundColor

```
int backgroundColor
```

The profiling background color.

##### borderColor

```
int borderColor
```

The color of the border that surrounds the profiled content.

##### nameForegroundColor

```
int nameForegroundColor
```

The foreground color for profiling attribute name.

##### valuesForegroundColor

```
int valuesForegroundColor
```

The foreground color for profiling attribute values.

### Class [ro.sync.ecss.conditions.ProfilingAttributeStylePO](ro/sync/ecss/conditions/ProfilingAttributeStylePO.md)

class ProfilingAttributeStylePO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### attributeGroupName

```
String attributeGroupName
```

The attribute group name.

##### attributeName

```
String attributeName
```

The attribute name.

##### attributeValue

```
String attributeValue
```

Condition attribute value

##### backgroundColor

```
int backgroundColor
```

The condition value background color. (Bits 24-31 are alpha, 16-23 are red, 8-15 are green, 0-7 are blue).

##### bold

```
boolean bold
```

true if the bold style should be applied on the content profiled by using this condition value.

##### docTypePattern

```
String docTypePattern
```

The document type pattern.

##### foregroundColor

```
int foregroundColor
```

The condition value foreground color. (Bits 24-31 are alpha, 16-23 are red, 8-15 are green, 0-7 are blue).

##### italic

```
boolean italic
```

true if the italic style should be applied on the content profiled by using this condition value.

##### textDecoration

```
String textDecoration
```

Text decoration to be applied on the content profiled by using this condition value. Example values: "underline", "overline", "double underline".

### Class ro.sync.ecss.conditions.SearchForMoreConditionSetsAction

class SearchForMoreConditionSetsAction extends ro.sync.ui.application.action.AccelActionProxy implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### conditionSets

```
List<ProfileConditionsSetInfoPO> conditionSets
```

##### manager

```
ro.sync.ecss.conditions.IConditionAttributesManager manager
```

## Package [ro.sync.ecss.css](ro/sync/ecss/css/package-summary.md)

### Exception ro.sync.ecss.css.InvalidPropertyValueException

class InvalidPropertyValueException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.ecss.css.UnsecureContextException

class UnsecureContextException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.css.functions](ro/sync/ecss/css/functions/package-summary.md)

### Exception ro.sync.ecss.css.functions.CannotEvaluateFunction

class CannotEvaluateFunction extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.ecss.css.functions.InvalidFunctionSignature

class InvalidFunctionSignature extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.ecss.css.functions.UnsecuredFunctionException

class UnsecuredFunctionException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### systemID

```
String systemID
```

## Package [ro.sync.ecss.dita.mapeditor.actions.export](ro/sync/ecss/dita/mapeditor/actions/export/package-summary.md)

### Class ro.sync.ecss.dita.mapeditor.actions.export.ExportDITAMapAction

class ExportDITAMapAction extends ro.sync.ecss.dita.mapeditor.actions.DITAMapAccelAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### mainFileOpener

```
ro.sync.exml.editor.EditorManager mainFileOpener
```

##### parentEditor

```
ro.sync.exml.editor.xmleditor.TransformationEditor parentEditor
```

##### progressTracker

```
ro.sync.io.ProgressTracker progressTracker
```

## Package [ro.sync.ecss.dom.builder](ro/sync/ecss/dom/builder/package-summary.md)

### Exception ro.sync.ecss.dom.builder.StylesheetException

class StylesheetException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.ecss.dom.builder.XMLSerializerException

class XMLSerializerException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions](ro/sync/ecss/extensions/package-summary.md)

### Class ro.sync.ecss.extensions.AuthorExtensionAction

class AuthorExtensionAction extends ro.sync.ui.application.action.TaggedAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### actionCore

```
ro.sync.ecss.extensions.AuthorExtensionActionCore actionCore
```

##### offset

```
int offset
```

### Class ro.sync.ecss.extensions.AuthorExtensionMenuButton

class AuthorExtensionMenuButton extends ro.sync.ui.ApplicationSplitButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### masterAction

```
ro.sync.ui.application.action.AbstractApplicationAction masterAction
```

## Package [ro.sync.ecss.extensions.api](ro/sync/ecss/extensions/api/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.AuthorOperationException](ro/sync/ecss/extensions/api/AuthorOperationException.md)

class AuthorOperationException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### operationRejectedOnPurpose

```
boolean operationRejectedOnPurpose
```

If true the operation was rejected and the shown error message should be more user-friendly.

### Exception [ro.sync.ecss.extensions.api.AuthorOperationStoppedByUserException](ro/sync/ecss/extensions/api/AuthorOperationStoppedByUserException.md)

class AuthorOperationStoppedByUserException extends [AuthorOperationException](ro/sync/ecss/extensions/api/AuthorOperationException.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.ecss.extensions.api.AuthorUndoManager](ro/sync/ecss/extensions/api/AuthorUndoManager.md)

class AuthorUndoManager extends [UndoManager](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/undo/UndoManager.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.ecss.extensions.api.CancelledByUserException](ro/sync/ecss/extensions/api/CancelledByUserException.md)

class CancelledByUserException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.ecss.extensions.api.CustomResolverException](ro/sync/ecss/extensions/api/CustomResolverException.md)

class CustomResolverException extends [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### errorResolver

```
ReferenceErrorResolver errorResolver
```

An error resolver.

### Exception ro.sync.ecss.extensions.api.ExtensionException

class ExtensionException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.ecss.extensions.api.InvalidEditException](ro/sync/ecss/extensions/api/InvalidEditException.md)

class InvalidEditException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### htmlMessage

```
String htmlMessage
```

HTML styled message.

##### presentToUser

```
boolean presentToUser
```

Indicates if the error message must be presented or not to the user.

##### showLinkToSchemaAwarePreferences

```
boolean showLinkToSchemaAwarePreferences
```

If true a link to the Schema aware preference page will be displayed with the error message.

##### title

```
String title
```

Title message.

### Exception ro.sync.ecss.extensions.api.InvalidXPathExtensionException

class InvalidXPathExtensionException extends ro.sync.ecss.extensions.api.ExtensionException implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### xpathExpression

```
String xpathExpression
```

### Exception [ro.sync.ecss.extensions.api.ReferenceResolverException](ro/sync/ecss/extensions/api/ReferenceResolverException.md)

class ReferenceResolverException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### errorResolver

```
ReferenceErrorResolver errorResolver
```

Offers to the user a possible solution for the error.

##### reportAsError

```
boolean reportAsError
```

true to report as error, false to report as warning.

##### shortMessage

```
String shortMessage
```

The short error message. Sometimes the message which will be presented first time to the user is shorter than the original message.

##### showInResultsPanel

```
boolean showInResultsPanel
```

true to also show the message in a results panel.

### Exception [ro.sync.ecss.extensions.api.ReferenceResolverSAXParseException](ro/sync/ecss/extensions/api/ReferenceResolverSAXParseException.md)

class ReferenceResolverSAXParseException extends [SAXParseException](https://docs.oracle.com/en/java/javase/17/docs/api/java.xml/org/xml/sax/SAXParseException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.ecss.extensions.api.ValidatingReferenceResolverException](ro/sync/ecss/extensions/api/ValidatingReferenceResolverException.md)

class ValidatingReferenceResolverException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### shortMessage

```
String shortMessage
```

The short error message. Sometimes the message which will be presented first time to the user is shorter than the original message.

### Class [ro.sync.ecss.extensions.api.WidthRepresentation](ro/sync/ecss/extensions/api/WidthRepresentation.md)

class WidthRepresentation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
  serialVersionUID: -7141751698158508637L
#### Serialized Fields

##### align

```
String align
```

The text align set in the width representation.

##### fixedWidthUnit

```
WidthRepresentation.Unit fixedWidthUnit
```

The fixed width unit.

##### fixedWidthValue

```
float fixedWidthValue
```

The fixed width value. For instance 2.5. In combination with the fixedWidthUnit represents a width.

##### isRelativeToParent

```
boolean isRelativeToParent
```

If true then the relativeWidth represents a percentage of the parent width, otherwise the relativeWidth will be computed taking into account the other siblings widths.

##### relativeWidthValue

```
float relativeWidthValue
```

The relative width. This value can be relative to the parent width, or relative to the other siblings. Ex: 3.2

## Package [ro.sync.ecss.extensions.api.component](ro/sync/ecss/extensions/api/component/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.component.AuthorComponentException](ro/sync/ecss/extensions/api/component/AuthorComponentException.md)

class AuthorComponentException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.api.link](ro/sync/ecss/extensions/api/link/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.link.CannotRecognizeIDException](ro/sync/ecss/extensions/api/link/CannotRecognizeIDException.md)

class CannotRecognizeIDException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.ecss.extensions.api.link.ElementLocatorException](ro/sync/ecss/extensions/api/link/ElementLocatorException.md)

class ElementLocatorException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.ecss.extensions.api.link.InvalidLinkException](ro/sync/ecss/extensions/api/link/InvalidLinkException.md)

class InvalidLinkException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### presentInplace

```
boolean presentInplace
```

true if the error message should be presented right in the document area, the same place where the link text should have been presented. false to report the error in the results area of the editor.

##### severity

```
Severity severity
```

A hint about the severity of the exception.

##### shortMessage

```
String shortMessage
```

Short message

## Package [ro.sync.ecss.extensions.api.table.operations](ro/sync/ecss/extensions/api/table/operations/package-summary.md)

### Class [ro.sync.ecss.extensions.api.table.operations.TableColumnSpecificationInformation](ro/sync/ecss/extensions/api/table/operations/TableColumnSpecificationInformation.md)

class TableColumnSpecificationInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
  serialVersionUID: 5273315963174368281L
#### Serialized Fields

##### widthRepresentation

```
WidthRepresentation widthRepresentation
```

The column width representation. Specifies the fixed and relative width determined from the column specification.

### Class [ro.sync.ecss.extensions.api.table.operations.TableRowsSpecificationInformation](ro/sync/ecss/extensions/api/table/operations/TableRowsSpecificationInformation.md)

class TableRowsSpecificationInformation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### sourceTableColumnsCount

```
int sourceTableColumnsCount
```

The number of columns from source table.

##### spanningCellIndexes

```
List<List<Integer>> spanningCellIndexes
```

The indexes of cells that spans over these rows

## Package [ro.sync.ecss.extensions.api.text](ro/sync/ecss/extensions/api/text/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.text.TextPageOperationException](ro/sync/ecss/extensions/api/text/TextPageOperationException.md)

class TextPageOperationException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### isError

```
boolean isError
```

true if the message of the exception is an error message.

## Package [ro.sync.ecss.extensions.api.webapp](ro/sync/ecss/extensions/api/webapp/package-summary.md)

## Package [ro.sync.ecss.extensions.api.webapp.access](ro/sync/ecss/extensions/api/webapp/access/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.webapp.access.EditingSessionOpenVetoException](ro/sync/ecss/extensions/api/webapp/access/EditingSessionOpenVetoException.md)

class EditingSessionOpenVetoException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### htmlMessage

```
String htmlMessage
```

The HTML message to be presented to the user.

## Package [ro.sync.ecss.extensions.api.webapp.cc](ro/sync/ecss/extensions/api/webapp/cc/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.webapp.cc.ItemNotFoundException](ro/sync/ecss/extensions/api/webapp/cc/ItemNotFoundException.md)

class ItemNotFoundException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.api.webapp.ce](ro/sync/ecss/extensions/api/webapp/ce/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.webapp.ce.RoomProxyCouldNotBeCreatedException](ro/sync/ecss/extensions/api/webapp/ce/RoomProxyCouldNotBeCreatedException.md)

class RoomProxyCouldNotBeCreatedException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### statusCode

```
int statusCode
```

The reason status code.

## Package [ro.sync.ecss.extensions.api.webapp.imagemap](ro/sync/ecss/extensions/api/webapp/imagemap/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.webapp.imagemap.ImageMapFormatException](ro/sync/ecss/extensions/api/webapp/imagemap/ImageMapFormatException.md)

class ImageMapFormatException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.api.webapp.license](ro/sync/ecss/extensions/api/webapp/license/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.webapp.license.UserNotLicensedException](ro/sync/ecss/extensions/api/webapp/license/UserNotLicensedException.md)

class UserNotLicensedException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.api.webapp.plugin](ro/sync/ecss/extensions/api/webapp/plugin/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.webapp.plugin.UserActionRequiredException](ro/sync/ecss/extensions/api/webapp/plugin/UserActionRequiredException.md)

class UserActionRequiredException extends [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### webappMessage

```
WebappMessage webappMessage
```

The webapp message.

## Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet](ro/sync/ecss/extensions/api/webapp/plugin/servlet/package-summary.md)

### Exception [ro.sync.ecss.extensions.api.webapp.plugin.servlet.ServletException](ro/sync/ecss/extensions/api/webapp/plugin/servlet/ServletException.md)

class ServletException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.commons](ro/sync/ecss/extensions/commons/package-summary.md)

### Exception [ro.sync.ecss.extensions.commons.CannotEditException](ro/sync/ecss/extensions/commons/CannotEditException.md)

class CannotEditException extends [CannotEditException](ro/sync/exml/workspace/api/images/handlers/CannotEditException.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.ecss.extensions.commons.PasteAsReferenceException](ro/sync/ecss/extensions/commons/PasteAsReferenceException.md)

class PasteAsReferenceException extends [AuthorOperationException](ro/sync/ecss/extensions/api/AuthorOperationException.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.commons.id](ro/sync/ecss/extensions/commons/id/package-summary.md)

### Class [ro.sync.ecss.extensions.commons.id.SAIDElementsCustomizerDialog](ro/sync/ecss/extensions/commons/id/SAIDElementsCustomizerDialog.md)

class SAIDElementsCustomizerDialog extends [OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### addButton

```
JButton addButton
```

The add button.

##### authorResourceBundle

```
AuthorResourceBundle authorResourceBundle
```

Author resource bundle.

##### autoAssignElementIDs

```
JCheckBox autoAssignElementIDs
```

Auto assign element IDs

##### editButton

```
JButton editButton
```

The edit button.

##### filterIDsOnCopy

```
JCheckBox filterIDsOnCopy
```

Filter IDs on copy

##### idGenerationPatternField

```
JTextField idGenerationPatternField
```

The id generation pattern field.

##### listMessage

```
String listMessage
```

The list message

##### listModel

```
DefaultListModel listModel
```

The list model.

##### listOfElements

```
JList listOfElements
```

The list of elements or class values for which to generate IDs

##### listPanel

```
JPanel listPanel
```

The panel holding the element list and the buttons.

##### removeButton

```
JButton removeButton
```

The remove button.

## Package [ro.sync.ecss.extensions.commons.sort](ro/sync/ecss/extensions/commons/sort/package-summary.md)

### Class [ro.sync.ecss.extensions.commons.sort.SASortCustomizerDialog](ro/sync/ecss/extensions/commons/sort/SASortCustomizerDialog.md)

class SASortCustomizerDialog extends [OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allElems

```
String allElems
```

The name of the "all elements" radio combo.

##### authorResourceBundle

```
AuthorResourceBundle authorResourceBundle
```

##### criteriaInformation

```
List<CriterionInformation> criteriaInformation
```

The all criteria information shown in the dialog.

##### firstCriterion

```
CriterionPanel firstCriterion
```

The panel for the first sorting criterion.

##### numberOfCriteria

```
int numberOfCriteria
```

The available number of criteria.

##### secondCriterion

```
CriterionPanel secondCriterion
```

The panel for the second sorting criterion.

##### selElems

```
String selElems
```

The name of the "selected elements" radio combo.

##### thirdCriterion

```
CriterionPanel thirdCriterion
```

The panel for the third sorting criterion.

## Package [ro.sync.ecss.extensions.commons.table.operations](ro/sync/ecss/extensions/commons/table/operations/package-summary.md)

### Class [ro.sync.ecss.extensions.commons.table.operations.SACustomTableColumnInsertionDialog](ro/sync/ecss/extensions/commons/table/operations/SACustomTableColumnInsertionDialog.md)

class SACustomTableColumnInsertionDialog extends [OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### afterRadioButton

```
JRadioButton afterRadioButton
```

"After" radio button. If selected, the column(s) will be inserted after the current location.

##### beforeRadioButton

```
JRadioButton beforeRadioButton
```

"Before" radio button. If selected, the column(s) will be inserted before the current location.

##### columnsSpinner

```
JSpinner columnsSpinner
```

Number of columns to be inserted.

### Class [ro.sync.ecss.extensions.commons.table.operations.SACustomTableRowInsertionDialog](ro/sync/ecss/extensions/commons/table/operations/SACustomTableRowInsertionDialog.md)

class SACustomTableRowInsertionDialog extends [OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### aboveRadioButton

```
JRadioButton aboveRadioButton
```

"Above" radio button. If selected, the row(s) will be inserted above the current location.

##### belowRadioButton

```
JRadioButton belowRadioButton
```

"Below" radio button. If selected, the row(s) will be inserted below the current location.

##### rowsSpinner

```
JSpinner rowsSpinner
```

Number of rows to be inserted.

### Class [ro.sync.ecss.extensions.commons.table.operations.SATableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableCustomizerDialog.md)

class SATableCustomizerDialog extends [OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### alignCombo

```
JComboBox alignCombo
```

Combo used to chose the table align value.

##### authorResourceBundle

```
AuthorResourceBundle authorResourceBundle
```

Author resource bundle.

##### calsModelRadio

```
JRadioButton calsModelRadio
```

Radio button used to choose CALS table model.

##### choiceTableModel

```
boolean choiceTableModel
```

true if the model is for choice table.

##### colsepCombo

```
JComboBox colsepCombo
```

Combo used to chose the table column separator value.

##### columnsSpinner

```
JSpinner columnsSpinner
```

Used to specify the number of columns.

##### colWidthsCombobox

```
JComboBox colWidthsCombobox
```

Used to specify how the column widths are generated. The column widths values can be fixed or proportional.

##### defaultColSpinnerModel

```
SpinnerModel defaultColSpinnerModel
```

The default table column spinner model.

##### footerCheckbox

```
JCheckBox footerCheckbox
```

If selected an empty table footer will be generated.

##### frameCombo

```
JComboBox frameCombo
```

Combo used to chose the table frame type.

##### hasAlignAttribute

```
boolean hasAlignAttribute
```

true if the table customized by this dialog has an align attribute.

##### hasColsepAttribute

```
boolean hasColsepAttribute
```

true if the table customized by this dialog has a column separator attribute.

##### hasFooter

```
boolean hasFooter
```

true if the table that is customized by this dialog has a footer.

##### hasFrameAttribute

```
boolean hasFrameAttribute
```

true if the table customized by this dialog has a frame attribute.

##### hasRowsepAttribute

```
boolean hasRowsepAttribute
```

true if the table customized by this dialog has a row separator attribute.

##### headerCheckbox

```
JCheckBox headerCheckbox
```

If selected an empty table header will be generated.

##### isCalsTable

```
boolean isCalsTable
```

true if the model is for CALS table.

##### isPropertiesTable

```
boolean isPropertiesTable
```

true if the model is for properties table.

##### isSimpleOrHtmlTable

```
boolean isSimpleOrHtmlTable
```

true if the model is for simple or HTML table, not CALS, nor properties.

##### isSimpleTableNotHtml

```
boolean isSimpleTableNotHtml
```

true if the table type is simple, not HTML.

##### predefinedColumnsCount

```
int predefinedColumnsCount
```

The predefined number of columns.

##### predefinedRowsCount

```
int predefinedRowsCount
```

The predefined number of rows.

##### propertiesModelRadio

```
JRadioButton propertiesModelRadio
```

Properties model.

##### propertiesTableColSpinnerModel

```
SpinnerModel propertiesTableColSpinnerModel
```

The model for the properties table column spinner.

##### rowsepCombo

```
JComboBox rowsepCombo
```

Combo used to chose the table row separator value.

##### rowsSpinner

```
JSpinner rowsSpinner
```

Used to specify the number of rows.

##### showModelChooser

```
boolean showModelChooser
```

If true the table model chooser will be shown. The table model can be CALS or HTML.

##### simpleOrHtmlModelRadio

```
JRadioButton simpleOrHtmlModelRadio
```

Either simple or HTML.

##### titleCheckbox

```
JCheckBox titleCheckbox
```

If selected the user can specify the table title.

##### titleTextField

```
JTextField titleTextField
```

Text field for specify the table title.

### Class [ro.sync.ecss.extensions.commons.table.operations.SATableSplitCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableSplitCustomizerDialog.md)

class SATableSplitCustomizerDialog extends [OKCancelDialog](ro/sync/exml/workspace/api/standalone/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### colsSpinner

```
JSpinner colsSpinner
```

Columns number chooser.

##### rowsSpinner

```
JSpinner rowsSpinner
```

Rows number chooser.

### Class [ro.sync.ecss.extensions.commons.table.operations.TableInfo](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md)

class TableInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
  serialVersionUID: 616939850L
#### Serialized Fields

##### align

```
String align
```

Alignment value.

##### colsep

```
String colsep
```

Column separator value.

##### columnsNumber

```
int columnsNumber
```

Number of cols

##### columnsWidthsType

```
TableCustomizerConstants.ColumnWidthsType columnsWidthsType
```

The column widths type.

##### frame

```
String frame
```

Frame value.

##### generateFooter

```
boolean generateFooter
```

true if should generate footer.

##### generateHeader

```
boolean generateHeader
```

true if should generate header.

##### rowsep

```
String rowsep
```

Row separator value.

##### rowsNumber

```
int rowsNumber
```

Number of rows

##### tableModel

```
int tableModel
```

The table model. One of the constants: [TableInfo.TABLE_MODEL_CALS](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md#TABLE_MODEL_CALS), [TableInfo.TABLE_MODEL_CUSTOM](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md#TABLE_MODEL_CUSTOM), [TableInfo.TABLE_MODEL_DITA_SIMPLE](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md#TABLE_MODEL_DITA_SIMPLE), [TableInfo.TABLE_MODEL_HTML](ro/sync/ecss/extensions/commons/table/operations/TableInfo.md#TABLE_MODEL_HTML).

##### title

```
String title
```

The title

## Package [ro.sync.ecss.extensions.commons.table.operations.cals](ro/sync/ecss/extensions/commons/table/operations/cals/package-summary.md)

### Class [ro.sync.ecss.extensions.commons.table.operations.cals.CALSTableColumnSpecificationInformation](ro/sync/ecss/extensions/commons/table/operations/cals/CALSTableColumnSpecificationInformation.md)

class CALSTableColumnSpecificationInformation extends [TableColumnSpecificationInformation](ro/sync/ecss/extensions/api/table/operations/TableColumnSpecificationInformation.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)
  serialVersionUID: 8593660063150563179L
#### Serialized Fields

##### columnName

```
String columnName
```

The name of the column.

## Package [ro.sync.ecss.extensions.commons.table.operations.xhtml](ro/sync/ecss/extensions/commons/table/operations/xhtml/package-summary.md)

### Class [ro.sync.ecss.extensions.commons.table.operations.xhtml.SAXHTMLTableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/xhtml/SAXHTMLTableCustomizerDialog.md)

class SAXHTMLTableCustomizerDialog extends [SATableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableCustomizerDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.commons.table.properties](ro/sync/ecss/extensions/commons/table/properties/package-summary.md)

### Class [ro.sync.ecss.extensions.commons.table.properties.SATablePropertiesCustomizerDialog](ro/sync/ecss/extensions/commons/table/properties/SATablePropertiesCustomizerDialog.md)

class SATablePropertiesCustomizerDialog extends [OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### authorResourceBundle

```
AuthorResourceBundle authorResourceBundle
```

The author resource bundle.

##### colorThemeUtilities

```
ColorThemeUtilities colorThemeUtilities
```

The color theme utilities.

## Package [ro.sync.ecss.extensions.commons.ui](ro/sync/ecss/extensions/commons/ui/package-summary.md)

### Class [ro.sync.ecss.extensions.commons.ui.OKCancelDialog](ro/sync/ecss/extensions/commons/ui/OKCancelDialog.md)

class OKCancelDialog extends [OKCancelDialog](ro/sync/exml/workspace/api/standalone/ui/OKCancelDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.dita.map.table](ro/sync/ecss/extensions/dita/map/table/package-summary.md)

### Class [ro.sync.ecss.extensions.dita.map.table.SADITARelTableCustomizerDialog](ro/sync/ecss/extensions/dita/map/table/SADITARelTableCustomizerDialog.md)

class SADITARelTableCustomizerDialog extends [SATableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableCustomizerDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.dita.topic.table](ro/sync/ecss/extensions/dita/topic/table/package-summary.md)

### Class [ro.sync.ecss.extensions.dita.topic.table.SADITATableCustomizerDialog](ro/sync/ecss/extensions/dita/topic/table/SADITATableCustomizerDialog.md)

class SADITATableCustomizerDialog extends [SATableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableCustomizerDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.docbook.table](ro/sync/ecss/extensions/docbook/table/package-summary.md)

### Class [ro.sync.ecss.extensions.docbook.table.SADocbook4TableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbook4TableCustomizerDialog.md)

class SADocbook4TableCustomizerDialog extends [SADocbookTableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbookTableCustomizerDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.ecss.extensions.docbook.table.SADocbook5TableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbook5TableCustomizerDialog.md)

class SADocbook5TableCustomizerDialog extends [SADocbookTableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbookTableCustomizerDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.ecss.extensions.docbook.table.SADocbookTableCustomizerDialog](ro/sync/ecss/extensions/docbook/table/SADocbookTableCustomizerDialog.md)

class SADocbookTableCustomizerDialog extends [SATableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableCustomizerDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.extensions.tei.table](ro/sync/ecss/extensions/tei/table/package-summary.md)

### Class [ro.sync.ecss.extensions.tei.table.SATEITableCustomizerDialog](ro/sync/ecss/extensions/tei/table/SATEITableCustomizerDialog.md)

class SATEITableCustomizerDialog extends [SATableCustomizerDialog](ro/sync/ecss/extensions/commons/table/operations/SATableCustomizerDialog.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.imagemap](ro/sync/ecss/imagemap/package-summary.md)

### Exception [ro.sync.ecss.imagemap.ImageMapNotSuportedException](ro/sync/ecss/imagemap/ImageMapNotSuportedException.md)

class ImageMapNotSuportedException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.ecss.imagemap.IncompleteAreaException

class IncompleteAreaException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.ecss.webapp](ro/sync/ecss/webapp/package-summary.md)

### Class ro.sync.ecss.webapp.AuthorDocumentModelImpl

class AuthorDocumentModelImpl extends ro.sync.ecss.webapp.BaseAuthorDocumentModel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.ecss.webapp.AuthorModelInitializationException

class AuthorModelInitializationException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ecss.webapp.BaseAuthorDocumentModel

class BaseAuthorDocumentModel extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialization Methods

##### readObject

private void readObject([ObjectInputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/ObjectInputStream.html) arg0)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), [ClassNotFoundException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassNotFoundException.html)
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) [ClassNotFoundException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassNotFoundException.html)
##### readObjectNoData

private void readObjectNoData() throws [ObjectStreamException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/ObjectStreamException.html)
  Throws: [ObjectStreamException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/ObjectStreamException.html)
##### writeObject

private void writeObject([ObjectOutputStream](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/ObjectOutputStream.html) arg0)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
  Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

#### Serialized Fields

##### actionsManager

```
WebappActionsManager actionsManager
```

##### actionsSupport

```
ro.sync.ecss.webapp.WebappAuthorSchemaAwareActionsSupport actionsSupport
```

##### attributesFilter

```
ro.sync.ecss.component.filter.CompoundAuthorAttributesDisplayFilter attributesFilter
```

##### authorAccess

```
AuthorAccess authorAccess
```

##### authorDocumentController

```
ro.sync.ecss.ue.AuthorDocumentControllerImpl authorDocumentController
```

##### ccManager

```
ContentCompletionManager ccManager
```

##### cmsUserId

```
String cmsUserId
```

##### contentType

```
String contentType
```

##### docTypeProvider

```
ro.sync.exml.editor.xmleditor.DocumentTypeProvider docTypeProvider
```

##### documentId

```
String documentId
```

##### editingHelper

```
ro.sync.ecss.webapp.formcontrols.WebappInplaceEditingHelper editingHelper
```

##### findReplaceSupport

```
ro.sync.ecss.webapp.findreplace.FindReplaceSupportImpl findReplaceSupport
```

##### imposedCompactTagsMode

```
Boolean imposedCompactTagsMode
```

##### indentOptions

```
ro.sync.exml.editor.prettyprint.IndentOptions indentOptions
```

##### indexer

```
ro.sync.ecss.webapp.AuthorIdIndexImpl<AuthorNode> indexer
```

##### licenseeId

```
String licenseeId
```

##### lockManager

```
ro.sync.ecss.webapp.WebappLockManagerImpl lockManager
```

##### markersIndexer

```
ro.sync.ecss.webapp.AuthorIdIndexImpl<AuthorPersistentHighlight> markersIndexer
```

##### messageReporter

```
ro.sync.ecss.webapp.WebappMessageReporter messageReporter
```

##### reviewController

```
ReviewController reviewController
```

##### selectionModel

```
AuthorSelectionAndCaretModel selectionModel
```

##### sessionTracker

```
ro.sync.ecss.webapp.license.SessionTracker sessionTracker
```

##### spellchecker

```
ro.sync.ecss.webapp.WebappSpellcheckerImpl spellchecker
```

##### validationAssistant

```
ro.sync.ecss.webapp.validate.WebappValidationAssistant validationAssistant
```

## Package [ro.sync.ecss.webapp.ditamap](ro/sync/ecss/webapp/ditamap/package-summary.md)

### Class ro.sync.ecss.webapp.ditamap.DITAMapDocumentModelImpl

class DITAMapDocumentModelImpl extends ro.sync.ecss.webapp.BaseAuthorDocumentModel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.exml](ro/sync/exml/package-summary.md)

### Class ro.sync.exml.ActionLinkLabel

class ActionLinkLabel extends ro.sync.exml.LinkLabel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### action

```
Action action
```

### Class ro.sync.exml.ContentTypePageAssociationPO

class ContentTypePageAssociationPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### contentType

```
String contentType
```

##### pageID

```
String pageID
```

### Class ro.sync.exml.FileHistory

class FileHistory extends ro.sync.ui.application.menu.ApplicationMenu implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### historyFile

```
File historyFile
```

##### historyList

```
List historyList
```

##### historyUpdateListeners

```
List<ro.sync.exml.FileHistory.FileHistoryUpdater> historyUpdateListeners
```

##### opener

```
ro.sync.exml.editor.role.FileOpener opener
```

##### shouldPresentIcons

```
boolean shouldPresentIcons
```

### Class ro.sync.exml.FileHistory.HistoryAction

class HistoryAction extends ro.sync.ui.application.action.ThreadAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### url

```
URL url
```

### Class ro.sync.exml.FocusableLabel

class FocusableLabel extends [JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.exml.LicenseNotFoundException

class LicenseNotFoundException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.LinkLabel

class LinkLabel extends ro.sync.exml.FocusableLabel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### UNDERLINED_TEXT_ATTRIBUTES_MAP

```
Map<? extends AttributedCharacterIterator.Attribute,?> UNDERLINED_TEXT_ATTRIBUTES_MAP
```

##### underlineFont

```
Font underlineFont
```

### Class ro.sync.exml.MainFrame

class MainFrame extends ro.sync.ui.application.ApplicationMainFrame implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### actionsProvider

```
ro.sync.exml.editor.CommonSAActionsProvider actionsProvider
```

##### applicationCloseListeners

```
List applicationCloseListeners
```

##### batchFormatAndIndentControl

```
ro.sync.exml.editor.pagetext.formatandindent.SABatchFormatAndIndentControl batchFormatAndIndentControl
```

##### cgmSupportOffered

```
boolean cgmSupportOffered
```

##### cmdLineEffectorMenu

```
ro.sync.exml.cmdbuttons.CmdMenu cmdLineEffectorMenu
```

##### cmdLineEffectorMenuButton

```
ro.sync.exml.cmdbuttons.CmdMenuButton cmdLineEffectorMenuButton
```

##### comparisonsOptionListeners

```
ro.sync.exml.OptionListeners comparisonsOptionListeners
```

##### component

```
ro.sync.exml.docking.OxygenContentContainer component
```

##### componentsMap

```
ro.sync.exml.componentinfo.ComponentsMap componentsMap
```

##### ctrlPressed

```
boolean ctrlPressed
```

##### dbResourcesProvider

```
ro.sync.exml.editor.helpers.DBExplorerPanel dbResourcesProvider
```

##### debuggerComponents

```
ro.sync.dxsl.DebuggerComponents debuggerComponents
```

##### debugMenu

```
ro.sync.ui.application.menu.ApplicationMenu debugMenu
```

##### delayedShutDownThread

```
ro.sync.ui.application.ApplicationThread delayedShutDownThread
```

##### ditaMapEdManager

```
ro.sync.ecss.dita.mapeditor.DITAMapsEditorManagerImpl ditaMapEdManager
```

##### ditaMapsMainPanel

```
ro.sync.ecss.dita.mapeditor.DITAMapMainPanel ditaMapsMainPanel
```

##### ditaReusableComponentsManager

```
ro.sync.ecss.dita.reference.DITAReusableComponentsViewPanel ditaReusableComponentsManager
```

##### editControl

```
ro.sync.exml.controllers.EditControl editControl
```

##### editorManager

```
ro.sync.exml.editor.DebuggerEditorManager editorManager
```

##### extensionMenu

```
ro.sync.ui.application.menu.ApplicationMenu extensionMenu
```

##### fileControl

```
ro.sync.exml.controllers.FileControl fileControl
```

##### fileExitAction

```
ro.sync.ui.application.action.AccelAction fileExitAction
```

##### firstShow

```
boolean firstShow
```

##### fixedTitle

```
String fixedTitle
```

##### helpControl

```
ro.sync.exml.controllers.HelpControl helpControl
```

##### historyControl

```
ro.sync.exml.controllers.HistoryControl historyControl
```

##### ideAccess

```
ro.sync.exml.SAIDEAccess ideAccess
```

##### ignoreLayoutOptionsChanges

```
boolean ignoreLayoutOptionsChanges
```

##### layoutChangingOptionsLastState

```
ro.sync.exml.LayoutChangingOptionsState layoutChangingOptionsLastState
```

##### layoutManager

```
ro.sync.exml.layout.MainFrameLayoutManager layoutManager
```

##### menuBar

```
ro.sync.ui.application.menu.ApplicationMenu[] menuBar
```

##### notAllowedComponents

```
Set<String> notAllowedComponents
```

##### onTopFramesRepository

```
ro.sync.exml.OnTopDockableFramesRepository onTopFramesRepository
```

##### optionsControl

```
ro.sync.exml.controllers.OptionsControl optionsControl
```

##### optionsForwarder

```
ro.sync.exml.editor.OptionsForwarderInterface optionsForwarder
```

##### perspectiveManager

```
ro.sync.exml.MainFramePerspectiveManager perspectiveManager
```

##### pluggableMenu

```
ro.sync.exml.editor.PluggableMenu pluggableMenu
```

##### projectManager

```
ro.sync.exml.project.ProjectManager projectManager
```

##### projectURL

```
URL projectURL
```

##### properlyInitialized

```
boolean properlyInitialized
```

##### pwa

```
StandalonePluginWorkspace pwa
```

##### quickFindAction

```
ro.sync.ui.application.action.AccelAction quickFindAction
```

##### resultsPanel

```
ro.sync.exml.editor.results.ResultsManagerPanel resultsPanel
```

##### saveAndLoadLayoutInhibited

```
boolean saveAndLoadLayoutInhibited
```

##### searchControl

```
ro.sync.exml.controllers.SearchControlImpl searchControl
```

##### skipToggleMaximizedEditor

```
boolean skipToggleMaximizedEditor
```

##### spellControl

```
ro.sync.azcheck.ui.files.SpellCheckControlImpl spellControl
```

##### titleUpdater

```
ro.sync.exml.TitleUpdater titleUpdater
```

##### toolsControl

```
ro.sync.exml.controllers.ToolsControl toolsControl
```

##### validator

```
ComponentsValidator validator
```

##### windowMenuControl

```
ro.sync.exml.editor.WindowActionsControl windowMenuControl
```

##### workspaceController

```
ro.sync.exml.project.WorkspaceController workspaceController
```

### Class ro.sync.exml.NextEditorAction

class NextEditorAction extends ro.sync.ui.application.action.AccelAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### switchDialog

```
ro.sync.exml.TabsSwitchDialog switchDialog
```

### Class ro.sync.exml.OnTopFramesPO

class OnTopFramesPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### onTopFrames

```
ro.sync.options.SerializableLinkedHashMap<ro.sync.exml.ContentTypePageAssociationPO,ro.sync.options.SerializableList<String>> onTopFrames
```

### Class ro.sync.exml.PreviousEditorAction

class PreviousEditorAction extends ro.sync.ui.application.action.AccelAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### switchDialog

```
ro.sync.exml.TabsSwitchDialog switchDialog
```

### Class ro.sync.exml.ShowDockableFrameAction

class ShowDockableFrameAction extends ro.sync.ui.application.action.AccelAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### componentProvider

```
ro.sync.exml.DockableFrameComponentProvider componentProvider
```

##### dockingManager

```
ro.sync.exml.docking.OxygenDockingManager dockingManager
```

##### frameKey

```
String frameKey
```

### Class ro.sync.exml.ShowDockableFrameFromAddOnAction

class ShowDockableFrameFromAddOnAction extends ro.sync.exml.ShowDockableFrameAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### addonID

```
String addonID
```

##### addonName

```
String addonName
```

##### viewID

```
String viewID
```

##### viewName

```
String viewName
```

##### viewsManager

```
ro.sync.exml.docking.IViewsManager viewsManager
```

### Class ro.sync.exml.Splash

class Splash extends [JFrame](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JFrame.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### dekoy

```
JDialog dekoy
```

##### editionDlgOverNative

```
JDialog editionDlgOverNative
```

##### editionIcon

```
Icon editionIcon
```

##### editionP

```
Point editionP
```

##### enableEditionDisplay

```
boolean enableEditionDisplay
```

##### imageIcon

```
ImageIcon imageIcon
```

##### isInhibited

```
boolean isInhibited
```

##### loadingProgress

```
ro.sync.exml.Splash.LoadingProgress loadingProgress
```

##### splashBounds

```
Rectangle splashBounds
```

### Exception ro.sync.exml.WrongXercesVersionException

class WrongXercesVersionException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### currentVersion

```
String currentVersion
```

##### expectedVersion

```
String expectedVersion
```

##### location

```
URL location
```

## Package [ro.sync.exml.editor](ro/sync/exml/editor/package-summary.md)

### Class ro.sync.exml.editor.AbstractEditor

class AbstractEditor extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### availablePages

```
String[] availablePages
```

##### breakPointCreator

```
ro.sync.ui.marks.BreakPointsManager breakPointCreator
```

##### buttonsBar

```
JPanel buttonsBar
```

##### canEditReadOnly

```
boolean canEditReadOnly
```

##### clearUndoBufferOnSave

```
boolean clearUndoBufferOnSave
```

##### closeAction

```
ro.sync.exml.editor.actions.CloseAction closeAction
```

##### contentType

```
String contentType
```

##### currentPageID

```
String currentPageID
```

##### customOxygenQueryParams

```
Map<String,String> customOxygenQueryParams
```

##### documentMenuActions

```
List documentMenuActions
```

##### documentTypePage

```
String documentTypePage
```

##### editorActions

```
List<ro.sync.ui.application.action.AccelAction> editorActions
```

##### editorIcon

```
Icon editorIcon
```

##### editorListener

```
ro.sync.exml.editor.CurrentEditorListener editorListener
```

##### editorListeners

```
List<ro.sync.exml.editor.BasicEditorListener> editorListeners
```

##### editorManager

```
ro.sync.exml.editor.EditorManager editorManager
```

##### editorManagerListener

```
ro.sync.exml.editor.AbstractEditor.EditorManagerListenerImpl editorManagerListener
```

##### editorPages

```
List<ro.sync.exml.editor.EditorPage> editorPages
```

##### enableSetBoundsInEditor

```
boolean enableSetBoundsInEditor
```

##### encodingDetectedOnOpen

```
String encodingDetectedOnOpen
```

##### fileChangeWatcher

```
ro.sync.exml.watcher.FileChangeWatcher fileChangeWatcher
```

##### fileHistory

```
ro.sync.exml.FileHistory fileHistory
```

##### filePrintAction

```
ro.sync.ui.application.action.AccelAction filePrintAction
```

##### filePrintPreviewAction

```
ro.sync.ui.application.action.AccelAction filePrintPreviewAction
```

##### firstRead

```
boolean firstRead
```

##### fixedTabTitle

```
String fixedTabTitle
```

##### fixedTooltip

```
String fixedTooltip
```

##### ideAccess

```
ro.sync.exml.IDEAccess ideAccess
```

##### infoPanel

```
ro.sync.exml.editor.infopanel.EditorInfoPanel infoPanel
```

##### initialized

```
boolean initialized
```

##### isCurrentSelected

```
boolean isCurrentSelected
```

##### isEditableViaAPI

```
boolean isEditableViaAPI
```

##### isEditorClosed

```
boolean isEditorClosed
```

##### largeDocumentMode

```
ro.sync.exml.editor.FileSizeHint largeDocumentMode
```

##### lastEditorBoundsNotProcessed

```
Rectangle lastEditorBoundsNotProcessed
```

##### location

```
URL location
```

##### longLineDocument

```
boolean longLineDocument
```

##### markCreatorAnyName

```
ro.sync.ui.marks.MarkCreatorAnyName markCreatorAnyName
```

##### operationInProgress

```
ro.sync.basic.util.concurrent.Semaphore operationInProgress
```

##### pageButtonGroup

```
ButtonGroup pageButtonGroup
```

##### pageCardLayout

```
CardLayout pageCardLayout
```

##### pageCardLayoutPanel

```
JPanel pageCardLayoutPanel
```

##### pageChangeToolbar

```
ro.sync.ui.toolbar.ToolBar pageChangeToolbar
```

##### parentFrame

```
Frame parentFrame
```

##### persistenceManager

```
ro.sync.exml.editor.PersistenceManager persistenceManager
```

##### pluggableMenuItemsMap

```
Map<String,List> pluggableMenuItemsMap
```

##### reloadAction

```
ro.sync.ui.application.action.AccelAction reloadAction
```

##### reviewDocumentsNavigatorProvider

```
ro.sync.ecss.component.ui.review.navigation.ReviewDocumentsNavigatorProvider reviewDocumentsNavigatorProvider
```

##### saveAction

```
ro.sync.ui.application.action.AccelAction saveAction
```

##### saveCount

```
int saveCount
```

##### savedAdditionalURLsToCheck

```
Map<ro.sync.exml.editor.EditorPage,Map<String,Long>> savedAdditionalURLsToCheck
```

##### statusModel

```
ro.sync.exml.editor.status.StatusModel statusModel
```

##### switchPageProgressStarter

```
ro.sync.io.ProgressTrackerStarter switchPageProgressStarter
```

##### title

```
String title
```

##### undoableEditListeners

```
List undoableEditListeners
```

##### viewInBrowserSystemAppAction

```
ro.sync.ui.application.action.AccelAction viewInBrowserSystemAppAction
```

### Class ro.sync.exml.editor.AbstractEditorPage

class AbstractEditorPage extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### additionalDockableViewers

```
ro.sync.exml.editor.AdditionalDockableViewer[] additionalDockableViewers
```

##### allActions

```
List<ro.sync.ui.application.action.AccelAction> allActions
```

##### bookmarksMap

```
Map<String,ro.sync.exml.editor.projecteditingstate.MarkLocation> bookmarksMap
```

##### contentOfPageChanged

```
boolean contentOfPageChanged
```

##### contentOfPageLoadAlreadyCalled

```
boolean contentOfPageLoadAlreadyCalled
```

##### editorIsLoading

```
boolean editorIsLoading
```

##### isReverting

```
boolean isReverting
```

##### listeners

```
List listeners
```

##### mustReload

```
boolean mustReload
```

##### pageComponentsInitialized

```
boolean pageComponentsInitialized
```

##### pageInitialized

```
boolean pageInitialized
```

##### parentEditor

```
ro.sync.exml.editor.Editor parentEditor
```

##### wasLoaded

```
boolean wasLoaded
```

### Class ro.sync.exml.editor.AdditionalDockableViewerContainer

class AdditionalDockableViewerContainer extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### componentVisible

```
boolean componentVisible
```

##### editorManager

```
ro.sync.exml.editor.EditorManager editorManager
```

##### enableViewUpdate

```
boolean enableViewUpdate
```

##### incompatibleEditorWarn

```
String incompatibleEditorWarn
```

##### mainFrameInitialized

```
boolean mainFrameInitialized
```

##### noEditorSelectedWarn

```
JComponent noEditorSelectedWarn
```

##### viewID

```
int viewID
```

##### warningsArea

```
ro.sync.ui.application.ApplicationTextArea warningsArea
```

### Class ro.sync.exml.editor.DebuggerContainerImpl

class DebuggerContainerImpl extends ro.sync.exml.editor.EditorContainerImpl implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### horizontalLayout

```
boolean horizontalLayout
```

### Class ro.sync.exml.editor.DefaultAnchor

class DefaultAnchor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### nonWhitespaceAnchor

```
boolean nonWhitespaceAnchor
```

##### offset

```
int offset
```

### Class ro.sync.exml.editor.EditorContainerImpl

class EditorContainerImpl extends ro.sync.exml.docking.OxygenContentContainer implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### dockingManager

```
ro.sync.exml.docking.OxygenDockingManager dockingManager
```

##### editorsLayoutFile

```
File editorsLayoutFile
```

##### layoutFilePrefix

```
String layoutFilePrefix
```

##### middleClickCustomizer

```
ro.sync.exml.editor.EditorContainerImpl.OxygenTabbedPaneCustomizer middleClickCustomizer
```

##### showEditorTabs

```
boolean showEditorTabs
```

### Class ro.sync.exml.editor.EditorDockableFrame

class EditorDockableFrame extends ro.sync.exml.docking.ApplicationDockableFrame implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### hpProvider

```
HelpPageProvider hpProvider
```

### Class ro.sync.exml.editor.EditorPageAssociation

class EditorPageAssociation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### contentType

```
String contentType
```

##### editorPage

```
String editorPage
```

### Exception ro.sync.exml.editor.ElementIteratorException

class ElementIteratorException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.exml.editor.ErrorsCheckException

class ErrorsCheckException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.exml.editor.FileCannotBeOpenedInReviewerException](ro/sync/exml/editor/FileCannotBeOpenedInReviewerException.md)

class FileCannotBeOpenedInReviewerException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.editor.FileTypeAssociation

class FileTypeAssociation extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### contentType

```
String contentType
```

##### defaultExtension

```
boolean defaultExtension
```

##### extension

```
String extension
```

### Exception ro.sync.exml.editor.FloatingLicenseViolationException

class FloatingLicenseViolationException extends [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.exml.editor.InvalidPageContentException

class InvalidPageContentException extends [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.editor.LineAnchor

class LineAnchor extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### column

```
int column
```

##### line

```
int line
```

### Class ro.sync.exml.editor.OxygenToggleButtonBorder

class OxygenToggleButtonBorder extends [LineBorder](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/border/LineBorder.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### segmentPosition

```
String segmentPosition
```

### Class ro.sync.exml.editor.PageToggleButton

class PageToggleButton extends ro.sync.ui.application.ApplicationToggleButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### pageID

```
String pageID
```

##### skipFireButtonClicked

```
boolean skipFireButtonClicked
```

##### skipFirePageChange

```
boolean skipFirePageChange
```

### Class ro.sync.exml.editor.PlaceHolderEditor

class PlaceHolderEditor extends ro.sync.exml.editor.AbstractEditor implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### extension

```
String extension
```

##### openedFileInfo

```
ro.sync.exml.editor.projecteditingstate.OpenedFileInfo openedFileInfo
```

### Class ro.sync.exml.editor.PluggableMenu

class PluggableMenu extends ro.sync.exml.editor.PluggableMenuBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.editor.PluggableMenuBase

class PluggableMenuBase extends ro.sync.ui.application.menu.ApplicationMenu implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### editorManager

```
ro.sync.exml.editor.EditorManager editorManager
```

##### selectedEditorURL

```
URL selectedEditorURL
```

### Class ro.sync.exml.editor.SortableTabbedPane

class SortableTabbedPane extends [JTabbedPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTabbedPane.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.editor.TextPageAction

class TextPageAction extends ro.sync.ui.application.action.AccelAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### textPage

```
ro.sync.exml.editor.pagetext.TextPage textPage
```

### Class ro.sync.exml.editor.TextPageWithBracketAnchor

class TextPageWithBracketAnchor extends ro.sync.exml.editor.validate.ValidationTextPage implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.exml.editor.UnsupportedInCurrentContextException

class UnsupportedInCurrentContextException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.editor.UserPreferredURLs

class UserPreferredURLs extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### keys

```
ro.sync.options.SerializableList keys
```

##### urlLists

```
ro.sync.options.SerializableList urlLists
```

### Class ro.sync.exml.editor.XsltXQueryInputPanel

class XsltXQueryInputPanel extends ro.sync.ui.application.ApplicationScrollPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### componentIsVisible

```
boolean componentIsVisible
```

##### emptyModelWarn

```
ro.sync.ui.application.ApplicationTextArea emptyModelWarn
```

##### instanceChanged

```
boolean instanceChanged
```

##### isXSLT

```
boolean isXSLT
```

##### lastInstanceChangeEvent

```
ro.sync.ui.tree.DocumentAndLocation[] lastInstanceChangeEvent
```

##### model

```
ro.sync.ui.tree.MultipleDocumentsXmlTreeModel model
```

##### proposalListener

```
ro.sync.exml.editor.proposal.ProposalSelectionListener proposalListener
```

##### proposalMenu

```
ro.sync.exml.editor.proposal.ProposalsMenu proposalMenu
```

##### textPage

```
ro.sync.exml.editor.pagetext.TextPage textPage
```

##### tree

```
ro.sync.ui.dnd.tree.DnDTree tree
```

## Package [ro.sync.exml.editor.xmleditor.pageauthor](ro/sync/exml/editor/xmleditor/pageauthor/package-summary.md)

### Class ro.sync.exml.editor.xmleditor.pageauthor.AuthorCSSHistoryPO

class AuthorCSSHistoryPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### map

```
ro.sync.options.SerializableLinkedHashMap<String,String> map
```

### Class ro.sync.exml.editor.xmleditor.pageauthor.AuthorEditorPage

class AuthorEditorPage extends ro.sync.exml.editor.AbstractEditorPage implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### actionsManager

```
ro.sync.ecss.component.ui.actions.TaglessActionsManager actionsManager
```

##### actionsProvider

```
ro.sync.exml.editor.xmleditor.pageauthor.SAAuthorActionsProvider actionsProvider
```

##### additionalAuthorReviewPanel

```
ro.sync.ecss.component.ui.review.AuthorReviewPanel additionalAuthorReviewPanel
```

##### applyDefaultQFsAction

```
ro.sync.exml.editor.actions.ApplyAllDefaultQuickFixesAction applyDefaultQFsAction
```

##### attributesDisplayFilter

```
ro.sync.ecss.component.filter.CompoundAuthorAttributesDisplayFilter attributesDisplayFilter
```

##### attributesPanel

```
ro.sync.ecss.component.ui.context.attributes.AttributesPanel attributesPanel
```

##### authorAccess

```
AuthorAccess authorAccess
```

##### authorDocumentListener

```
ro.sync.ecss.dom.AuthorDocumentListenerExt authorDocumentListener
```

##### authorExtensionBuilder

```
ro.sync.ecss.extensions.AuthorExtensionBuilder authorExtensionBuilder
```

##### authorExtensionsBundle

```
ExtensionsBundle authorExtensionsBundle
```

##### authorPageAccess

```
WSAuthorEditorPage authorPageAccess
```

##### authorPersistentHighlightsListener

```
AuthorPersistentHighlightsListener authorPersistentHighlightsListener
```

##### authorReferenceNodeExtensionBuilderProvider

```
ro.sync.ecss.extensions.AuthorExtensionBuilderProvider authorReferenceNodeExtensionBuilderProvider
```

##### authorReviewPanel

```
ro.sync.ecss.component.ui.review.AuthorReviewPanel authorReviewPanel
```

##### breadcrumbAndDITAPositionPanel

```
JPanel breadcrumbAndDITAPositionPanel
```

##### breadCrumbPanel

```
ro.sync.ecss.component.ui.status.AuthorCurrentXpathPanel breadCrumbPanel
```

##### caretListeners

```
List caretListeners
```

##### codeTemplatesHelper

```
ro.sync.contentcompletion.CTAcceleratorsHelper codeTemplatesHelper
```

##### conrefResolverListener

```
ro.sync.ecss.component.AuthorConrefResolverListener conrefResolverListener
```

##### cssMenuButton

```
ro.sync.exml.editor.xmleditor.pageauthor.CSSMenuButton cssMenuButton
```

##### dnDHandlerWrapper

```
ro.sync.exml.editor.xmleditor.pageauthor.AuthorDnDHandlerWrapper dnDHandlerWrapper
```

##### documentTypeChecker

```
ro.sync.ecss.contentcompletion.AuthorDocumentTypeChangeChecker documentTypeChecker
```

##### documentTypePO

```
ro.sync.exml.editor.persistance.DocumentTypePO documentTypePO
```

##### dropHandlers

```
List dropHandlers
```

##### editorClosed

```
boolean editorClosed
```

##### editorPopUpCustomizer

```
PopupMenuCustomizer editorPopUpCustomizer
```

##### elementsPanel

```
ro.sync.ecss.component.ui.context.elements.ElementsPanel elementsPanel
```

##### entitiesPanel

```
ro.sync.ecss.component.ui.context.entities.EntitiesPanel entitiesPanel
```

##### expandAllTopicRefs

```
boolean expandAllTopicRefs
```

##### extensionStateListener

```
AuthorExtensionStateListener extensionStateListener
```

##### filteredContentWarningPanel

```
ro.sync.exml.editor.xmleditor.pageauthor.FilteredContentWarningPanel filteredContentWarningPanel
```

##### gotoDefinitionAction

```
ro.sync.ecss.component.ui.actions.edit.GoToDefinitionAction gotoDefinitionAction
```

##### host

```
ro.sync.ecss.component.SwingAuthorHostComponent host
```

##### idLocationProvider

```
ro.sync.exml.editor.identifiers.XMLIDLocationProvider idLocationProvider
```

##### initialSchemaManager

```
ro.sync.contentcompletion.SchemaManagerProvider initialSchemaManager
```

##### inRefresh

```
boolean inRefresh
```

##### isEditorReadOnlyForActionsUpdate

```
boolean isEditorReadOnlyForActionsUpdate
```

##### isEditorSelected

```
boolean isEditorSelected
```

##### isPageSelected

```
boolean isPageSelected
```

##### keysHaveChanged

```
boolean keysHaveChanged
```

##### keysManagerListener

```
ro.sync.ecss.dita.reference.keyref.KeysManagerListener keysManagerListener
```

##### lastCaretOffset

```
int lastCaretOffset
```

##### lastDetectTime

```
long lastDetectTime
```

##### learnWordSpellingAction

```
ro.sync.ui.application.action.AccelAction learnWordSpellingAction
```

##### markersManager

```
ro.sync.ecss.component.markers.AuthorPageMarkersManager markersManager
```

##### modifiedReferencesCollector

```
ro.sync.exml.editor.xmleditor.pageauthor.modifiedreferences.ModifiedReferencesCollector modifiedReferencesCollector
```

##### modifiedURLs

```
Set<String> modifiedURLs
```

##### openFileAtCaretAction

```
ro.sync.ecss.component.ui.actions.edit.OpenFileAtCaretAction openFileAtCaretAction
```

##### optionsStorage

```
OptionsStorage optionsStorage
```

##### outliner

```
ro.sync.ecss.component.ui.outline.AuthorOutlinerPanel outliner
```

##### pluggableActions

```
List<ro.sync.ui.application.action.AccelAction> pluggableActions
```

##### positionInMapPanel

```
ro.sync.exml.editor.xmleditor.pageauthor.PositionInMapPanel positionInMapPanel
```

##### quickAssistAction

```
ro.sync.exml.editor.actions.QuickAssistAction quickAssistAction
```

##### quickAssistManager

```
ro.sync.exml.editor.quickassist.author.AuthorQuickAssistManager quickAssistManager
```

##### quickAssistPresenter

```
ro.sync.exml.editor.xmleditor.pageauthor.AuthorQuickAssistPresenter quickAssistPresenter
```

##### quickAssistStripe

```
ro.sync.ui.stripes.AuthorQuickAssistStripe quickAssistStripe
```

##### rangeStripe

```
ro.sync.ecss.component.stripes.AuthorRangeStripe rangeStripe
```

##### referencesResolver

```
ro.sync.ecss.component.AuthorContentReferencesResolverImpl referencesResolver
```

##### resolverProgressTracker

```
ro.sync.exml.editor.xmleditor.pageauthor.AuthorConrefResolverProgressTracker resolverProgressTracker
```

##### scrollPane

```
ro.sync.exml.editor.xmleditor.pageauthor.bookmarks.AuthorMarkScrollPane scrollPane
```

##### southPanel

```
JPanel southPanel
```

##### spellChecker

```
ro.sync.ecss.component.spellcheck.AuthorAutoSpellCheck spellChecker
```

##### startupDocumentTypeProvider

```
ro.sync.exml.editor.xmleditor.pageauthor.StartupDocumentTypeProvider startupDocumentTypeProvider
```

##### urlsDndHandler

```
AuthorExternalObjectInsertionHandler urlsDndHandler
```

##### usedRootMap

```
URL usedRootMap
```

##### validationStateManager

```
ro.sync.exml.editor.helpers.validation.ValidationStateManager validationStateManager
```

##### validationStatusHelper

```
ro.sync.ecss.component.validation.ValidationStatusPanelManager validationStatusHelper
```

##### viewport

```
ro.sync.ecss.component.AuthorViewport viewport
```

##### viewportWidth

```
int viewportWidth
```

##### xmlOperationProcessor

```
ro.sync.exml.editor.XMLOperationProcessor xmlOperationProcessor
```

### Class ro.sync.exml.editor.xmleditor.pageauthor.CSSMenuButton

class CSSMenuButton extends ro.sync.ui.ApplicationSplitButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### actions

```
List<Action> actions
```

##### behaveLikeRadio

```
boolean behaveLikeRadio
```

##### mergedCSSs

```
List<CSSGroup> mergedCSSs
```

##### selectedMergedCSSs

```
List<CSSGroup> selectedMergedCSSs
```

##### systemIdProvider

```
ro.sync.basic.io.SystemIdProvider systemIdProvider
```

### Class ro.sync.exml.editor.xmleditor.pageauthor.FilteredContentWarningPanel

class FilteredContentWarningPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### filtereContentdWarningLabel

```
JLabel filtereContentdWarningLabel
```

##### showForContentStructure

```
boolean showForContentStructure
```

### Class ro.sync.exml.editor.xmleditor.pageauthor.PositionInMapPanel

class PositionInMapPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### docDescriptor

```
ro.sync.document.Descriptor docDescriptor
```

##### next

```
ro.sync.ui.toolbar.ToolBarButton next
```

##### occurrencesLabel

```
JLabel occurrencesLabel
```

##### prev

```
ro.sync.ui.toolbar.ToolBarButton prev
```

##### selInterractor

```
ro.sync.exml.editor.xmleditor.pageauthor.DITAMapSelectionInteractor selInterractor
```

##### timer

```
ro.sync.exml.editor.helpers.SwingTimer timer
```

## Package [ro.sync.exml.options](ro/sync/exml/options/package-summary.md)

### Class ro.sync.exml.options.AntOptionPane

class AntOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### builtinAntLabel

```
JLabel builtinAntLabel
```

##### builtinRadioButton

```
JRadioButton builtinRadioButton
```

##### customFilePanel

```
ro.sync.ui.InputFilePanel customFilePanel
```

##### customRadioButton

```
JRadioButton customRadioButton
```

##### inhibitListener

```
boolean inhibitListener
```

### Class ro.sync.exml.options.ApplicationLayoutOptionPane

class ApplicationLayoutOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### browseLocal

```
ro.sync.ui.application.action.TaggedAction browseLocal
```

##### editorsTabOnBottomRadioButton

```
JRadioButton editorsTabOnBottomRadioButton
```

##### editorsTabOnTopRadioButton

```
JRadioButton editorsTabOnTopRadioButton
```

##### enableFloatableEditors

```
JCheckBox enableFloatableEditors
```

##### inputEditorVariablesAction

```
ro.sync.ui.application.action.TaggedAction inputEditorVariablesAction
```

##### predefinedLayoutRadioButton

```
JRadioButton predefinedLayoutRadioButton
```

##### predefinedLayoutsCombo

```
JComboBox predefinedLayoutsCombo
```

##### rememberLayoutChangesPerProject

```
JCheckBox rememberLayoutChangesPerProject
```

##### resetLayoutAtStartup

```
JCheckBox resetLayoutAtStartup
```

##### specifiedLayoutPathField

```
ro.sync.ui.UndoableTextField specifiedLayoutPathField
```

##### specifiedLayoutRadioButton

```
JRadioButton specifiedLayoutRadioButton
```

##### useDefaultLayoutRadioButton

```
JRadioButton useDefaultLayoutRadioButton
```

##### viewsTabOnBottomRadioButton

```
JRadioButton viewsTabOnBottomRadioButton
```

##### viewsTabOnTopRadioButton

```
JRadioButton viewsTabOnTopRadioButton
```

### Class ro.sync.exml.options.AttributeNamesEditorPanel

class AttributeNamesEditorPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### downButton

```
JButton downButton
```

##### list

```
JList list
```

##### model

```
DefaultListModel model
```

##### removeButton

```
JButton removeButton
```

##### upButton

```
JButton upButton
```

### Class ro.sync.exml.options.AuthorAutoCorrectOptionPane

class AuthorAutoCorrectOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### autocorrectCheckBox

```
JCheckBox autocorrectCheckBox
```

##### autocorrectReplacementsTable

```
ro.sync.exml.options.common.AutocorrectReplacementsTablePanel autocorrectReplacementsTable
```

##### autocorrectSupport

```
ro.sync.ecss.autocorrect.AutocorrectOptionsSupport autocorrectSupport
```

##### customDictLoc

```
String customDictLoc
```

##### endDoubleQuoteButton

```
JButton endDoubleQuoteButton
```

##### endSingleQuoteButton

```
JButton endSingleQuoteButton
```

##### langComboIndexBasedOnSpellCheckLang

```
int langComboIndexBasedOnSpellCheckLang
```

##### languagesComboBox

```
JComboBox languagesComboBox
```

##### loadAdditionalDicts

```
boolean loadAdditionalDicts
```

##### replaceDoubleQuoteCheckBox

```
JCheckBox replaceDoubleQuoteCheckBox
```

##### replaceSingleQuoteCheckBox

```
JCheckBox replaceSingleQuoteCheckBox
```

##### startDoubleQuoteButton

```
JButton startDoubleQuoteButton
```

##### startSingleQuoteButton

```
JButton startSingleQuoteButton
```

##### storing

```
boolean storing
```

##### useDocTypeSuggestions

```
JCheckBox useDocTypeSuggestions
```

##### useSpellCheckDicts

```
JCheckBox useSpellCheckDicts
```

### Class ro.sync.exml.options.AuthorCaretNavigationOptionPane

class AuthorCaretNavigationOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### avoidPositionsBetweenBlocksAfterDelCheckBox

```
JCheckBox avoidPositionsBetweenBlocksAfterDelCheckBox
```

##### caretProximityHighlightColor

```
ro.sync.exml.options.ColorButton caretProximityHighlightColor
```

##### moveCaretInTheReadingDirectionCheckBox

```
JCheckBox moveCaretInTheReadingDirectionCheckBox
```

##### quickNavigationInTablesCheckBox

```
JCheckBox quickNavigationInTablesCheckBox
```

##### quickUpDownNavigation

```
JCheckBox quickUpDownNavigation
```

##### showCaretPositionInfo

```
JCheckBox showCaretPositionInfo
```

##### showCaretProximityHighlight

```
JCheckBox showCaretProximityHighlight
```

##### showLocationTooltipOnMouseMove

```
JCheckBox showLocationTooltipOnMouseMove
```

### Class ro.sync.exml.options.AuthorEditorOptionPane

class AuthorEditorOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### authorBackgroundColorButton

```
ro.sync.exml.options.ColorButton authorBackgroundColorButton
```

##### authorForegroundColorButton

```
ro.sync.exml.options.ColorButton authorForegroundColorButton
```

##### compactMode

```
JCheckBox compactMode
```

##### displayModeCombo

```
JComboBox displayModeCombo
```

##### displayReferencesExpanded

```
JCheckBox displayReferencesExpanded
```

##### editResolvedReferredContent

```
JCheckBox editResolvedReferredContent
```

##### fastTextLayoutCheckBox

```
JCheckBox fastTextLayoutCheckBox
```

##### imageWidthLimitToScale

```
ro.sync.ui.UndoableTextField imageWidthLimitToScale
```

##### loadVeryLargeImages

```
JCheckBox loadVeryLargeImages
```

##### restrictEditingReferredContentToLocalFiles

```
JCheckBox restrictEditingReferredContentToLocalFiles
```

##### showAuthorRangeStripe

```
JCheckBox showAuthorRangeStripe
```

##### showDoctypes

```
JCheckBox showDoctypes
```

##### showEmptyInlineElements

```
JCheckBox showEmptyInlineElements
```

##### showLayoutMessages

```
JCheckBox showLayoutMessages
```

##### showPIs

```
JCheckBox showPIs
```

##### showSelectionFloatingToolbar

```
JCheckBox showSelectionFloatingToolbar
```

##### showXMLComments

```
JCheckBox showXMLComments
```

##### sortAttrsForFullTagsWithAttrs

```
JCheckBox sortAttrsForFullTagsWithAttrs
```

##### tagsBackgroundColor

```
ro.sync.exml.options.ColorButton tagsBackgroundColor
```

##### tagsFontButton

```
ro.sync.exml.options.common.FontPanel tagsFontButton
```

##### tagsForegroundColor

```
ro.sync.exml.options.ColorButton tagsForegroundColor
```

### Class ro.sync.exml.options.AuthorMathMLOptionPane

class AuthorMathMLOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### externalEditorCommandLine

```
ro.sync.ui.UndoableTextField externalEditorCommandLine
```

##### mathFlowInstallationDir

```
ro.sync.ui.UndoableTextField mathFlowInstallationDir
```

##### mathFlowLicenseFile

```
ro.sync.ui.UndoableTextField mathFlowLicenseFile
```

##### minimumFontSizeCB

```
JComboBox minimumFontSizeCB
```

##### saveSpecialCharsAsCharEntities

```
JRadioButton saveSpecialCharsAsCharEntities
```

##### saveSpecialCharsAsCharValues

```
JRadioButton saveSpecialCharsAsCharValues
```

##### saveSpecialCharsAsEntityNames

```
JRadioButton saveSpecialCharsAsEntityNames
```

##### simpleEditorRB

```
JRadioButton simpleEditorRB
```

##### structureEditorRB

```
JRadioButton structureEditorRB
```

##### styleEditorRB

```
JRadioButton styleEditorRB
```

### Class ro.sync.exml.options.AuthorReviewCalloutsOptionPane

class AuthorReviewCalloutsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### calloutsTextLimitComboBox

```
ro.sync.ui.application.ApplicationComboBox calloutsTextLimitComboBox
```

##### calloutsTextLimitLabel

```
JLabel calloutsTextLimitLabel
```

##### calloutsWidthComboBox

```
ro.sync.ui.application.ApplicationComboBox calloutsWidthComboBox
```

##### calloutsWidthLabel

```
JLabel calloutsWidthLabel
```

##### showCommentsCheckBox

```
JCheckBox showCommentsCheckBox
```

##### showConnectingLinesCheckBox

```
JCheckBox showConnectingLinesCheckBox
```

##### showDeletedContentCheckBox

```
JCheckBox showDeletedContentCheckBox
```

##### showDeletionsCheckBox

```
JCheckBox showDeletionsCheckBox
```

##### showInsertedContentCheckBox

```
JCheckBox showInsertedContentCheckBox
```

##### showInsertionsCheckBox

```
JCheckBox showInsertionsCheckBox
```

##### showReviewTimeCheckBox

```
JCheckBox showReviewTimeCheckBox
```

### Class ro.sync.exml.options.AuthorReviewOptionPane

class AuthorReviewOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### authorNameTextField

```
ro.sync.ui.UndoableTextField authorNameTextField
```

##### authorsAssignColorsPanel

```
ro.sync.exml.options.AuthorsAssignedColorsPanel authorsAssignColorsPanel
```

##### autoColorForComment

```
JRadioButton autoColorForComment
```

##### autoColorForDelete

```
JRadioButton autoColorForDelete
```

##### autoColorForInsert

```
JRadioButton autoColorForInsert
```

##### commentColorButton

```
ro.sync.exml.options.ColorButton commentColorButton
```

##### customColorForComment

```
JRadioButton customColorForComment
```

##### customColorForDelete

```
JRadioButton customColorForDelete
```

##### customColorForInsert

```
JRadioButton customColorForInsert
```

##### deleteColorButton

```
ro.sync.exml.options.ColorButton deleteColorButton
```

##### displayChangedLineMarkers

```
JCheckBox displayChangedLineMarkers
```

##### displayModeCombo

```
ro.sync.ui.application.ApplicationComboBox displayModeCombo
```

##### initialStateCombo

```
ro.sync.ui.application.ApplicationComboBox initialStateCombo
```

##### insertColorButton

```
ro.sync.exml.options.ColorButton insertColorButton
```

##### showInfoMessage

```
boolean showInfoMessage
```

##### transparencyForCommentSlider

```
JSlider transparencyForCommentSlider
```

##### transparencyForDeleteSlider

```
JSlider transparencyForDeleteSlider
```

##### transparencyForInsertSlider

```
JSlider transparencyForInsertSlider
```

##### useColorForBGForDelete

```
JCheckBox useColorForBGForDelete
```

##### useColorForBGForInsert

```
JCheckBox useColorForBGForInsert
```

##### useColorForFGForDelete

```
JCheckBox useColorForFGForDelete
```

##### useColorForFGForInsert

```
JCheckBox useColorForFGForInsert
```

### Class ro.sync.exml.options.AuthorsAssignedColorsPanel

class AuthorsAssignedColorsPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### colorsListComponent

```
JList colorsListComponent
```

##### colorsListModel

```
DefaultListModel colorsListModel
```

##### removeButton

```
JButton removeButton
```

### Class ro.sync.exml.options.AuthorSchemaAwareEditingOptionPane

class AuthorSchemaAwareEditingOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### autoApplyBestSolution

```
JCheckBox autoApplyBestSolution
```

##### contentCompletionLabel

```
JLabel contentCompletionLabel
```

##### convertExternalAlsoInSpacePreserve

```
JCheckBox convertExternalAlsoInSpacePreserve
```

##### convertExternalContentOnPaste

```
JCheckBox convertExternalContentOnPaste
```

##### convertPastedURLsToLinks

```
JCheckBox convertPastedURLsToLinks
```

##### customRadio

```
JRadioButton customRadio
```

##### deleteElementTagsSmart

```
JCheckBox deleteElementTagsSmart
```

##### deleteElementTagsWithBackspaceLabel

```
JLabel deleteElementTagsWithBackspaceLabel
```

##### deleteElementValidateOperationResult

```
JCheckBox deleteElementValidateOperationResult
```

##### insertOnlyValidAttrValues

```
JCheckBox insertOnlyValidAttrValues
```

##### insertOnlyValidElements

```
JCheckBox insertOnlyValidElements
```

##### joinWarnOnInvalid

```
JCheckBox joinWarnOnInvalid
```

##### offRadio

```
JRadioButton offRadio
```

##### onRadio

```
JRadioButton onRadio
```

##### pasteAndDnDLabel

```
JLabel pasteAndDnDLabel
```

##### pasteDNDSmart

```
JCheckBox pasteDNDSmart
```

##### pasteDNDValidateOperationResult

```
JCheckBox pasteDNDValidateOperationResult
```

##### saIndentCSSBlocksOnly

```
JCheckBox saIndentCSSBlocksOnly
```

##### saNormalizeAndFormat

```
JCheckBox saNormalizeAndFormat
```

##### schemaAwareOptions

```
ro.sync.ecss.component.AuthorSchemaAwareOptions schemaAwareOptions
```

##### showAllPossibleElementsInCC

```
JCheckBox showAllPossibleElementsInCC
```

##### showAvailableCCItemsOnEnter

```
JCheckBox showAvailableCCItemsOnEnter
```

##### typingLabel

```
JLabel typingLabel
```

##### typingSmart

```
JCheckBox typingSmart
```

##### typingValidateOperationResult

```
JCheckBox typingValidateOperationResult
```

##### unwrapWarnOnInvalid

```
JCheckBox unwrapWarnOnInvalid
```

##### warnOnInvalidContent

```
JLabel warnOnInvalidContent
```

### Class ro.sync.exml.options.AuthorSerializationOptionPane

class AuthorSerializationOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### compatibilityModeCombo

```
JComboBox compatibilityModeCombo
```

##### formatEntireDocument

```
JRadioButton formatEntireDocument
```

##### formatEntireDocumentAsInText

```
JCheckBox formatEntireDocumentAsInText
```

##### formatOnlyModified

```
JRadioButton formatOnlyModified
```

### Class ro.sync.exml.options.AutoCorrectQuotesOptions

class AutoCorrectQuotesOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### enabled

```
boolean enabled
```

##### endQuote

```
char endQuote
```

##### startQuote

```
char startQuote
```

### Class ro.sync.exml.options.BooleanRenderer

class BooleanRenderer extends [JCheckBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JCheckBox.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.CatalogsURITablePanel

class CatalogsURITablePanel extends ro.sync.exml.options.common.URITablePanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### provider

```
ro.sync.util.editorvars.FrameworkVariablesResolver provider
```

### Class ro.sync.exml.options.CertificatesOptionPane

class CertificatesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### certificateAliasField

```
ro.sync.ui.UndoableTextField certificateAliasField
```

##### keystoreFileField

```
ro.sync.ui.UndoableTextField keystoreFileField
```

##### keystorePasswordField

```
ro.sync.ui.application.ApplicationPasswordField keystorePasswordField
```

##### keystoreTypeComboBox

```
JComboBox keystoreTypeComboBox
```

##### privateKeyPasswordField

```
ro.sync.ui.application.ApplicationPasswordField privateKeyPasswordField
```

### Class ro.sync.exml.options.ChooseXSDPanel

class ChooseXSDPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### xmlSchemaURLPanel

```
ro.sync.ui.InputUrlPanel xmlSchemaURLPanel
```

### Class ro.sync.exml.options.CodeTemplatesOptionPane

class CodeTemplatesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### additionalFolderPanel

```
ro.sync.ui.InputFilePanel additionalFolderPanel
```

##### deleteAction

```
ro.sync.ui.application.action.ApplicationAbstractAction deleteAction
```

##### deleteButton

```
JButton deleteButton
```

##### model

```
ro.sync.exml.options.CodeTemplatesOptionPane.DataTableModel model
```

##### previewTextArea

```
ro.sync.syntaxhighlight.SHTextArea previewTextArea
```

##### table

```
ro.sync.ui.table.SortableTable table
```

### Class ro.sync.exml.options.ColorAlphaChooserPanel

class ColorAlphaChooserPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### alphaSlider

```
JSlider alphaSlider
```

##### colorButton

```
ro.sync.exml.options.ColorButton colorButton
```

##### disableColorListener

```
boolean disableColorListener
```

##### disableSliderListener

```
boolean disableSliderListener
```

### Class ro.sync.exml.options.ColorAndStylePanel

class ColorAndStylePanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### bgColor

```
Color bgColor
```

##### bgColorButton

```
ro.sync.exml.options.ColorButton bgColorButton
```

##### bgColorCheck

```
JCheckBox bgColorCheck
```

##### boldCheck

```
JCheckBox boldCheck
```

##### fgColorButton

```
ro.sync.exml.options.ColorButton fgColorButton
```

##### fgLabel

```
JLabel fgLabel
```

##### italicCheck

```
JCheckBox italicCheck
```

##### ltgtCheck

```
JCheckBox ltgtCheck
```

##### ltgtColorButton

```
ro.sync.exml.options.ColorButton ltgtColorButton
```

##### ltgtFgColor

```
Color ltgtFgColor
```

##### stylesLabel

```
JLabel stylesLabel
```

### Class ro.sync.exml.options.ColorButton

class ColorButton extends ro.sync.ui.application.ApplicationButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### cIcon

```
ro.sync.exml.options.ColorIcon cIcon
```

##### colorListeners

```
List colorListeners
```

### Class ro.sync.exml.options.ColorOptionPane

class ColorOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### additionalXMLPreviews

```
ro.sync.syntaxhighlight.SHTextArea[] additionalXMLPreviews
```

##### colorAndStylePanel

```
ro.sync.exml.options.ColorAndStylePanel colorAndStylePanel
```

##### discard

```
boolean discard
```

##### enableNestedSyntaxHighlightCheckBox

```
JCheckBox enableNestedSyntaxHighlightCheckBox
```

##### lastSelectedSHMarker

```
ro.sync.exml.options.sh.SHMarker lastSelectedSHMarker
```

##### mainPreviewArea

```
ro.sync.syntaxhighlight.SHTextArea mainPreviewArea
```

##### markers

```
ro.sync.exml.options.sh.SHMarker[] markers
```

##### markersTree

```
ro.sync.ui.application.ApplicationTree markersTree
```

##### previewPane

```
JTabbedPane previewPane
```

### Class ro.sync.exml.options.CSSBasedProcessorsOptionPane

class CSSBasedProcessorsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### autodetectChemistry

```
JRadioButton autodetectChemistry
```

##### chemistryInputPanel

```
ro.sync.ui.InputFilePanel chemistryInputPanel
```

##### chemistryMemoryCombo

```
JComboBox chemistryMemoryCombo
```

##### enablePDFUA_1Check

```
JCheckBox enablePDFUA_1Check
```

##### externalChemistryDir

```
JRadioButton externalChemistryDir
```

##### openConsoleAlwaysRadio

```
JRadioButton openConsoleAlwaysRadio
```

##### openConsoleWhenBuildFailsRadio

```
JRadioButton openConsoleWhenBuildFailsRadio
```

### Class ro.sync.exml.options.CSSValidatorOptionPane

class CSSValidatorOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### ignoredPropertiesPatterns

```
ro.sync.ui.UndoableTextField ignoredPropertiesPatterns
```

##### mediaCombo

```
JComboBox mediaCombo
```

##### profileCombo

```
JComboBox profileCombo
```

##### recognizeBrowserExtCheck

```
JCheckBox recognizeBrowserExtCheck
```

##### warningLevelCombo

```
JComboBox warningLevelCombo
```

### Class ro.sync.exml.options.CustomEditorVariablesOptionPane

class CustomEditorVariablesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### customVarsPanel

```
ro.sync.exml.options.CustomEditorVariablesPanel customVarsPanel
```

### Class ro.sync.exml.options.CustomEditorVariablesPanel

class CustomEditorVariablesPanel extends ro.sync.ui.table.EditableSortableTablePanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### model

```
ro.sync.exml.options.CustomEditorVariablesPanel.CustomEditorVariablesTableModel model
```

### Class ro.sync.exml.options.CustomEditorVariablesPanel.CustomEditorVariablesTableModel

class CustomEditorVariablesTableModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### data

```
List<ro.sync.util.editorvars.UserEditorVariablePO> data
```

### Class ro.sync.exml.options.CustomEnginesOptionPane

class CustomEnginesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### changeDialog

```
ro.sync.exml.options.CustomEngineEditDialog changeDialog
```

##### hasAdditionalContent

```
boolean hasAdditionalContent
```

##### model

```
ro.sync.exml.options.CustomEnginesOptionPane.CustomEngineModel model
```

##### tablePanel

```
ro.sync.ui.table.EditableTablePanel tablePanel
```

### Class ro.sync.exml.options.CustomValidationOptionPane

class CustomValidationOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### model

```
ro.sync.exml.options.CustomValidationOptionPane.CustomErrorScannerTableModel model
```

##### tablePanel

```
ro.sync.ui.table.EditableTablePanel tablePanel
```

### Class ro.sync.exml.options.DBFiltersOptionPane

class DBFiltersOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### showAlias

```
JCheckBox showAlias
```

##### showGlobalTemp

```
JCheckBox showGlobalTemp
```

##### showLocalTemp

```
JCheckBox showLocalTemp
```

##### showSynonym

```
JCheckBox showSynonym
```

##### showSystem

```
JCheckBox showSystem
```

##### showTable

```
JCheckBox showTable
```

##### showView

```
JCheckBox showView
```

### Class ro.sync.exml.options.DBImportOptionPane

class DBImportOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### createEmptyElemForEmptyVals

```
JCheckBox createEmptyElemForEmptyVals
```

##### createEmptyElemForNullVals

```
JCheckBox createEmptyElemForNullVals
```

##### customFormatRadioButton

```
JRadioButton customFormatRadioButton
```

##### dateChooserPanel

```
ro.sync.exml.options.DBImportOptionPane.FormatChooserPanel dateChooserPanel
```

##### dateTimeChooserPanel

```
ro.sync.exml.options.DBImportOptionPane.FormatChooserPanel dateTimeChooserPanel
```

##### dateTypesTabbedPane

```
JTabbedPane dateTypesTabbedPane
```

##### escapeContentAsXML

```
JCheckBox escapeContentAsXML
```

##### generateAnnotationsForSchema

```
JCheckBox generateAnnotationsForSchema
```

##### timeChooserPanel

```
ro.sync.exml.options.DBImportOptionPane.FormatChooserPanel timeChooserPanel
```

##### unformattedDateRadioButton

```
JRadioButton unformattedDateRadioButton
```

##### xmlSchemaFormatRadioButton

```
JRadioButton xmlSchemaFormatRadioButton
```

### Class ro.sync.exml.options.DBOptionPane

class DBOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### connectionsTable

```
ro.sync.ui.KeySearchTable connectionsTable
```

##### connectionTablePanel

```
ro.sync.ui.table.EditableTablePanel connectionTablePanel
```

##### dataSourceConnectionTableModel

```
ro.sync.exml.options.DBSourceConnectionsModel dataSourceConnectionTableModel
```

##### dataSourceList

```
List<ro.sync.db.core.DBSourceDriverInfo> dataSourceList
```

##### dataSourceTable

```
ro.sync.ui.KeySearchTable dataSourceTable
```

##### dataSourceTableModel

```
ro.sync.exml.options.DBOptionPane.DataSourceDriversModel dataSourceTableModel
```

##### dataSourceTablePanel

```
ro.sync.ui.table.EditableTablePanel dataSourceTablePanel
```

##### limitCellsNumberField

```
ro.sync.ui.UndoableTextField limitCellsNumberField
```

##### navigationTreeWindowNumberField

```
ro.sync.ui.UndoableTextField navigationTreeWindowNumberField
```

### Class ro.sync.exml.options.DBSourceConfiguratorBase

class DBSourceConfiguratorBase extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### sessionID

```
int sessionID
```

### Class ro.sync.exml.options.DBSourceConnectionsModel

class DBSourceConnectionsModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### connectionsList

```
List<ro.sync.db.DBConnectionInfo> connectionsList
```

### Class ro.sync.exml.options.DebuggerOptionPane

class DebuggerOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### debugAlwaysAsk

```
JRadioButton debugAlwaysAsk
```

##### debugAlwaysStop

```
JRadioButton debugAlwaysStop
```

##### debuggerCurrentInstructionPointer

```
ro.sync.exml.options.ColorAlphaChooserPanel debuggerCurrentInstructionPointer
```

##### debugNeverStop

```
JRadioButton debugNeverStop
```

##### enableOptimizationsCheck

```
JCheckBox enableOptimizationsCheck
```

##### horizontalSplit

```
JRadioButton horizontalSplit
```

##### maxXslTemplatesTextField

```
ro.sync.ui.UndoableTextField maxXslTemplatesTextField
```

##### redirectSaxonOutput

```
JCheckBox redirectSaxonOutput
```

##### useInfiniteLoopCheck

```
JCheckBox useInfiniteLoopCheck
```

##### verticalSplit

```
JRadioButton verticalSplit
```

##### xWatchTimeoutTextField

```
ro.sync.ui.UndoableTextField xWatchTimeoutTextField
```

### Class ro.sync.exml.options.DiffAppearanceOptionPane

class DiffAppearanceOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### commentCalloutWidthCombo

```
ro.sync.ui.application.ApplicationComboBox commentCalloutWidthCombo
```

##### commentCalloutWidthLabel

```
JLabel commentCalloutWidthLabel
```

##### conflictColorButton

```
ro.sync.exml.options.ColorButton conflictColorButton
```

##### incomingColorButton

```
ro.sync.exml.options.ColorButton incomingColorButton
```

##### lineWrap

```
JCheckBox lineWrap
```

##### outgoingColorButton

```
ro.sync.exml.options.ColorButton outgoingColorButton
```

##### showCommentCallouts

```
JCheckBox showCommentCallouts
```

### Class ro.sync.exml.options.DiffDirsAppearanceOptionPane

class DiffDirsAppearanceOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### addDeleteColorButton

```
ro.sync.exml.options.ColorButton addDeleteColorButton
```

##### modifiedColorButton

```
ro.sync.exml.options.ColorButton modifiedColorButton
```

### Class ro.sync.exml.options.DiffDirsOptionPane

class DiffDirsOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### alwaysAsk

```
JRadioButton alwaysAsk
```

##### doNothing

```
JRadioButton doNothing
```

##### goToNextPrevious

```
JRadioButton goToNextPrevious
```

##### lookInArchives

```
JCheckBox lookInArchives
```

##### optionPresenter

```
ro.sync.options.IOptionDialog optionPresenter
```

##### performBinaryFilesComparison

```
JRadioButton performBinaryFilesComparison
```

##### performContentFilesComparison

```
JRadioButton performContentFilesComparison
```

##### performTimestampFilesComparison

```
JRadioButton performTimestampFilesComparison
```

### Class ro.sync.exml.options.DiffFilesOptionPane

class DiffFilesOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### browseCompareAppAction

```
ro.sync.ui.application.action.TaggedAction browseCompareAppAction
```

##### defaultXPathCheck

```
JCheckBox defaultXPathCheck
```

##### defaultXPathField

```
ro.sync.syntaxhighlight.textfield.SHTextField defaultXPathField
```

##### enableComparisonInAuthorMode

```
JCheckBox enableComparisonInAuthorMode
```

##### externalComparatorLocation

```
ro.sync.ui.UndoableTextField externalComparatorLocation
```

##### ignoreAttrsOrder

```
JCheckBox ignoreAttrsOrder
```

##### ignoreCDATA

```
JCheckBox ignoreCDATA
```

##### ignoreComments

```
JCheckBox ignoreComments
```

##### ignoreDOCTYPE

```
JCheckBox ignoreDOCTYPE
```

##### ignoreNamespaceDeclarations

```
JCheckBox ignoreNamespaceDeclarations
```

##### ignoreNamespaces

```
JCheckBox ignoreNamespaces
```

##### ignorePI

```
JCheckBox ignorePI
```

##### ignorePrefixes

```
JCheckBox ignorePrefixes
```

##### ignoreStateOfEmptyElements

```
JCheckBox ignoreStateOfEmptyElements
```

##### ignoreText

```
JCheckBox ignoreText
```

##### ignoreWhitespaces

```
JCheckBox ignoreWhitespaces
```

##### markEndTagsAsDifferent

```
JCheckBox markEndTagsAsDifferent
```

##### mergeAdjacentDifferences

```
JCheckBox mergeAdjacentDifferences
```

##### openComparisonsInEditorArea

```
JCheckBox openComparisonsInEditorArea
```

##### showPseudoConflicts

```
JCheckBox showPseudoConflicts
```

##### threeWayAlgorithmsCombo

```
JComboBox threeWayAlgorithmsCombo
```

##### threeWayDiffAlgorithmComplexityLevel

```
ro.sync.ui.application.ApplicationComboBox threeWayDiffAlgorithmComplexityLevel
```

##### twoWayAlgorithmsCombo

```
JComboBox twoWayAlgorithmsCombo
```

##### twoWayDiffAlgorithmComplexityLevel

```
ro.sync.ui.application.ApplicationComboBox twoWayDiffAlgorithmComplexityLevel
```

##### useExternalDiff

```
JCheckBox useExternalDiff
```

### Class ro.sync.exml.options.DITALoggingOptionPane

class DITALoggingOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### ditaOTErrorsCheckBox

```
JCheckBox ditaOTErrorsCheckBox
```

##### ditaOTInfosCheckBox

```
JCheckBox ditaOTInfosCheckBox
```

##### ditaOTWarnsCheckBox

```
JCheckBox ditaOTWarnsCheckBox
```

##### fopErrorsCheckBox

```
JCheckBox fopErrorsCheckBox
```

##### fopInfosCheckBox

```
JCheckBox fopInfosCheckBox
```

##### fopWarningsCheckBox

```
JCheckBox fopWarningsCheckBox
```

##### openConsoleAlwaysRadio

```
JRadioButton openConsoleAlwaysRadio
```

##### openConsoleWhenBuildFailsRadio

```
JRadioButton openConsoleWhenBuildFailsRadio
```

##### xsltProblemsCheckBox

```
JCheckBox xsltProblemsCheckBox
```

### Class ro.sync.exml.options.DITAOptionPane

class DITAOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### browseForDitaOtDirAction

```
ro.sync.ui.application.action.TaggedAction browseForDitaOtDirAction
```

##### ditaOTBuiltinDirRadio

```
JRadioButton ditaOTBuiltinDirRadio
```

##### ditaOTCustomDirRadio

```
JRadioButton ditaOTCustomDirRadio
```

##### ditaOtDirectoryComboBox

```
ro.sync.ui.HistoryComboBox ditaOtDirectoryComboBox
```

##### editorVariablesInputUrlAction

```
ro.sync.ui.application.action.TaggedAction editorVariablesInputUrlAction
```

##### enableDITA2_0Support

```
JCheckBox enableDITA2_0Support
```

##### extraPluginContributedDITAOTRadios

```
LinkedHashMap<ro.sync.exml.plugin.AdditionalPluginFolderDescription,JRadioButton> extraPluginContributedDITAOTRadios
```

##### usedFromOxygen

```
boolean usedFromOxygen
```

### Class ro.sync.exml.options.DITAShowConsoleErrorsInTransformationPO

class DITAShowConsoleErrorsInTransformationPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### showDITAOTErrors

```
boolean showDITAOTErrors
```

##### showDITAOTInfos

```
boolean showDITAOTInfos
```

##### showDITAOTWarnings

```
boolean showDITAOTWarnings
```

##### showFopErrors

```
boolean showFopErrors
```

##### showFopInfos

```
boolean showFopInfos
```

##### showFopWarns

```
boolean showFopWarns
```

##### showXsltProblems

```
boolean showXsltProblems
```

### Class ro.sync.exml.options.DocumentTemplatesOptionPane

class DocumentTemplatesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### templatesPanel

```
ro.sync.exml.options.documenttype.DocumentTemplatesPanel templatesPanel
```

### Class ro.sync.exml.options.DocumentTypeAssociationOptionPane

class DocumentTypeAssociationOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### docTypesPanel

```
ro.sync.exml.options.documenttype.DocumentTypesPresenterPanel docTypesPanel
```

##### dtdSupportInRuleMatchingCheckBox

```
JCheckBox dtdSupportInRuleMatchingCheckBox
```

##### onlyForLocalDTDsCheckBox

```
JCheckBox onlyForLocalDTDsCheckBox
```

##### useGrammarCacheCheckBox

```
JCheckBox useGrammarCacheCheckBox
```

### Class ro.sync.exml.options.DocumentTypeCustomLocationsOptionPane

class DocumentTypeCustomLocationsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### customFrameworksDirFolderRadio

```
JRadioButton customFrameworksDirFolderRadio
```

##### customFrameworksDirTextField

```
ro.sync.ui.UndoableTextField customFrameworksDirTextField
```

##### defaultFrameworksDirRadio

```
JRadioButton defaultFrameworksDirRadio
```

##### defaultFrameworksDirTextField

```
ro.sync.ui.UndoableTextField defaultFrameworksDirTextField
```

##### frameworksBrowseAction

```
ro.sync.ui.application.action.TaggedAction frameworksBrowseAction
```

##### frameworksEditorVariablesAction

```
ro.sync.ui.application.action.TaggedAction frameworksEditorVariablesAction
```

##### tablePanel

```
ro.sync.exml.options.common.URITablePanel tablePanel
```

### Class ro.sync.exml.options.EditorCCAnnotationsOptionPane

class EditorCCAnnotationsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### displayHTMLAnnotations

```
JCheckBox displayHTMLAnnotations
```

##### preferCustomOxyCommehtsForDTDAnnotations

```
JCheckBox preferCustomOxyCommehtsForDTDAnnotations
```

##### showAnnotations

```
JCheckBox showAnnotations
```

##### showAnnotationsAsTooltips

```
JCheckBox showAnnotationsAsTooltips
```

##### useAllRelaxNGAnnotationsAsDocumentation

```
JCheckBox useAllRelaxNGAnnotationsAsDocumentation
```

### Class ro.sync.exml.options.EditorCCJSONOptionPane

class EditorCCJSONOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### generateAdditionalProps

```
JCheckBox generateAdditionalProps
```

##### generateOptionalProps

```
JCheckBox generateOptionalProps
```

##### generateRequiredContent

```
JCheckBox generateRequiredContent
```

### Class ro.sync.exml.options.EditorCCJSOptionPane

class EditorCCJSOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### labelUD

```
JLabel labelUD
```

##### uriTablePanel

```
ro.sync.exml.options.common.URITablePanel uriTablePanel
```

##### useBuiltinJSCheck

```
JCheckBox useBuiltinJSCheck
```

##### useCCCheck

```
JCheckBox useCCCheck
```

### Class ro.sync.exml.options.EditorCCOptionPaneGroup

class EditorCCOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### activationDelayField

```
ro.sync.ui.UndoableTextField activationDelayField
```

##### addFirstChoice

```
JCheckBox addFirstChoice
```

##### addGuessElementsCheck

```
JCheckBox addGuessElementsCheck
```

##### addOptionalContent

```
JCheckBox addOptionalContent
```

##### autocloseLastOpenedTag

```
JCheckBox autocloseLastOpenedTag
```

##### caseSensitiveTagInsightCheck

```
JCheckBox caseSensitiveTagInsightCheck
```

##### closeTheInsertedElementCheck

```
JCheckBox closeTheInsertedElementCheck
```

##### considerNextSiblingsCheck

```
JCheckBox considerNextSiblingsCheck
```

##### cursorBetweenTags

```
JCheckBox cursorBetweenTags
```

##### insFixedAttrCheck

```
JCheckBox insFixedAttrCheck
```

##### insReqAttrCheck

```
JCheckBox insReqAttrCheck
```

##### learnAttsValues

```
JCheckBox learnAttsValues
```

##### learnOnOpen

```
JCheckBox learnOnOpen
```

##### learnWords

```
JCheckBox learnWords
```

##### maximumNumberOfItems

```
JComboBox maximumNumberOfItems
```

##### notIfMathingTagFoundCheck

```
JCheckBox notIfMathingTagFoundCheck
```

##### renameMatchingTag

```
JCheckBox renameMatchingTag
```

##### showEntities

```
JCheckBox showEntities
```

##### showRecentlyUsedItems

```
JCheckBox showRecentlyUsedItems
```

##### useCCCheck

```
JCheckBox useCCCheck
```

### Class ro.sync.exml.options.EditorCCXPathOptionPane

class EditorCCXPathOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### enableXPathCC

```
JCheckBox enableXPathCC
```

##### fsWindowBackgroundColorButton

```
ro.sync.exml.options.ColorButton fsWindowBackgroundColorButton
```

##### fsWindowForegroundColorButton

```
ro.sync.exml.options.ColorButton fsWindowForegroundColorButton
```

##### includeAxes

```
JCheckBox includeAxes
```

##### includeXPathFunctions

```
JCheckBox includeXPathFunctions
```

##### includeXSLTFunctions

```
JCheckBox includeXSLTFunctions
```

##### showFunctionsSignatures

```
JCheckBox showFunctionsSignatures
```

### Class ro.sync.exml.options.EditorCCXSDOptionPane

class EditorCCXSDOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### noneRB

```
JRadioButton noneRB
```

##### schemaPanel

```
ro.sync.exml.options.ChooseXSDPanel schemaPanel
```

##### schematron15RB

```
JRadioButton schematron15RB
```

##### schematronISORB

```
JRadioButton schematronISORB
```

##### userDefinedRB

```
JRadioButton userDefinedRB
```

### Class ro.sync.exml.options.EditorCCXSLOptionPane

class EditorCCXSLOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### builtinDocSchemaRadio

```
JRadioButton builtinDocSchemaRadio
```

##### ccSchemaAndDTDPanel

```
ro.sync.exml.options.SchemaAndDTDPanel ccSchemaAndDTDPanel
```

##### customDocSchemaRadio

```
JRadioButton customDocSchemaRadio
```

##### detectXhtmlFO

```
JCheckBox detectXhtmlFO
```

##### docSchemaURLPanel

```
ro.sync.exml.options.SchemaAndDTDPanel docSchemaURLPanel
```

##### fopRB

```
JRadioButton fopRB
```

##### htmlRB

```
JRadioButton htmlRB
```

##### noneRB

```
JRadioButton noneRB
```

##### userDefinedRB

```
JRadioButton userDefinedRB
```

### Class ro.sync.exml.options.EditorCCYAMLOptionPane

class EditorCCYAMLOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### generateAdditionalProps

```
JCheckBox generateAdditionalProps
```

##### generateOptionalProps

```
JCheckBox generateOptionalProps
```

##### generateRequiredContent

```
JCheckBox generateRequiredContent
```

##### propValuesCombo

```
JComboBox<Object> propValuesCombo
```

##### propValuesLabel

```
JLabel propValuesLabel
```

### Class ro.sync.exml.options.EditorDiagramOptionPane

class EditorDiagramOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### diagramPosition

```
JComboBox diagramPosition
```

##### enableNVDLDiagramViews

```
JCheckBox enableNVDLDiagramViews
```

##### enableRNGDiagramViews

```
JCheckBox enableRNGDiagramViews
```

##### enableXSDDiagramViews

```
JCheckBox enableXSDDiagramViews
```

##### showNVDLDiagram

```
JCheckBox showNVDLDiagram
```

##### showRNGDiagram

```
JCheckBox showRNGDiagram
```

### Class ro.sync.exml.options.EditorDocumentValidationPaneGroup

class EditorDocumentValidationPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### alwaysShowValidationStatus

```
JCheckBox alwaysShowValidationStatus
```

##### maxNumberOfErrorMarkers

```
ro.sync.ui.UndoableTextField maxNumberOfErrorMarkers
```

##### validationAsYouType

```
JCheckBox validationAsYouType
```

##### validationDelay

```
ro.sync.ui.UndoableTextField validationDelay
```

##### validationErrorHighlightColorButton

```
ro.sync.exml.options.ColorButton validationErrorHighlightColorButton
```

##### validationFatalErrorHighlightColorButton

```
ro.sync.exml.options.ColorButton validationFatalErrorHighlightColorButton
```

##### validationInfoHighlightColorButton

```
ro.sync.exml.options.ColorButton validationInfoHighlightColorButton
```

##### validationSuccessColorButton

```
ro.sync.exml.options.ColorButton validationSuccessColorButton
```

##### validationWarningHighlightColorButton

```
ro.sync.exml.options.ColorButton validationWarningHighlightColorButton
```

### Class ro.sync.exml.options.EditorFormatCSSOptionPane

class EditorFormatCSSOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### addNewLineBetweenClassesCheck

```
JCheckBox addNewLineBetweenClassesCheck
```

##### addSpaceBeforePropertyValueCheck

```
JCheckBox addSpaceBeforePropertyValueCheck
```

##### classBodyOnNewLineCheck

```
JCheckBox classBodyOnNewLineCheck
```

##### formatEmbeddedCSS

```
JCheckBox formatEmbeddedCSS
```

##### indentClassContentCheck

```
JCheckBox indentClassContentCheck
```

##### preserveEmptyLinesCheck

```
JCheckBox preserveEmptyLinesCheck
```

### Class ro.sync.exml.options.EditorFormatJSONOptionPane

class EditorFormatJSONOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### sortKeysCheck

```
JCheckBox sortKeysCheck
```

### Class ro.sync.exml.options.EditorFormatJSOptionPane

class EditorFormatJSOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### formatEmbeddedJS

```
JCheckBox formatEmbeddedJS
```

##### preserveEmptyLineCheck

```
JCheckBox preserveEmptyLineCheck
```

##### putStartBraceOnNewLineCheck

```
JCheckBox putStartBraceOnNewLineCheck
```

### Class ro.sync.exml.options.EditorFormatOptionPaneGroup

class EditorFormatOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### clearUndoBeforePPCheck

```
JCheckBox clearUndoBeforePPCheck
```

##### detectIndentOptionsCheck

```
JCheckBox detectIndentOptionsCheck
```

##### detectLineWidthCheck

```
JCheckBox detectLineWidthCheck
```

##### enableZeroIndentFormatting

```
JCheckBox enableZeroIndentFormatting
```

##### formatOnOpen

```
JCheckBox formatOnOpen
```

##### indentOnEnter

```
JCheckBox indentOnEnter
```

##### indentSizeCombo

```
JComboBox indentSizeCombo
```

##### lineWidthCombo

```
JComboBox lineWidthCombo
```

##### useHardWrap

```
JCheckBox useHardWrap
```

##### useSmartEnter

```
JCheckBox useSmartEnter
```

##### useTabsCheck

```
JCheckBox useTabsCheck
```

### Class ro.sync.exml.options.EditorFormatWhitespaceOptionPane

class EditorFormatWhitespaceOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### wsTable

```
ro.sync.ui.application.ApplicationTable wsTable
```

##### wsTableModel

```
ro.sync.exml.options.EditorFormatWhitespaceOptionPane.WhitespaceTableModel wsTableModel
```

### Class ro.sync.exml.options.EditorFormatXMLOptionPane

class EditorFormatXMLOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### addSpaceBeforeClosingEmptyCheck

```
JCheckBox addSpaceBeforeClosingEmptyCheck
```

##### breakLineBeforeAttributeCheck

```
JCheckBox breakLineBeforeAttributeCheck
```

##### breakLinesEditablePanel

```
ro.sync.exml.options.EditorFormatXMLOptionPane.BreakLinesEditablePanel breakLinesEditablePanel
```

##### breakLongAttributesCheck

```
JCheckBox breakLongAttributesCheck
```

##### expandEmptyElementsCheck

```
JCheckBox expandEmptyElementsCheck
```

##### indentInlineElems

```
JCheckBox indentInlineElems
```

##### indentInPreserveSpaceCheck

```
JCheckBox indentInPreserveSpaceCheck
```

##### indentOnPaste

```
JCheckBox indentOnPaste
```

##### preserveEmptyLinesCheck

```
JCheckBox preserveEmptyLinesCheck
```

##### preserveLineBreaksInAttrsValues

```
JCheckBox preserveLineBreaksInAttrsValues
```

##### preserveMixed

```
ro.sync.exml.options.ListEditorPanel preserveMixed
```

##### preservePanel

```
ro.sync.exml.options.ListEditorPanel preservePanel
```

##### preserveTextAsItIsCheck

```
JCheckBox preserveTextAsItIsCheck
```

##### schemaAwareIndentCheck

```
JCheckBox schemaAwareIndentCheck
```

##### sortAttributesCheck

```
JCheckBox sortAttributesCheck
```

##### stripPanel

```
ro.sync.exml.options.ListEditorPanel stripPanel
```

### Class ro.sync.exml.options.EditorFormatXPathOptionPane

class EditorFormatXPathOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### formatEmbeddedXPath

```
JCheckBox formatEmbeddedXPath
```

### Class ro.sync.exml.options.EditorFormatXQueryOptionPane

class EditorFormatXQueryOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### breakLineBeforeAttributeCheck

```
JCheckBox breakLineBeforeAttributeCheck
```

##### preserveLineBreaksCheck

```
JCheckBox preserveLineBreaksCheck
```

### Class ro.sync.exml.options.EditorOpenOptionPane

class EditorOpenOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### askForEachDocButton

```
JRadioButton askForEachDocButton
```

##### bidiLimitCheck

```
JCheckBox bidiLimitCheck
```

##### bidiLimitCombo

```
JComboBox bidiLimitCombo
```

##### disableBIDISupportButton

```
JRadioButton disableBIDISupportButton
```

##### editorLineLimit

```
ro.sync.ui.UndoableTextField editorLineLimit
```

##### editorLineLimitCheck

```
JCheckBox editorLineLimitCheck
```

##### enableBIDISupportButton

```
JRadioButton enableBIDISupportButton
```

##### lockLocalResourcesForEditing

```
JCheckBox lockLocalResourcesForEditing
```

##### openEachEditorNextToCurrent

```
JCheckBox openEachEditorNextToCurrent
```

##### optimizeLoadFileSizeCombo

```
JComboBox optimizeLoadFileSizeCombo
```

##### restoreCursorPositionCheck

```
JCheckBox restoreCursorPositionCheck
```

##### showLoadLargeDocumentsInfo

```
JCheckBox showLoadLargeDocumentsInfo
```

### Class ro.sync.exml.options.EditorOptionPaneGroup

class EditorOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### canEditReadOnlyFiles

```
JCheckBox canEditReadOnlyFiles
```

##### ccDocWindowBackgroundColorButton

```
ro.sync.exml.options.ColorButton ccDocWindowBackgroundColorButton
```

##### ccDocWindowForegroundColorButton

```
ro.sync.exml.options.ColorButton ccDocWindowForegroundColorButton
```

##### ccWindowBackgroundColorButton

```
ro.sync.exml.options.ColorButton ccWindowBackgroundColorButton
```

##### ccWindowForegroundColorButton

```
ro.sync.exml.options.ColorButton ccWindowForegroundColorButton
```

##### displayQuickAssistHint

```
JCheckBox displayQuickAssistHint
```

##### enableMouseWheelZooming

```
JCheckBox enableMouseWheelZooming
```

##### findHighlightsColorButton

```
ro.sync.exml.options.ColorButton findHighlightsColorButton
```

##### marksColorButton

```
ro.sync.exml.options.ColorButton marksColorButton
```

##### maxNoOfHighlightsFiled

```
ro.sync.ui.UndoableTextField maxNoOfHighlightsFiled
```

##### searchDeclHighlightsColorButton

```
ro.sync.exml.options.ColorButton searchDeclHighlightsColorButton
```

##### searchRefHighlightsColorButton

```
ro.sync.exml.options.ColorButton searchRefHighlightsColorButton
```

##### selectionBackgroundColorButton

```
ro.sync.exml.options.ColorButton selectionBackgroundColorButton
```

##### selectionForegroundColorButton

```
ro.sync.exml.options.ColorButton selectionForegroundColorButton
```

##### showEOL_EOFCheck

```
JCheckBox showEOL_EOFCheck
```

##### showSpacesCheck

```
JCheckBox showSpacesCheck
```

##### undoHistorySizeTextField

```
ro.sync.ui.UndoableTextField undoHistorySizeTextField
```

##### xPathHighlightsColorButton

```
ro.sync.exml.options.ColorButton xPathHighlightsColorButton
```

### Class ro.sync.exml.options.EditorPageAssociationsPanel

class EditorPageAssociationsPanel extends ro.sync.ui.table.EditableSortableTablePanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### model

```
ro.sync.exml.options.EditorPageAssociationsPanel.EditorPageTableModel model
```

### Class ro.sync.exml.options.EditorPageAssociationsPanel.EditorPageTableModel

class EditorPageTableModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### editorPageAssociation

```
List<ro.sync.exml.editor.EditorPageAssociation> editorPageAssociation
```

### Class ro.sync.exml.options.EditorPrintOptionPane

class EditorPrintOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### footerColor

```
ro.sync.exml.options.ColorButton footerColor
```

##### footerFontButton

```
ro.sync.exml.options.common.FontPanel footerFontButton
```

##### footerLeft

```
ro.sync.ui.UndoableTextField footerLeft
```

##### footerMiddle

```
ro.sync.ui.UndoableTextField footerMiddle
```

##### footerOverline

```
JCheckBox footerOverline
```

##### footerRight

```
ro.sync.ui.UndoableTextField footerRight
```

##### headerColor

```
ro.sync.exml.options.ColorButton headerColor
```

##### headerFontButton

```
ro.sync.exml.options.common.FontPanel headerFontButton
```

##### headerLeft

```
ro.sync.ui.UndoableTextField headerLeft
```

##### headerMiddle

```
ro.sync.ui.UndoableTextField headerMiddle
```

##### headerRight

```
ro.sync.ui.UndoableTextField headerRight
```

##### headerUnderline

```
JCheckBox headerUnderline
```

### Class ro.sync.exml.options.EditorSaveOptionPane

class EditorSaveOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### autoRecoveryIntervalCombo

```
JComboBox autoRecoveryIntervalCombo
```

##### autoRecoveryLocationPanel

```
JPanel autoRecoveryLocationPanel
```

##### autoRecoveryLocationTextField

```
ro.sync.ui.UndoableTextField autoRecoveryLocationTextField
```

##### autosaveIntervalCombo

```
JComboBox autosaveIntervalCombo
```

##### backupExtensionField

```
ro.sync.ui.UndoableTextField backupExtensionField
```

##### checkValidateBeforeSave

```
JCheckBox checkValidateBeforeSave
```

##### clearUndoOnSaveCheck

```
JCheckBox clearUndoOnSaveCheck
```

##### compileLessOnSave

```
JCheckBox compileLessOnSave
```

##### enableAutoRecoveryCheckBox

```
JCheckBox enableAutoRecoveryCheckBox
```

##### enableAutosaveCheckBox

```
JCheckBox enableAutosaveCheckBox
```

##### enableSaveAsInNewDlgCheck

```
JCheckBox enableSaveAsInNewDlgCheck
```

##### makeBackupCheck

```
JCheckBox makeBackupCheck
```

##### safeSaveCheck

```
JCheckBox safeSaveCheck
```

##### saveAllBeforeTransformationOrValidation

```
JCheckBox saveAllBeforeTransformationOrValidation
```

##### saveCurrentFileBeforeCallingExternalTool

```
JCheckBox saveCurrentFileBeforeCallingExternalTool
```

### Class ro.sync.exml.options.EmptyOptionPaneGroup

class EmptyOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.ExistXMLDatabaseOptionPane

class ExistXMLDatabaseOptionPane extends ro.sync.exml.options.DBSourceConfiguratorBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### baseUriTextField

```
ro.sync.ui.UndoableTextField baseUriTextField
```

##### currentCollection

```
ro.sync.ui.UndoableTextField currentCollection
```

##### driver

```
ro.sync.db.core.DBSourceDriverInfo driver
```

##### passwordTextField

```
ro.sync.ui.application.ApplicationPasswordField passwordTextField
```

##### usernameTextField

```
ro.sync.ui.UndoableTextField usernameTextField
```

##### useSSL

```
JCheckBox useSSL
```

### Class ro.sync.exml.options.ExternalPOTestClass

class ExternalPOTestClass extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### location

```
URL location
```

##### name

```
String name
```

##### notPersistent

```
String notPersistent
```

### Class ro.sync.exml.options.ExternalToolsOptionPane

class ExternalToolsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### editor

```
ro.sync.cmdline.CmdLinesEditor editor
```

### Class ro.sync.exml.options.FOProcessorsOptionPane

class FOProcessorsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### apacheFopInputPanel

```
ro.sync.ui.InputFilePanel apacheFopInputPanel
```

##### browseConfigurationAction

```
ro.sync.ui.application.action.TaggedAction browseConfigurationAction
```

##### configurationFilePathField

```
ro.sync.ui.UndoableTextField configurationFilePathField
```

##### editor

```
ro.sync.cmdline.CmdLinesEditor editor
```

##### enableInternalFopOutputCheck

```
JCheckBox enableInternalFopOutputCheck
```

##### enablePDFA_1bCheck

```
JCheckBox enablePDFA_1bCheck
```

##### fopMemoryCombo

```
JComboBox fopMemoryCombo
```

##### useBuilInApacheFOP

```
JRadioButton useBuilInApacheFOP
```

##### useOtherApacheFOP

```
JRadioButton useOtherApacheFOP
```

### Class ro.sync.exml.options.ForbiddenCharsDocument

class ForbiddenCharsDocument extends ro.sync.document.OxygenPlainDocument implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.GridEditorOptionPane

class GridEditorOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### borderColorButton

```
ro.sync.exml.options.ColorButton borderColorButton
```

##### chCurrentSelectedEnd1ColorButton

```
ro.sync.exml.options.ColorButton chCurrentSelectedEnd1ColorButton
```

##### chCurrentSelectedEnd2ColorButton

```
ro.sync.exml.options.ColorButton chCurrentSelectedEnd2ColorButton
```

##### chCurrentSelectedStart1ColorButton

```
ro.sync.exml.options.ColorButton chCurrentSelectedStart1ColorButton
```

##### chCurrentSelectedStart2ColorButton

```
ro.sync.exml.options.ColorButton chCurrentSelectedStart2ColorButton
```

##### chPreviewCurrentSelectedIcon

```
ro.sync.exml.options.GridEditorOptionPane.IconPainterPanel chPreviewCurrentSelectedIcon
```

##### chPreviewSelectedIcon

```
ro.sync.exml.options.GridEditorOptionPane.IconPainterPanel chPreviewSelectedIcon
```

##### chPreviewUnselectedIcon

```
ro.sync.exml.options.GridEditorOptionPane.IconPainterPanel chPreviewUnselectedIcon
```

##### chSelectedEnd1ColorButton

```
ro.sync.exml.options.ColorButton chSelectedEnd1ColorButton
```

##### chSelectedEnd2ColorButton

```
ro.sync.exml.options.ColorButton chSelectedEnd2ColorButton
```

##### chSelectedStart1ColorButton

```
ro.sync.exml.options.ColorButton chSelectedStart1ColorButton
```

##### chSelectedStart2ColorButton

```
ro.sync.exml.options.ColorButton chSelectedStart2ColorButton
```

##### chUnselectedEnd1ColorButton

```
ro.sync.exml.options.ColorButton chUnselectedEnd1ColorButton
```

##### chUnselectedEnd2ColorButton

```
ro.sync.exml.options.ColorButton chUnselectedEnd2ColorButton
```

##### chUnselectedStart1ColorButton

```
ro.sync.exml.options.ColorButton chUnselectedStart1ColorButton
```

##### chUnselectedStart2ColorButton

```
ro.sync.exml.options.ColorButton chUnselectedStart2ColorButton
```

##### compactRepresentation

```
JCheckBox compactRepresentation
```

##### currentlySelectionColorButton

```
ro.sync.exml.options.ColorButton currentlySelectionColorButton
```

##### defaultColsWidthTextField

```
ro.sync.ui.UndoableTextField defaultColsWidthTextField
```

##### gridBackgroundColorButton

```
ro.sync.exml.options.ColorButton gridBackgroundColorButton
```

##### gridForegroundColorButton

```
ro.sync.exml.options.ColorButton gridForegroundColorButton
```

##### prettyPrintContent

```
JCheckBox prettyPrintContent
```

##### rowCurrentSelectedColorButton

```
ro.sync.exml.options.ColorButton rowCurrentSelectedColorButton
```

##### rowSelectedColorButton

```
ro.sync.exml.options.ColorButton rowSelectedColorButton
```

##### rowUnselectedColorButton

```
ro.sync.exml.options.ColorButton rowUnselectedColorButton
```

##### selectionColorButton

```
ro.sync.exml.options.ColorButton selectionColorButton
```

### Class ro.sync.exml.options.HostsTableModel

class HostsTableModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### trustedHosts

```
List<String> trustedHosts
```

### Class ro.sync.exml.options.IgnoredValidationProblemsOptionPane

class IgnoredValidationProblemsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### ignoredProblemsPanel

```
ro.sync.exml.options.IgnoredValidationProblemsPanel ignoredProblemsPanel
```

##### ignoreProblemsSupportCheckBox

```
JCheckBox ignoreProblemsSupportCheckBox
```

### Class ro.sync.exml.options.IgnoredValidationProblemsPanel

class IgnoredValidationProblemsPanel extends ro.sync.ui.table.EditableSortableTablePanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### ignoreProblemsSupportCheckBox

```
JCheckBox ignoreProblemsSupportCheckBox
```

##### model

```
ro.sync.exml.options.IgnoredValidationProblemsPanel.IgnoredValidationProblemsTableModel model
```

### Class ro.sync.exml.options.IgnoredValidationProblemsPanel.IgnoredValidationProblemsTableModel

class IgnoredValidationProblemsTableModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### data

```
List<ro.sync.quickfix.generic.IgnoredProblemPO> data
```

### Class ro.sync.exml.options.JSONSchemaEditorPropertiesOptionPane

class JSONSchemaEditorPropertiesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### showAdditionalPropertiesInViews

```
JCheckBox showAdditionalPropertiesInViews
```

##### treeTable

```
ro.sync.ui.treetable.ApplicationTreeTable treeTable
```

### Class ro.sync.exml.options.LegacyProperties

class LegacyProperties extends [Properties](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Properties.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.ListEditorPanel

class ListEditorPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### addButton

```
JButton addButton
```

##### dialogTitle

```
String dialogTitle
```

##### examplelist

```
String examplelist
```

##### list

```
JList list
```

##### model

```
DefaultListModel model
```

##### removeButton

```
JButton removeButton
```

##### userMessage

```
String userMessage
```

### Class ro.sync.exml.options.MapsOptionsPane

class MapsOptionsPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### alwaysNavigateToNextDocument

```
JRadioButton alwaysNavigateToNextDocument
```

##### alwaysOpenDitaManagerButton

```
JRadioButton alwaysOpenDitaManagerButton
```

##### askWhenNavigateToNextDocument

```
JRadioButton askWhenNavigateToNextDocument
```

##### askWhenOpenDitaManagerButton

```
JRadioButton askWhenOpenDitaManagerButton
```

##### ditaMapPatterns

```
ro.sync.ui.UndoableTextField ditaMapPatterns
```

##### doNothingWhenNavigatingToNextDocument

```
JRadioButton doNothingWhenNavigatingToNextDocument
```

##### editResolvedReferredContent

```
JCheckBox editResolvedReferredContent
```

##### enableAutosaveCheckBox

```
JCheckBox enableAutosaveCheckBox
```

##### enableDynamicConversion

```
JCheckBox enableDynamicConversion
```

##### expandMapReferencesInAuthorPage

```
JCheckBox expandMapReferencesInAuthorPage
```

##### navTitleAttrForTitleRendition

```
JCheckBox navTitleAttrForTitleRendition
```

##### neverOpenDitaManagerButton

```
JRadioButton neverOpenDitaManagerButton
```

##### preferAddingKeyrefToRefRes

```
JCheckBox preferAddingKeyrefToRefRes
```

##### presentOnlyItemsRelatedToOpenMaps

```
JCheckBox presentOnlyItemsRelatedToOpenMaps
```

##### restrictEditingReferredContentToLocalFiles

```
JCheckBox restrictEditingReferredContentToLocalFiles
```

##### topicRefFormatCheckbox

```
JCheckBox topicRefFormatCheckbox
```

##### topicRefNavtitleCheckbox

```
JCheckBox topicRefNavtitleCheckbox
```

##### topicRefScopeCheckbox

```
JCheckBox topicRefScopeCheckbox
```

##### topicRefTypeCheckbox

```
JCheckBox topicRefTypeCheckbox
```

##### usedFromOxygen

```
boolean usedFromOxygen
```

##### useFilenameForTopicrefKeysAttr

```
JCheckBox useFilenameForTopicrefKeysAttr
```

### Class ro.sync.exml.options.MarkdownOptionPane

class MarkdownOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### enableComments

```
JCheckBox enableComments
```

### Class ro.sync.exml.options.MarkLogicDatabaseOptionPane

class MarkLogicDatabaseOptionPane extends ro.sync.exml.options.DBSourceConfiguratorBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### databaseTextField

```
ro.sync.ui.UndoableTextField databaseTextField
```

##### driver

```
ro.sync.db.core.DBSourceDriverInfo driver
```

##### hostTextField

```
ro.sync.ui.UndoableTextField hostTextField
```

##### passwordTextField

```
ro.sync.ui.application.ApplicationPasswordField passwordTextField
```

##### portTextField

```
ro.sync.ui.UndoableTextField portTextField
```

##### usernameTextField

```
ro.sync.ui.UndoableTextField usernameTextField
```

##### webdavTextField

```
ro.sync.ui.UndoableTextField webdavTextField
```

### Class ro.sync.exml.options.MarkOccurrencesOptionPane

class MarkOccurrencesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### colorPanel

```
JPanel colorPanel
```

##### declarationColorButton

```
ro.sync.exml.options.ColorButton declarationColorButton
```

##### enableHighlightInAnt

```
JCheckBox enableHighlightInAnt
```

##### enableHighlightInRNG

```
JCheckBox enableHighlightInRNG
```

##### enableHighlightInSchematron

```
JCheckBox enableHighlightInSchematron
```

##### enableHighlightInWSDL

```
JCheckBox enableHighlightInWSDL
```

##### enableHighlightInXML

```
JCheckBox enableHighlightInXML
```

##### enableHighlightInXsd

```
JCheckBox enableHighlightInXsd
```

##### enableHighlightInXSL

```
JCheckBox enableHighlightInXSL
```

##### referenceColorButton

```
ro.sync.exml.options.ColorButton referenceColorButton
```

### Class ro.sync.exml.options.MasterFilesOptionPane

class MasterFilesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.MessagesOptionPane

class MessagesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### alwaysAsk

```
JRadioButton alwaysAsk
```

##### alwaysExpand

```
JRadioButton alwaysExpand
```

##### dontExpand

```
JRadioButton dontExpand
```

##### promptWhenMoveResources

```
JCheckBox promptWhenMoveResources
```

##### showAddedToProjectWarningDialog

```
JCheckBox showAddedToProjectWarningDialog
```

##### showBIDIWarning

```
JCheckBox showBIDIWarning
```

##### showChangeOrientationWarnCheck

```
JCheckBox showChangeOrientationWarnCheck
```

##### showChooseEncodingForConversionsDialog

```
JCheckBox showChooseEncodingForConversionsDialog
```

##### showJavaVendorWarning

```
JCheckBox showJavaVendorWarning
```

##### showMathMLEditorRecommendation

```
JCheckBox showMathMLEditorRecommendation
```

##### showSaveDlgWhenMergingFilesManually

```
JCheckBox showSaveDlgWhenMergingFilesManually
```

##### showSFTPDialog

```
JCheckBox showSFTPDialog
```

##### showSharePointEnterpriseLicenseMessage

```
JCheckBox showSharePointEnterpriseLicenseMessage
```

##### showSwitchToDITAPersp

```
JCheckBox showSwitchToDITAPersp
```

##### showXPathBuilderWarningCheck

```
JCheckBox showXPathBuilderWarningCheck
```

### Class ro.sync.exml.options.OpenFindResourceIndexingOptions

class OpenFindResourceIndexingOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### ignoredContentFilesPatterns

```
String ignoredContentFilesPatterns
```

##### includedContentBinaryFilesPatterns

```
String includedContentBinaryFilesPatterns
```

##### indexRemoteResourcesContent

```
boolean indexRemoteResourcesContent
```

##### lang

```
String lang
```

##### searchInContent

```
boolean searchInContent
```

##### stopWords

```
String stopWords
```

##### xmlAware

```
boolean xmlAware
```

##### xmlAwareContentSizeLimit

```
int xmlAwareContentSizeLimit
```

### Class ro.sync.exml.options.OpenFindResourceOptionPane

class OpenFindResourceOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### exactMatches

```
JRadioButton exactMatches
```

##### ignoredFilesFilter

```
ro.sync.ui.UndoableTextField ignoredFilesFilter
```

##### includedBinaryFilesFilter

```
ro.sync.ui.UndoableTextField includedBinaryFilesFilter
```

##### indexContentOfOpenedMaps

```
JCheckBox indexContentOfOpenedMaps
```

##### indexOnlyResourceOnlyTopics

```
JCheckBox indexOnlyResourceOnlyTopics
```

##### indexRemoteContents

```
JCheckBox indexRemoteContents
```

##### langCombo

```
JComboBox langCombo
```

##### maximumHitsNumberCombo

```
ro.sync.ui.application.ApplicationComboBox maximumHitsNumberCombo
```

##### operatorCombo

```
ro.sync.ui.application.ApplicationComboBox operatorCombo
```

##### prefixMatches

```
JRadioButton prefixMatches
```

##### searchInContents

```
JCheckBox searchInContents
```

##### stopWordsArea

```
ro.sync.ui.application.ApplicationTextArea stopWordsArea
```

##### toEnableDisable

```
List<JComponent> toEnableDisable
```

##### xmlAware

```
JCheckBox xmlAware
```

##### xmlAwareContentSizeLimit

```
ro.sync.ui.UndoableTextField xmlAwareContentSizeLimit
```

### Class ro.sync.exml.options.OpenFindResourceSearchingOptions

class OpenFindResourceSearchingOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### exactMatches

```
boolean exactMatches
```

##### maximumHitsNumber

```
int maximumHitsNumber
```

##### usingAndAsDefaultJoinOperator

```
boolean usingAndAsDefaultJoinOperator
```

### Class ro.sync.exml.options.OutlineOptionPane

class OutlineOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### attrNamesPanel

```
ro.sync.exml.options.AttributeNamesEditorPanel attrNamesPanel
```

##### enableOutlineDnD

```
JCheckBox enableOutlineDnD
```

### Class ro.sync.exml.options.OxygenArchiveOptionPane

class OxygenArchiveOptionPane extends ro.sync.exml.options.common.ArchiveOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.OxygenEncodingOptionPane

class OxygenEncodingOptionPane extends ro.sync.exml.options.common.EncodingOptionPaneBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.OxygenFileTypesOptionPane

class OxygenFileTypesOptionPane extends ro.sync.exml.options.common.FileTypesOptionPaneBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.OxygenFontsOptionPane

class OxygenFontsOptionPane extends ro.sync.exml.options.common.FontsOptionPaneBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.OxygenMenuShorcutKeysOptionPane

class OxygenMenuShorcutKeysOptionPane extends ro.sync.exml.options.common.MenuShorcutKeysOptionPaneBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.PageOptionsMapping

class PageOptionsMapping extends [HashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/HashMap.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.PagesOptionPaneGroup

class PagesOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allowDTPageOverride

```
JCheckBox allowDTPageOverride
```

##### editorPageAssociationsPanel

```
ro.sync.exml.options.EditorPageAssociationsPanel editorPageAssociationsPanel
```

### Class ro.sync.exml.options.PerspectivesLayoutInfo

class PerspectivesLayoutInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### predefinedLayout

```
boolean predefinedLayout
```

##### predefinedLayoutName

```
String predefinedLayoutName
```

##### specifiedLayoutPath

```
String specifiedLayoutPath
```

##### useFixedLayout

```
boolean useFixedLayout
```

### Class ro.sync.exml.options.PluginCellRenderer

class PluginCellRenderer extends [DefaultTableCellRenderer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/DefaultTableCellRenderer.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.PluginsOptionPane

class PluginsOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### addonExtensionsManager

```
ro.sync.exml.addons.ExtensionsManager addonExtensionsManager
```

##### pluginArea

```
ro.sync.ui.application.ApplicationEditorPane pluginArea
```

##### pluginTable

```
ro.sync.ui.application.ApplicationTable pluginTable
```

### Class ro.sync.exml.options.ProfilerOptionPane

class ProfilerOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### hotSpotThreshold

```
ro.sync.ui.UndoableTextField hotSpotThreshold
```

##### ignoreInvocationLessThan

```
ro.sync.ui.UndoableTextField ignoreInvocationLessThan
```

##### microseconds

```
JRadioButton microseconds
```

##### miliseconds

```
JRadioButton miliseconds
```

##### percentageAbsolute

```
JRadioButton percentageAbsolute
```

##### percentageRelative

```
JRadioButton percentageRelative
```

##### showInherentTime

```
JCheckBox showInherentTime
```

##### showInvocationCount

```
JCheckBox showInvocationCount
```

##### showTime

```
JCheckBox showTime
```

### Class ro.sync.exml.options.RelaxNGOptionPane

class RelaxNGOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### checkFeasiblyValid

```
JCheckBox checkFeasiblyValid
```

##### checkIdIdref

```
JCheckBox checkIdIdref
```

##### relaxNGDefaults

```
JCheckBox relaxNGDefaults
```

##### skipDataAttrs

```
JCheckBox skipDataAttrs
```

### Class ro.sync.exml.options.SchemaAndDTDPanel

class SchemaAndDTDPanel extends ro.sync.ui.InputUrlPanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.exml.options.SchemaEditorOptionPane

class SchemaEditorOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### alwaysAskRadioButton

```
JRadioButton alwaysAskRadioButton
```

##### diagramZoomCombo

```
JComboBox diagramZoomCombo
```

##### noRadioButton

```
JRadioButton noRadioButton
```

##### showDocumentationInSchema

```
JCheckBox showDocumentationInSchema
```

##### yesRadioButton

```
JRadioButton yesRadioButton
```

### Class ro.sync.exml.options.SchematronOptionPane

class SchematronOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allLangRadio

```
JRadioButton allLangRadio
```

##### allowForeign

```
JCheckBox allowForeign
```

##### applicationLangRadio

```
JRadioButton applicationLangRadio
```

##### considerOnlyDefaultQFs

```
JCheckBox considerOnlyDefaultQFs
```

##### customLangCombo

```
JComboBox customLangCombo
```

##### customLangRadio

```
JRadioButton customLangRadio
```

##### disableSecurityButton

```
JCheckBox disableSecurityButton
```

##### enableSQFSupport

```
JCheckBox enableSQFSupport
```

##### queryBindingXslt1Button

```
JRadioButton queryBindingXslt1Button
```

##### queryBindingXslt2Button

```
JRadioButton queryBindingXslt2Button
```

##### queryBindingXslt3Button

```
JRadioButton queryBindingXslt3Button
```

##### schemaLangRadio

```
JRadioButton schemaLangRadio
```

##### useISOSchematronDefaultSchemaAttrs

```
JCheckBox useISOSchematronDefaultSchemaAttrs
```

##### useISOSchematronWithXSLT2QueryBindings

```
JCheckBox useISOSchematronWithXSLT2QueryBindings
```

##### useXPath10Button

```
JRadioButton useXPath10Button
```

##### useXPath20Button

```
JRadioButton useXPath20Button
```

##### useXPath31Button

```
JRadioButton useXPath31Button
```

##### visitNoAttributes

```
JCheckBox visitNoAttributes
```

### Class ro.sync.exml.options.SecretsOptionPane

class SecretsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### secretsPanel

```
ro.sync.exml.options.SecretsPanel secretsPanel
```

### Class ro.sync.exml.options.SecretsPanel

class SecretsPanel extends ro.sync.ui.table.EditableSortableTablePanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### model

```
ro.sync.exml.options.SecretsTableModel model
```

### Class ro.sync.exml.options.SecretsTableModel

class SecretsTableModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### data

```
List<ro.sync.util.editorvars.UserSecretPO> data
```

### Class ro.sync.exml.options.SharePointOnlineOptionPane

class SharePointOnlineOptionPane extends ro.sync.exml.options.DBSourceConfiguratorBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### urlTextField

```
ro.sync.ui.UndoableTextFieldWithPlaceholder urlTextField
```

### Class ro.sync.exml.options.SharePointOptionPane

class SharePointOptionPane extends ro.sync.exml.options.DBSourceConfiguratorBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### domainTextField

```
ro.sync.ui.UndoableTextField domainTextField
```

##### passwordTextField

```
ro.sync.ui.application.ApplicationPasswordField passwordTextField
```

##### urlTextField

```
ro.sync.ui.UndoableTextField urlTextField
```

##### usernameTextField

```
ro.sync.ui.UndoableTextField usernameTextField
```

### Class ro.sync.exml.options.SpellCheckOptionPane

class SpellCheckOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allowCompound

```
JCheckBox allowCompound
```

##### allowFileExtensions

```
JCheckBox allowFileExtensions
```

##### autoCheckContentTypes

```
String[] autoCheckContentTypes
```

##### autocorrectOptionsPageLink

```
ro.sync.exml.LinkLabel autocorrectOptionsPageLink
```

##### automaticSpellCheck

```
JCheckBox automaticSpellCheck
```

##### checkCapitalization

```
JCheckBox checkCapitalization
```

##### checkPunctuation

```
JCheckBox checkPunctuation
```

##### dictionariesCombo

```
ro.sync.azcheck.ui.DictionaryComboBox dictionariesCombo
```

##### enableDictionariesComboUpdate

```
boolean enableDictionariesComboUpdate
```

##### honourLangAttributes

```
JCheckBox honourLangAttributes
```

##### ignoreAcronyms

```
JCheckBox ignoreAcronyms
```

##### ignoreAcronymsSelected

```
boolean ignoreAcronymsSelected
```

##### ignoreDigits

```
JCheckBox ignoreDigits
```

##### ignoreDuplicates

```
JCheckBox ignoreDuplicates
```

##### ignoreElementsPanel

```
ro.sync.exml.options.ListEditorPanel ignoreElementsPanel
```

##### ignoreMixedCase

```
JCheckBox ignoreMixedCase
```

##### ignoreURL

```
JCheckBox ignoreURL
```

##### langAttrMissingDoNotCheck

```
JRadioButton langAttrMissingDoNotCheck
```

##### langAttrMissingUseDefaultLang

```
JRadioButton langAttrMissingUseDefaultLang
```

##### spellCheckColorButton

```
ro.sync.exml.options.ColorButton spellCheckColorButton
```

##### spellCheckContentTypesButton

```
JButton spellCheckContentTypesButton
```

##### spellCheckInAttributeValues

```
JCheckBox spellCheckInAttributeValues
```

##### spellCheckInCDATA

```
JCheckBox spellCheckInCDATA
```

##### spellCheckInComments

```
JCheckBox spellCheckInComments
```

##### spellCheckInPIs

```
JCheckBox spellCheckInPIs
```

##### spellCheckInText

```
JCheckBox spellCheckInText
```

### Class ro.sync.exml.options.TextEditorOptionPane

class TextEditorOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### caretColorButton

```
ro.sync.exml.options.ColorButton caretColorButton
```

##### editorBackgroundColorButton

```
ro.sync.exml.options.ColorButton editorBackgroundColorButton
```

##### enableFoldingCheck

```
JCheckBox enableFoldingCheck
```

##### enableLineCopyWithNoSelectionCheck

```
JCheckBox enableLineCopyWithNoSelectionCheck
```

##### highlightCurrentLine

```
JCheckBox highlightCurrentLine
```

##### highlightMatchingTag

```
JCheckBox highlightMatchingTag
```

##### lineHighlightColorButton

```
ro.sync.exml.options.ColorButton lineHighlightColorButton
```

##### lineNumberForegroundColor

```
ro.sync.exml.options.ColorButton lineNumberForegroundColor
```

##### lineWrapCheck

```
JCheckBox lineWrapCheck
```

##### lockTags

```
JCheckBox lockTags
```

##### matchingTagHighlightColorButton

```
ro.sync.exml.options.ColorButton matchingTagHighlightColorButton
```

##### optionPresenter

```
ro.sync.options.IOptionDialog optionPresenter
```

##### printMarginColorButton

```
ro.sync.exml.options.ColorButton printMarginColorButton
```

##### printMarginCols

```
ro.sync.ui.UndoableTextField printMarginCols
```

##### showJSONPropertyNames

```
JCheckBox showJSONPropertyNames
```

##### showPrintMargin

```
JCheckBox showPrintMargin
```

##### showSpaceMarksForYAMLDocs

```
JCheckBox showSpaceMarksForYAMLDocs
```

##### transparencyForPropertySlider

```
JSlider transparencyForPropertySlider
```

##### useLineNumberCheck

```
JCheckBox useLineNumberCheck
```

### Class ro.sync.exml.options.TitleBasedFilenameGenerationOptions

class TitleBasedFilenameGenerationOptions extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allLowerCase

```
boolean allLowerCase
```

##### charToReplaceSpacesWith

```
String charToReplaceSpacesWith
```

##### howToGenerateFilenameFromTitle

```
int howToGenerateFilenameFromTitle
```

##### upperCaseFirstLetter

```
boolean upperCaseFirstLetter
```

### Class ro.sync.exml.options.TopicsOptionsPane

class TopicsOptionsPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allLowerCaseCheckBox

```
JCheckBox allLowerCaseCheckBox
```

##### characterTextField

```
ro.sync.ui.UndoableTextField characterTextField
```

##### errorWindow

```
ro.sync.contentcompletion.editor.CCDocumentationWindow errorWindow
```

##### linkFormatCheckbox

```
JCheckBox linkFormatCheckbox
```

##### linkScopeCheckbox

```
JCheckBox linkScopeCheckbox
```

##### linkTypeCheckbox

```
JCheckBox linkTypeCheckbox
```

##### replaceSpacesRadioBtn

```
JRadioButton replaceSpacesRadioBtn
```

##### sameTopicFragIdent

```
JCheckBox sameTopicFragIdent
```

##### uppercaseFirstLetterCheckBox

```
JCheckBox uppercaseFirstLetterCheckBox
```

##### useCamelCaseRadioBtn

```
JRadioButton useCamelCaseRadioBtn
```

##### useFilenameForRootIDCheckBox

```
JCheckBox useFilenameForRootIDCheckBox
```

##### useTitleForFileNameCheckBox

```
JCheckBox useTitleForFileNameCheckBox
```

### Class ro.sync.exml.options.TrustedHostsOptionPane

class TrustedHostsOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### tablePanel

```
ro.sync.exml.options.TrustedHostsTablePanel tablePanel
```

### Class ro.sync.exml.options.TrustedHostsTablePanel

class TrustedHostsTablePanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### deleteRowButton

```
JButton deleteRowButton
```

##### filterPanel

```
ro.sync.ui.FilterPanel filterPanel
```

##### newRowButton

```
JButton newRowButton
```

##### scPane

```
ro.sync.ui.application.ApplicationScrollPane scPane
```

##### table

```
ro.sync.ui.application.ApplicationTable table
```

##### tableModel

```
ro.sync.exml.options.HostsTableModel tableModel
```

### Class ro.sync.exml.options.ViewOptionPane

class ViewOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### enableProjectDnD

```
JCheckBox enableProjectDnD
```

##### maxNoLinesCombo

```
JComboBox maxNoLinesCombo
```

##### showOnlyAllowedItems

```
JCheckBox showOnlyAllowedItems
```

### Class ro.sync.exml.options.WebdavOptionPane

class WebdavOptionPane extends ro.sync.exml.options.DBSourceConfiguratorBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### passwordTextField

```
ro.sync.ui.application.ApplicationPasswordField passwordTextField
```

##### urlTextField

```
ro.sync.ui.UndoableTextField urlTextField
```

##### usernameTextField

```
ro.sync.ui.UndoableTextField usernameTextField
```

### Class ro.sync.exml.options.XMLCatalogOptionPane

class XMLCatalogOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### catalogsPanel

```
ro.sync.exml.options.CatalogsURITablePanel catalogsPanel
```

##### defaultCatalog

```
ro.sync.ui.UndoableTextField defaultCatalog
```

##### preferPublicRadio

```
JRadioButton preferPublicRadio
```

##### preferSystemRadio

```
JRadioButton preferSystemRadio
```

##### processNamespacesForXMLSchema

```
JCheckBox processNamespacesForXMLSchema
```

##### schemaThroughSystemMappings

```
JCheckBox schemaThroughSystemMappings
```

##### useDefaultCatalog

```
JCheckBox useDefaultCatalog
```

##### verbosityAllMessages

```
JRadioButton verbosityAllMessages
```

##### verbosityNone

```
JRadioButton verbosityNone
```

##### verbosityUnresolvedEntities

```
JRadioButton verbosityUnresolvedEntities
```

### Class ro.sync.exml.options.XmlInstanceGeneratorOptionPane

class XmlInstanceGeneratorOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### discardOptionalElementsLevel

```
ro.sync.ui.UndoableTextField discardOptionalElementsLevel
```

##### incrementNamesForDefaultValues

```
JCheckBox incrementNamesForDefaultValues
```

##### oneSettingPanel

```
ro.sync.xml.generator.OneSettingPanel oneSettingPanel
```

##### preferedMaxLengthForStrings

```
ro.sync.ui.UndoableTextField preferedMaxLengthForStrings
```

### Class ro.sync.exml.options.XMLParserOptionPane

class XMLParserOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### baseUriFixup

```
JCheckBox baseUriFixup
```

##### dtdPostValidation

```
JCheckBox dtdPostValidation
```

##### enableParserCaching

```
JCheckBox enableParserCaching
```

##### enableSecureProcessing

```
JCheckBox enableSecureProcessing
```

##### enableSystemParameterEntityExpandionInOtheEntities

```
JCheckBox enableSystemParameterEntityExpandionInOtheEntities
```

##### entityExpansionLimitTextField

```
ro.sync.ui.UndoableTextField entityExpansionLimitTextField
```

##### languageFixup

```
JCheckBox languageFixup
```

##### nodeLimitMaximumOccuranceTextField

```
ro.sync.ui.UndoableTextField nodeLimitMaximumOccuranceTextField
```

##### validateAgainstSchema

```
JCheckBox validateAgainstSchema
```

##### xInclude

```
JCheckBox xInclude
```

### Class ro.sync.exml.options.XMLPrefixToColorOptionPane

class XMLPrefixToColorOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### colorAndStylePanel

```
ro.sync.exml.options.ColorAndStylePanel colorAndStylePanel
```

##### currentCAP

```
ro.sync.exml.options.XMLPrefixToColorOptionPane.ColorAndProxy currentCAP
```

##### list

```
JList list
```

##### model

```
DefaultListModel model
```

##### prefixOnlyCheck

```
JCheckBox prefixOnlyCheck
```

### Class ro.sync.exml.options.XMLRefactoringOptionPane

class XMLRefactoringOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### additionalOperationsDirTextField

```
ro.sync.ui.UndoableTextField additionalOperationsDirTextField
```

### Class ro.sync.exml.options.XMLSchemaOptionPane

class XMLSchemaOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### assertionsCanSeeComments

```
JCheckBox assertionsCanSeeComments
```

##### enableCommentsPIsForAssertions

```
JCheckBox enableCommentsPIsForAssertions
```

##### engineSaxonEERadio

```
JRadioButton engineSaxonEERadio
```

##### engineXercesRadio

```
JRadioButton engineXercesRadio
```

##### fullChecking

```
JCheckBox fullChecking
```

##### fullXPathChecking

```
JCheckBox fullXPathChecking
```

##### honourAllSchemas

```
JCheckBox honourAllSchemas
```

##### multipleSchemaImports

```
JCheckBox multipleSchemaImports
```

##### version1_0Radio

```
JRadioButton version1_0Radio
```

##### version1_1Radio

```
JRadioButton version1_1Radio
```

### Class ro.sync.exml.options.XPathOptionPane

class XPathOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### defNSEditor

```
ro.sync.exml.options.XPathOptionPane.XPathDefaultNamespaceEditor defNSEditor
```

##### model

```
DefaultTableModel model
```

##### multipleXPathResultsCheck

```
JCheckBox multipleXPathResultsCheck
```

##### tablePanel

```
ro.sync.ui.table.EditableTablePanel tablePanel
```

##### unescapeExpressionCheck

```
JCheckBox unescapeExpressionCheck
```

### Class ro.sync.exml.options.XPathOptionPane.XPathDefaultNamespaceEditor

class XPathDefaultNamespaceEditor extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### noNamespace

```
JRadioButton noNamespace
```

##### rootDefaultNamespace

```
JRadioButton rootDefaultNamespace
```

##### rootNamespace

```
JRadioButton rootNamespace
```

##### thisNamespace

```
JRadioButton thisNamespace
```

##### thisNamespaceText

```
ro.sync.ui.UndoableTextField thisNamespaceText
```

### Class ro.sync.exml.options.XProcEnginesOptionPane

class XProcEnginesOptionPane extends ro.sync.exml.options.CustomEnginesOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### xprocVerbosity

```
JCheckBox xprocVerbosity
```

### Class ro.sync.exml.options.XQJOptionPane

class XQJOptionPane extends ro.sync.exml.options.DBSourceConfiguratorBase implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### driver

```
ro.sync.db.core.DBSourceDriverInfo driver
```

##### passwordRenderer

```
ro.sync.exml.options.XQJOptionPane.PasswordRenderer passwordRenderer
```

##### propertiesTable

```
ro.sync.ui.KeySearchTable propertiesTable
```

### Class ro.sync.exml.options.XQJOptionPane.PropsCellEditor

class PropsCellEditor extends [DefaultCellEditor](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/DefaultCellEditor.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### isPasswordInPlace

```
boolean isPasswordInPlace
```

##### passwordField

```
ro.sync.ui.application.ApplicationPasswordField passwordField
```

### Class ro.sync.exml.options.XQJOptionPane.PropsTableModel

class PropsTableModel extends [AbstractTableModel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/AbstractTableModel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### properties

```
ro.sync.options.SerializableLinkedHashMap<String,String> properties
```

### Class ro.sync.exml.options.XQueryOptionPaneGroup

class XQueryOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### formatTransformerOutput

```
JCheckBox formatTransformerOutput
```

##### saxon8WrapResult

```
JCheckBox saxon8WrapResult
```

##### sizeLimitField

```
ro.sync.ui.UndoableTextField sizeLimitField
```

##### xqueryTransformerCombo

```
ro.sync.ui.application.ApplicationComboBox xqueryTransformerCombo
```

### Class ro.sync.exml.options.XQuerySaxonAdvancedOptionPane

class XQuerySaxonAdvancedOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### collectionUriResolverClassNameField

```
ro.sync.ui.UndoableTextField collectionUriResolverClassNameField
```

##### uriResolverClassNameField

```
ro.sync.ui.UndoableTextField uriResolverClassNameField
```

### Class ro.sync.exml.options.XQuerySaxonOptionPane

class XQuerySaxonOptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### enableBackup

```
JCheckBox enableBackup
```

##### enableOptimizationsCheckBox

```
JCheckBox enableOptimizationsCheckBox
```

##### enableXQueryUpdate

```
JCheckBox enableXQueryUpdate
```

##### saxon8DisableCallsOnExtensionFunctions

```
JCheckBox saxon8DisableCallsOnExtensionFunctions
```

##### saxon8ValidationCommentsInResult

```
JCheckBox saxon8ValidationCommentsInResult
```

##### saxon8ValidationWarningsInResult

```
JCheckBox saxon8ValidationWarningsInResult
```

##### sectionLabelsAlwaysEnabled

```
List<JComponent> sectionLabelsAlwaysEnabled
```

##### urlPanel

```
ro.sync.ui.InputUrlPanel urlPanel
```

##### useConfigFile

```
JCheckBox useConfigFile
```

##### useLinkedTreeModel

```
JCheckBox useLinkedTreeModel
```

##### validationCombo

```
JComboBox validationCombo
```

##### wsCombo

```
JComboBox wsCombo
```

### Class ro.sync.exml.options.XSDSchemaEditorPropertiesOptionPane

class XSDSchemaEditorPropertiesOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### showAdditionalPropertiesInViews

```
JCheckBox showAdditionalPropertiesInViews
```

##### treeTable

```
ro.sync.ui.treetable.ApplicationTreeTable treeTable
```

### Class ro.sync.exml.options.XSLTOptionPaneGroup

class XSLTOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### xslt1TransformerCombo

```
JComboBox xslt1TransformerCombo
```

##### xslt2TransformerCombo

```
JComboBox xslt2TransformerCombo
```

##### xslt3TransformerCombo

```
JComboBox xslt3TransformerCombo
```

### Class ro.sync.exml.options.XSLTProcOptionPane

class XSLTProcOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### debugOn

```
JCheckBox debugOn
```

##### dumpExtensionsOn

```
JCheckBox dumpExtensionsOn
```

##### loadTraceOn

```
JCheckBox loadTraceOn
```

##### maxXslTemplatesTextField

```
ro.sync.ui.UndoableTextField maxXslTemplatesTextField
```

##### noDtdAttrOn

```
JCheckBox noDtdAttrOn
```

##### noMkDirOn

```
JCheckBox noMkDirOn
```

##### noNetOn

```
JCheckBox noNetOn
```

##### noWriteOn

```
JCheckBox noWriteOn
```

##### profileOn

```
JCheckBox profileOn
```

##### skipLoadingDTDOn

```
JCheckBox skipLoadingDTDOn
```

##### timingOn

```
JCheckBox timingOn
```

##### verboseOn

```
JCheckBox verboseOn
```

##### xIncludeOn

```
JCheckBox xIncludeOn
```

##### xsltprocVersion

```
JCheckBox xsltprocVersion
```

### Class ro.sync.exml.options.XSLTSaxon6OptionPane

class XSLTSaxon6OptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### recoverPolicyLabelSaxon6

```
JLabel recoverPolicyLabelSaxon6
```

##### saxon6DisableCallsOnExtensionFunctions

```
JCheckBox saxon6DisableCallsOnExtensionFunctions
```

##### saxon6DoNotRecover

```
JRadioButton saxon6DoNotRecover
```

##### saxon6LineNumberingCheck

```
JCheckBox saxon6LineNumberingCheck
```

##### saxon6RecoverPolicyGroup

```
ButtonGroup saxon6RecoverPolicyGroup
```

##### saxon6RecoverSilent

```
JRadioButton saxon6RecoverSilent
```

##### saxon6RecoverWithWarning

```
JRadioButton saxon6RecoverWithWarning
```

### Class ro.sync.exml.options.XSLTSaxon8AdvancedOptionPane

class XSLTSaxon8AdvancedOptionPane extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### collectionUriResolverClassNameField

```
ro.sync.ui.UndoableTextField collectionUriResolverClassNameField
```

##### uriResolverClassNameField

```
ro.sync.ui.UndoableTextField uriResolverClassNameField
```

### Class ro.sync.exml.options.XSLTSaxon8OptionPane

class XSLTSaxon8OptionPane extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### dtdValidationCombo

```
JComboBox dtdValidationCombo
```

##### enableOptimizations

```
JCheckBox enableOptimizations
```

##### expandAttributeDefaults

```
JCheckBox expandAttributeDefaults
```

##### registerSaxonJSExtension

```
JCheckBox registerSaxonJSExtension
```

##### saxon8AllowCallsOnExtensionFunctions

```
JCheckBox saxon8AllowCallsOnExtensionFunctions
```

##### saxon8EnableAssertions

```
JCheckBox saxon8EnableAssertions
```

##### saxon8LineNumberingCheck

```
JCheckBox saxon8LineNumberingCheck
```

##### saxon8ValidationCommentsInResult

```
JCheckBox saxon8ValidationCommentsInResult
```

##### saxon8ValidationWarningsInResult

```
JCheckBox saxon8ValidationWarningsInResult
```

##### sectionLabelsAlwaysEnabled

```
List<JComponent> sectionLabelsAlwaysEnabled
```

##### traceIntoXPathCheck

```
JCheckBox traceIntoXPathCheck
```

##### urlPanel

```
ro.sync.ui.InputUrlPanel urlPanel
```

##### useConfigFile

```
JCheckBox useConfigFile
```

##### validationCombo

```
JComboBox validationCombo
```

##### wsCombo

```
JComboBox wsCombo
```

### Class ro.sync.exml.options.XSLTXQueryOptionPaneGroup

class XSLTXQueryOptionPaneGroup extends ro.sync.options.BasicOptionPaneGroup implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### allowExtensionFunctionsOutsideFrameworks

```
JCheckBox allowExtensionFunctionsOutsideFrameworks
```

##### tempFilesInTempDir

```
JCheckBox tempFilesInTempDir
```

## Package [ro.sync.exml.plugin](ro/sync/exml/plugin/package-summary.md)

### Class ro.sync.exml.plugin.PluginAction

class PluginAction extends ro.sync.ui.application.action.TaggedAction implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### pluginExtension

```
PluginExtension pluginExtension
```

### Exception ro.sync.exml.plugin.PluginLicensingException

class PluginLicensingException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.exml.plugin.PluginLoadException

class PluginLoadException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### baseDir

```
String baseDir
```

##### pluginName

```
String pluginName
```

## Package [ro.sync.exml.plugin.ai](ro/sync/exml/plugin/ai/package-summary.md)

### Exception [ro.sync.exml.plugin.ai.ExternalServiceException](ro/sync/exml/plugin/ai/ExternalServiceException.md)

class ExternalServiceException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### isFatal

```
boolean isFatal
```

If true, it indicates that the error is critical and further interaction with the AI or further tool executions should be halted. If false, it means the error is non-fatal and the system can recover or continue executing other AI tasks.

## Package [ro.sync.exml.plugin.lock](ro/sync/exml/plugin/lock/package-summary.md)

### Exception [ro.sync.exml.plugin.lock.LockException](ro/sync/exml/plugin/lock/LockException.md)

class LockException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### acquire

```
boolean acquire
```

True if the exception occurred while trying to acquire the lock.

##### detailedMessage

```
String detailedMessage
```

The detailed exception message.

##### ownerName

```
String ownerName
```

The name of the lock owner, null if it is not available.

## Package [ro.sync.exml.workspace.api.editor.page.text.xml](ro/sync/exml/workspace/api/editor/page/text/xml/package-summary.md)

### Exception [ro.sync.exml.workspace.api.editor.page.text.xml.TextOperationException](ro/sync/exml/workspace/api/editor/page/text/xml/TextOperationException.md)

class TextOperationException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.exml.workspace.api.editor.page.text.xml.XPathException](ro/sync/exml/workspace/api/editor/page/text/xml/XPathException.md)

class XPathException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.exml.workspace.api.editor.transformation](ro/sync/exml/workspace/api/editor/transformation/package-summary.md)

### Exception [ro.sync.exml.workspace.api.editor.transformation.TransformationScenarioNotFoundException](ro/sync/exml/workspace/api/editor/transformation/TransformationScenarioNotFoundException.md)

class TransformationScenarioNotFoundException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.exml.workspace.api.editor.validation](ro/sync/exml/workspace/api/editor/validation/package-summary.md)

### Exception [ro.sync.exml.workspace.api.editor.validation.OperationInProgressException](ro/sync/exml/workspace/api/editor/validation/OperationInProgressException.md)

class OperationInProgressException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception [ro.sync.exml.workspace.api.editor.validation.ValidationScenarioNotFoundException](ro/sync/exml/workspace/api/editor/validation/ValidationScenarioNotFoundException.md)

class ValidationScenarioNotFoundException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.exml.workspace.api.images.handlers](ro/sync/exml/workspace/api/images/handlers/package-summary.md)

### Exception [ro.sync.exml.workspace.api.images.handlers.CannotEditException](ro/sync/exml/workspace/api/images/handlers/CannotEditException.md)

class CannotEditException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.exml.workspace.api.options](ro/sync/exml/workspace/api/options/package-summary.md)

### Class [ro.sync.exml.workspace.api.options.SimpleListOfStringsExternalPersistentObject](ro/sync/exml/workspace/api/options/SimpleListOfStringsExternalPersistentObject.md)

class SimpleListOfStringsExternalPersistentObject extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### items

```
ro.sync.options.SerializableList<String> items
```

The items list

## Package [ro.sync.exml.workspace.api.standalone.project](ro/sync/exml/workspace/api/standalone/project/package-summary.md)

### Exception [ro.sync.exml.workspace.api.standalone.project.ProjectIndexerException](ro/sync/exml/workspace/api/standalone/project/ProjectIndexerException.md)

class ProjectIndexerException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.exml.workspace.api.standalone.ui](ro/sync/exml/workspace/api/standalone/ui/package-summary.md)

### Class [ro.sync.exml.workspace.api.standalone.ui.Button](ro/sync/exml/workspace/api/standalone/ui/Button.md)

class Button extends ro.sync.ui.application.ApplicationButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.ColorButton](ro/sync/exml/workspace/api/standalone/ui/ColorButton.md)

class ColorButton extends ro.sync.exml.options.ColorButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.Menu](ro/sync/exml/workspace/api/standalone/ui/Menu.md)

class Menu extends ro.sync.ui.application.menu.ApplicationMenu implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.OKCancelDialog](ro/sync/exml/workspace/api/standalone/ui/OKCancelDialog.md)

class OKCancelDialog extends [JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### buttonsSize

```
Dimension buttonsSize
```

Default buttons size.

##### cancelButton

```
JButton cancelButton
```

The cancel button.

##### contentPanel

```
JPanel contentPanel
```

The content panel

##### helpButton

```
JButton helpButton
```

The help button.

##### okButton

```
JButton okButton
```

The ok button.

##### result

```
int result
```

The result of the dialog. If 'Ok' was pressed the dialog data can be questioned, otherwise does not matter.

### Class [ro.sync.exml.workspace.api.standalone.ui.PopupMenu](ro/sync/exml/workspace/api/standalone/ui/PopupMenu.md)

class PopupMenu extends ro.sync.ui.application.ApplicationPopupMenu implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.SplitMenuButton](ro/sync/exml/workspace/api/standalone/ui/SplitMenuButton.md)

class SplitMenuButton extends ro.sync.ui.ApplicationSplitButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.Table](ro/sync/exml/workspace/api/standalone/ui/Table.md)

class Table extends ro.sync.ui.application.ApplicationTable implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.TextField](ro/sync/exml/workspace/api/standalone/ui/TextField.md)

class TextField extends ro.sync.ui.ApplicationTextField implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.ToolbarButton](ro/sync/exml/workspace/api/standalone/ui/ToolbarButton.md)

class ToolbarButton extends ro.sync.ui.toolbar.ToolBarButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.ToolbarToggleButton](ro/sync/exml/workspace/api/standalone/ui/ToolbarToggleButton.md)

class ToolbarToggleButton extends ro.sync.ui.toolbar.ToolbarToggleButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.Tree](ro/sync/exml/workspace/api/standalone/ui/Tree.md)

class Tree extends ro.sync.ui.application.ApplicationTree implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class [ro.sync.exml.workspace.api.standalone.ui.TreeCellRenderer](ro/sync/exml/workspace/api/standalone/ui/TreeCellRenderer.md)

class TreeCellRenderer extends ro.sync.ui.application.ApplicationTreeCellRenderer implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.exml.workspace.api.util](ro/sync/exml/workspace/api/util/package-summary.md)

### Exception [ro.sync.exml.workspace.api.util.PrettyPrintException](ro/sync/exml/workspace/api/util/PrettyPrintException.md)

class PrettyPrintException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.net.protocol.http](ro/sync/net/protocol/http/package-summary.md)

### Exception [ro.sync.net.protocol.http.HttpExceptionWithDetails](ro/sync/net/protocol/http/HttpExceptionWithDetails.md)

class HttpExceptionWithDetails extends ro.sync.basic.net.http.HttpException implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### baseURL

```
URL baseURL
```

The base URL.

##### httpResponse

```
ro.sync.net.protocol.http.abstraction.HttpResponse httpResponse
```

The httpResponse of the request that threw this HttpException.

### Exception ro.sync.net.protocol.http.ServerHasNoLockSupportException

class ServerHasNoLockSupportException extends [LockException](ro/sync/exml/plugin/lock/LockException.md) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.options](ro/sync/options/package-summary.md)

### Class ro.sync.options.BasicOptionPane

class BasicOptionPane extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### content

```
JPanel content
```

##### controlPanel

```
JPanel controlPanel
```

##### count

```
int count
```

##### globalOptionsButton

```
JToggleButton globalOptionsButton
```

##### gridBagLayout

```
GridBagLayout gridBagLayout
```

##### helpButton

```
ro.sync.ui.InlineHelpButton helpButton
```

##### helper

```
ro.sync.options.PropertiesHelper helper
```

##### hideProjectOptionsChooser

```
boolean hideProjectOptionsChooser
```

##### hideStorageChoosers

```
boolean hideStorageChoosers
```

##### ignoreOptionsListener

```
boolean ignoreOptionsListener
```

##### imposedLevelZeroIndentationValue

```
int imposedLevelZeroIndentationValue
```

##### initialized

```
boolean initialized
```

##### name

```
String name
```

##### paneKey

```
String paneKey
```

##### projectOptionsButton

```
JToggleButton projectOptionsButton
```

##### properties

```
ro.sync.options.NotifyableMap properties
```

##### storeLocationListener

```
ro.sync.options.PageStoreLocationChangedListener storeLocationListener
```

##### useGlobalOptions

```
boolean useGlobalOptions
```

### Class ro.sync.options.BasicOptionPaneGroup

class BasicOptionPaneGroup extends ro.sync.options.BasicOptionPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### itemsToSaveLater

```
List<ro.sync.options.Persistent> itemsToSaveLater
```

##### members

```
List members
```

### Exception ro.sync.options.EmptySetOfOptionsException

class EmptySetOfOptionsException extends [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.options.EncryptedString

class EncryptedString extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### encryptedStringValue

```
String encryptedStringValue
```

### Exception [ro.sync.options.InvalidPersistentObjException](ro/sync/options/InvalidPersistentObjException.md)

class InvalidPersistentObjException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.options.InvalidPersistentObjRuntimeException

class InvalidPersistentObjRuntimeException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.options.OptionsDeserializedMap

class OptionsDeserializedMap extends ro.sync.options.SerializableLinkedHashMap implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### externalPersistentObjectsMap

```
Map<Object,Object> externalPersistentObjectsMap
```

### Class ro.sync.options.OptionTreeCellRenderer

class OptionTreeCellRenderer extends ro.sync.ui.application.ApplicationTreeCellRenderer implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### boldFont

```
Font boldFont
```

##### filterField

```
ro.sync.ui.UndoableTextField filterField
```

##### treeFont

```
Font treeFont
```

### Class ro.sync.options.SerializableLinkedHashMap

class SerializableLinkedHashMap extends [LinkedHashMap](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/LinkedHashMap.html)<K extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html),V extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.options.SerializableList

class SerializableList extends [ArrayList](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/ArrayList.html)<E extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.options.SimpleXMLSerializerException

class SimpleXMLSerializerException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Exception ro.sync.options.WrongFieldTypeException

class WrongFieldTypeException extends [RuntimeException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/RuntimeException.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### field

```
Field field
```

### Exception ro.sync.options.XmlSerializerException

class XmlSerializerException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.quickfix](ro/sync/quickfix/package-summary.md)

### Exception ro.sync.quickfix.DefaultQuickFixesExecutor.DefaultQuickFixesExecutorException

class DefaultQuickFixesExecutorException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### severity

```
int severity
```

##### type

```
ro.sync.quickfix.DefaultQuickFixesExecutor.DefaultQuickFixesExecutorException.Type type
```

## Package [ro.sync.template](ro/sync/template/package-summary.md)

### Class ro.sync.template.AbstractTemplate

class AbstractTemplate extends ro.sync.template.BaseAbstractTemplate implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### templateLocation

```
File templateLocation
```

### Class ro.sync.template.ArchiveTemplate

class ArchiveTemplate extends ro.sync.template.AbstractTemplate implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.template.BaseAbstractTemplate

class BaseAbstractTemplate extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### bigIconPath

```
String bigIconPath
```

##### displayName

```
String displayName
```

##### filenamePrefix

```
String filenamePrefix
```

##### filenameSuffix

```
String filenameSuffix
```

##### isFromFrameworks

```
boolean isFromFrameworks
```

##### longDescriptionProvider

```
ro.sync.template.LongDescriptionProvider longDescriptionProvider
```

##### smallIconPath

```
String smallIconPath
```

##### sourceInformation

```
String sourceInformation
```

##### typeProperty

```
String typeProperty
```

### Class ro.sync.template.ConfigResourceBasedTemplate

class ConfigResourceBasedTemplate extends ro.sync.template.BaseAbstractTemplate implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### otherProps

```
ro.sync.options.SerializableLinkedHashMap<String,String> otherProps
```

##### templateURL

```
String templateURL
```

### Class ro.sync.template.FileTemplate

class FileTemplate extends ro.sync.template.AbstractTemplate implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### otherProps

```
ro.sync.options.SerializableLinkedHashMap<String,String> otherProps
```

### Class ro.sync.template.ProjectTemplate

class ProjectTemplate extends ro.sync.template.AbstractTemplate implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### expandEdVarsExcludeFilter

```
String expandEdVarsExcludeFilter
```

##### expandEdVarsIncludeFilter

```
String expandEdVarsIncludeFilter
```

### Class ro.sync.template.RecentlyUsedEditorTemplates

class RecentlyUsedEditorTemplates extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### recentlyUsed

```
ro.sync.options.SerializableList<EditorTemplate> recentlyUsed
```

### Class ro.sync.template.RemoteFileTemplate

class RemoteFileTemplate extends ro.sync.template.BaseAbstractTemplate implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### otherProps

```
ro.sync.options.SerializableLinkedHashMap<String,String> otherProps
```

##### templateLocation

```
URL templateLocation
```

### Class ro.sync.template.SimpleEditorTemplate

class SimpleEditorTemplate extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### content

```
String content
```

##### customizationPageID

```
String customizationPageID
```

##### description

```
String description
```

##### extension

```
String extension
```

### Class ro.sync.template.SimpleEditorTemplateWithImposedContentType

class SimpleEditorTemplateWithImposedContentType extends ro.sync.template.SimpleEditorTemplate implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### imposedContentType

```
String imposedContentType
```

## Package [ro.sync.ui.application](ro/sync/ui/application/package-summary.md)

### Class ro.sync.ui.application.ApplicationAdaptiveLayoutPanel

class ApplicationAdaptiveLayoutPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### lastLayoutMode

```
ro.sync.ui.application.ApplicationAdaptiveLayoutPanel.LayoutMode lastLayoutMode
```

##### lastTopContainer

```
Container lastTopContainer
```

##### topContainerComponentListener

```
ComponentListener topContainerComponentListener
```

### Class ro.sync.ui.application.ApplicationArrowButton

class ApplicationArrowButton extends [BasicArrowButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/plaf/basic/BasicArrowButton.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### colorTheme

```
ro.sync.ui.theme.ColorTheme colorTheme
```

##### forComboBox

```
boolean forComboBox
```

##### foregroundColor

```
Color foregroundColor
```

### Class ro.sync.ui.application.ApplicationBorderFactory.ApplicationTitledBorder

class ApplicationTitledBorder extends [TitledBorder](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/border/TitledBorder.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationButton

class ApplicationButton extends [JButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JButton.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### disabledIconSet

```
boolean disabledIconSet
```

##### disabledSelectedIconSet

```
boolean disabledSelectedIconSet
```

##### ourDisabledIcon

```
Icon ourDisabledIcon
```

##### ourDisabledSelectedIcon

```
Icon ourDisabledSelectedIcon
```

##### ourPressedIcon

```
Icon ourPressedIcon
```

##### pressedIconSet

```
boolean pressedIconSet
```

### Class ro.sync.ui.application.ApplicationComboBox

class ApplicationComboBox extends [JComboBox](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComboBox.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### editorComponentLocationAdjusted

```
boolean editorComponentLocationAdjusted
```

##### imposedMaxNoOfCheckedItemsToComputeWidthOfCombo

```
int imposedMaxNoOfCheckedItemsToComputeWidthOfCombo
```

##### lastComputedPopupWidth

```
int lastComputedPopupWidth
```

##### layingOut

```
boolean layingOut
```

##### listRendererWasSet

```
boolean listRendererWasSet
```

##### maxPopupWidth

```
int maxPopupWidth
```

##### modelListener

```
ListDataListener modelListener
```

##### popupListRenderer

```
ro.sync.ui.application.ApplicationComboBox.PopupListCellRenderer popupListRenderer
```

##### widthLimit

```
int widthLimit
```

### Class ro.sync.ui.application.ApplicationContentPanel

class ApplicationContentPanel extends ro.sync.ui.application.ApplicationPanel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### basicTopPanel

```
JPanel basicTopPanel
```

##### messageTypePanel

```
JPanel messageTypePanel
```

##### neverShowCheckBox

```
JCheckBox neverShowCheckBox
```

##### neverShowCheckboxPanel

```
JPanel neverShowCheckboxPanel
```

##### southPanel

```
JPanel southPanel
```

### Class ro.sync.ui.application.ApplicationEditorPane

class ApplicationEditorPane extends [JEditorPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JEditorPane.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationFilePathLabel

class ApplicationFilePathLabel extends [JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### enableResizeListener

```
boolean enableResizeListener
```

##### originalText

```
String originalText
```

### Class ro.sync.ui.application.ApplicationFrame

class ApplicationFrame extends com.jidesoft.action.DefaultDockableBarHolder implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### editMenuInstalled

```
boolean editMenuInstalled
```

### Class ro.sync.ui.application.ApplicationHTMLLabel

class ApplicationHTMLLabel extends [JLabel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JLabel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationHTMLListCellRenderer

class ApplicationHTMLListCellRenderer extends ro.sync.ui.application.ApplicationHTMLLabel implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### isHovered

```
boolean isHovered
```

##### isSelected

```
boolean isSelected
```

##### linkForeground

```
String linkForeground
```

##### list

```
JList list
```

##### verticalScrollbarSize

```
int verticalScrollbarSize
```

##### winSelectionPainter

```
ro.sync.ui.application.WindowsVistaPainter winSelectionPainter
```

### Class ro.sync.ui.application.ApplicationJideButton

class ApplicationJideButton extends com.jidesoft.swing.JideButton implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### disabledIconSet

```
boolean disabledIconSet
```

##### disabledSelectedIconSet

```
boolean disabledSelectedIconSet
```

##### ourDisabledIcon

```
Icon ourDisabledIcon
```

##### ourDisabledSelectedIcon

```
Icon ourDisabledSelectedIcon
```

##### ourPressedIcon

```
Icon ourPressedIcon
```

##### pressedIconSet

```
boolean pressedIconSet
```

### Class ro.sync.ui.application.ApplicationListResizeSensitive

class ApplicationListResizeSensitive extends ro.sync.ui.application.list.ApplicationHoveringList implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### size

```
Dimension size
```

### Class ro.sync.ui.application.ApplicationLoadingProgress

class ApplicationLoadingProgress extends [JDialog](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JDialog.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### inhibit

```
boolean inhibit
```

##### messageLabel

```
JLabel messageLabel
```

##### progressBar

```
ro.sync.ui.application.ApplicationProgressBar progressBar
```

### Class ro.sync.ui.application.ApplicationMainFrame

class ApplicationMainFrame extends ro.sync.ui.application.ApplicationFrame implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### descriptor

```
ro.sync.ui.application.ApplicationMainFrameDescriptor descriptor
```

##### exitHandler

```
ro.sync.exml.ExitHandler exitHandler
```

##### lastLocation

```
Point lastLocation
```

##### location

```
Point location
```

##### maximized

```
boolean maximized
```

##### openLastOpenedFiles

```
boolean openLastOpenedFiles
```

##### size

```
Dimension size
```

##### splashWindow

```
ro.sync.exml.Splash splashWindow
```

### Class ro.sync.ui.application.ApplicationOptionPane

class ApplicationOptionPane extends [JOptionPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JOptionPane.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationOptionPane.FormattedPanel

class FormattedPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationPanel

class ApplicationPanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationPasswordField

class ApplicationPasswordField extends [JPasswordField](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPasswordField.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### widthLimit

```
int widthLimit
```

### Class ro.sync.ui.application.ApplicationPopupMenu

class ApplicationPopupMenu extends [JPopupMenu](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPopupMenu.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### invokerFocusListener

```
FocusListener invokerFocusListener
```

##### menuTagPath

```
String[] menuTagPath
```

### Class ro.sync.ui.application.ApplicationProgressBar

class ApplicationProgressBar extends [JProgressBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JProgressBar.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### wasForcedToDeterminate

```
boolean wasForcedToDeterminate
```

### Class ro.sync.ui.application.ApplicationScrollPane

class ApplicationScrollPane extends [JScrollPane](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JScrollPane.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### viewListener

```
ContainerListener viewListener
```

##### viewportChangeListener

```
PropertyChangeListener viewportChangeListener
```

### Class ro.sync.ui.application.ApplicationTable

class ApplicationTable extends [JTable](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTable.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### changeSelection

```
boolean changeSelection
```

##### columnListener

```
PropertyChangeListener columnListener
```

##### columnModelListener

```
TableColumnModelListener columnModelListener
```

##### defaultAction

```
Action defaultAction
```

##### deleteAction

```
Action deleteAction
```

##### doubleClickListener

```
MouseListener doubleClickListener
```

##### drawingStripes

```
boolean drawingStripes
```

##### macOSTableHeaderUpdaterSortListener

```
RowSorterListener macOSTableHeaderUpdaterSortListener
```

##### oldRowSorter

```
RowSorter oldRowSorter
```

##### rowColors

```
Color[] rowColors
```

##### rowHeightUpdater

```
ro.sync.ui.application.RowHeightUpdater rowHeightUpdater
```

### Class ro.sync.ui.application.ApplicationTable.BooleanEditor

class BooleanEditor extends [DefaultCellEditor](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/DefaultCellEditor.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationTableHeader

class ApplicationTableHeader extends [JTableHeader](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/JTableHeader.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### columnModelListener

```
TableColumnModelListener columnModelListener
```

### Class ro.sync.ui.application.ApplicationTableHeader.SimpleHeaderRenderer

class SimpleHeaderRenderer extends [DefaultTableCellRenderer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/table/DefaultTableCellRenderer.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### colorTheme

```
ro.sync.ui.theme.ColorTheme colorTheme
```

##### horizontalTextPositionSet

```
boolean horizontalTextPositionSet
```

### Class ro.sync.ui.application.ApplicationTextArea

class ApplicationTextArea extends [JTextArea](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTextArea.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### inputMethodRequestsWrapper

```
InputMethodRequests inputMethodRequestsWrapper
```

### Class ro.sync.ui.application.ApplicationToggleButton

class ApplicationToggleButton extends [JToggleButton](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToggleButton.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### disabledIconSet

```
boolean disabledIconSet
```

##### disabledSelectedIconSet

```
boolean disabledSelectedIconSet
```

##### ourDisabledIcon

```
Icon ourDisabledIcon
```

##### ourDisabledSelectedIcon

```
Icon ourDisabledSelectedIcon
```

##### ourPressedIcon

```
Icon ourPressedIcon
```

##### pressedIconSet

```
boolean pressedIconSet
```

### Class ro.sync.ui.application.ApplicationTranslucentMessageWindow

class ApplicationTranslucentMessageWindow extends [JWindow](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JWindow.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### currentTranslucency

```
float currentTranslucency
```

##### delayUntilFade

```
int delayUntilFade
```

##### fadeTimer

```
Timer fadeTimer
```

### Class ro.sync.ui.application.ApplicationTree

class ApplicationTree extends [JTree](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTree.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### doubleClickAction

```
Action doubleClickAction
```

##### doubleClickListener

```
MouseListener doubleClickListener
```

##### enableCellEditing

```
boolean enableCellEditing
```

##### focusAwareCellEditing

```
boolean focusAwareCellEditing
```

##### lastNotifiedTreeExpansionListener

```
TreeExpansionListener lastNotifiedTreeExpansionListener
```

##### skipNextMouseReleasedEvent

```
boolean skipNextMouseReleasedEvent
```

##### skipNextMouseReleasedWhen

```
long skipNextMouseReleasedWhen
```

### Class ro.sync.ui.application.ApplicationTree.ApplicationAccessibleJTree

class ApplicationAccessibleJTree extends [JTree.AccessibleJTree](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JTree.AccessibleJTree.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.ApplicationTreeCellEditor.ApplicationEditorContainer

class ApplicationEditorContainer extends [Container](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/java/awt/Container.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### leftInset

```
int leftInset
```

### Class ro.sync.ui.application.ApplicationTreeCellRenderer

class ApplicationTreeCellRenderer extends [DefaultTreeCellRenderer](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/tree/DefaultTreeCellRenderer.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### active

```
boolean active
```

##### activeInactiveSelectionEnabled

```
boolean activeInactiveSelectionEnabled
```

##### macActiveSelectionColor

```
Color macActiveSelectionColor
```

##### macActiveSelectionTextColor

```
Color macActiveSelectionTextColor
```

##### macInactiveSelectionTextColor

```
Color macInactiveSelectionTextColor
```

##### selectionPainter

```
ro.sync.ui.application.WindowsVistaPainter selectionPainter
```

### Class ro.sync.ui.application.DarkModeAwareHTMLEditorKit

class DarkModeAwareHTMLEditorKit extends [HTMLEditorKit](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/text/html/HTMLEditorKit.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.DashedBorder

class DashedBorder extends [AbstractBorder](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/border/AbstractBorder.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### color

```
Color color
```

### Class ro.sync.ui.application.HoverButtonsToolbar

class HoverButtonsToolbar extends [JToolBar](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JToolBar.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.LeftScrollBarScrollPaneLayout

class LeftScrollBarScrollPaneLayout extends [ScrollPaneLayout](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/ScrollPaneLayout.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.MiddleClickScrollableScrollPane

class MiddleClickScrollableScrollPane extends ro.sync.ui.application.ApplicationScrollPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### autoScrollDecoration

```
JLabel autoScrollDecoration
```

##### autoScrollDecorationBounds

```
Rectangle autoScrollDecorationBounds
```

##### currentAutoScrollPoint

```
Point currentAutoScrollPoint
```

##### focusListener

```
FocusListener focusListener
```

##### inAutoScrollState

```
boolean inAutoScrollState
```

##### inDragScrollState

```
boolean inDragScrollState
```

##### keyListener

```
KeyListener keyListener
```

##### mouseListener

```
MouseListener mouseListener
```

##### mouseMotionListener

```
MouseMotionListener mouseMotionListener
```

##### previousComponentCursor

```
Cursor previousComponentCursor
```

##### scrollTimer

```
Timer scrollTimer
```

### Class ro.sync.ui.application.RightRowHeaderScrollPaneLayout

class RightRowHeaderScrollPaneLayout extends [ScrollPaneLayout](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/ScrollPaneLayout.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.TreeBasePanelCellRenderer

class TreeBasePanelCellRenderer extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### active

```
boolean active
```

##### delegateSelectionPainting

```
boolean delegateSelectionPainting
```

##### selected

```
boolean selected
```

##### selectionPainter

```
ro.sync.ui.application.WindowsVistaPainter selectionPainter
```

### Class ro.sync.ui.application.UnicodeFontUpdatablePanel

class UnicodeFontUpdatablePanel extends [JPanel](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JPanel.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

### Class ro.sync.ui.application.WrapLongSentencesApplicationEditorPane

class WrapLongSentencesApplicationEditorPane extends ro.sync.ui.application.ApplicationEditorPane implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

## Package [ro.sync.util.editorvars](ro/sync/util/editorvars/package-summary.md)

### Class ro.sync.util.editorvars.UserEditorVariablePO

class UserEditorVariablePO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### name

```
String name
```

##### shortDescription

```
String shortDescription
```

##### value

```
String value
```

### Class ro.sync.util.editorvars.UserSecretPO

class UserSecretPO extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

#### Serialized Fields

##### encryptedValue

```
String encryptedValue
```

##### name

```
String name
```

## Package [ro.sync.xml.parser](ro/sync/xml/parser/package-summary.md)

### Exception ro.sync.xml.parser.HTMLParserCreator.HTMLParserCreationException

class HTMLParserCreationException extends [Exception](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Exception.html) implements [Serializable](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Serializable.html)

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
