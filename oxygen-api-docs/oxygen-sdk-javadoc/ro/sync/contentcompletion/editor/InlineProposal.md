Package [ro.sync.contentcompletion.editor](package-summary.md)

# Interface InlineProposal
    All Known Subinterfaces: [IQuickAssistProposal](../../exml/editor/quickassist/IQuickAssistProposal.md)<I>, [SAQuickAssistProposal](../../exml/editor/quickassist/sa/SAQuickAssistProposal.md)   @API(type=INTERNAL, src=PUBLIC) public interface InlineProposal
Inline proposal presented in InlineProposalsWindow.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final int [HIGH_IMPORTANCE](#HIGH_IMPORTANCE)
The item is of high importance.
  static final int [LOW_IMPORTANCE](#LOW_IMPORTANCE)
The item is of low importance.
  static final int [NORMAL_IMPORTANCE](#NORMAL_IMPORTANCE)
The item is of normal importance.
  static final int [PRESENT_NORMALLY](#PRESENT_NORMALLY)
The item is to be presented in the normal position in the list.
  static final int [PRESENT_VERY_FIRST](#PRESENT_VERY_FIRST)
The item is to be presented as the first item in the list.
  static final int [UNRECOMMENDED_IMPORTANCE](#UNRECOMMENDED_IMPORTANCE)
The item is not recommended to be used.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [compareTo](#compareTo(java.lang.Object,boolean))([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) other, boolean numericSort)
Compares two items.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getDocumentation](#getDocumentation())()
Returns optional additional information about the proposal.
  int [getImportance](#getImportance())()
Gets the importance attribute of the CCItem object
  int [getPresentPosition](#getPresentPosition())()
Used for rendering of the list only.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRenderString](#getRenderString())()
Returns the string to be displayed in the list of completion proposals.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getStringForFilter](#getStringForFilter())()
Gets the string used by filters.

## Field Details

### PRESENT_NORMALLY

static final int PRESENT_NORMALLY

The item is to be presented in the normal position in the list.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.editor.InlineProposal.PRESENT_NORMALLY)

### PRESENT_VERY_FIRST

static final int PRESENT_VERY_FIRST

The item is to be presented as the first item in the list.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.editor.InlineProposal.PRESENT_VERY_FIRST)

### UNRECOMMENDED_IMPORTANCE

static final int UNRECOMMENDED_IMPORTANCE

The item is not recommended to be used. The renderer can ignore it.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.editor.InlineProposal.UNRECOMMENDED_IMPORTANCE)

### LOW_IMPORTANCE

static final int LOW_IMPORTANCE

The item is of low importance.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.editor.InlineProposal.LOW_IMPORTANCE)

### NORMAL_IMPORTANCE

static final int NORMAL_IMPORTANCE

The item is of normal importance.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.editor.InlineProposal.NORMAL_IMPORTANCE)

### HIGH_IMPORTANCE

static final int HIGH_IMPORTANCE

The item is of high importance.
  See Also:
        * [Constant Field Values](../../../../constant-values.md#ro.sync.contentcompletion.editor.InlineProposal.HIGH_IMPORTANCE)

## Method Details

### getStringForFilter

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getStringForFilter()

Gets the string used by filters.
  Returns: The string used by filters.
### getDocumentation

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getDocumentation()

Returns optional additional information about the proposal. The additional information will be presented to assist the user in deciding if the selected proposal is the desired choice.
  Returns: the additional information or null
### getRenderString

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRenderString()

Returns the string to be displayed in the list of completion proposals.
  Returns: the string to be displayed
### getImportance

int getImportance()

Gets the importance attribute of the CCItem object
  Returns: The importance value
### getPresentPosition

int getPresentPosition()

Used for rendering of the list only.
  Returns: Returns the presentPosition. See Also:
        * [PRESENT_NORMALLY](#PRESENT_NORMALLY)
        * [PRESENT_VERY_FIRST](#PRESENT_VERY_FIRST)

### compareTo

int compareTo([Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) other, boolean numericSort)

Compares two items. If numericSort is true the compare is done first by trying to convert the render strings to Double. If they are not numeric values then the compare is delegated to the render string. If the render string starts with '/' then it is considered to be greater than the other that does not begin with '/'. This is used for changing the order in the list.
  Parameters: other - The item to be compared with. numericSort - If true numeirc sort will be performed. Returns: -1 if less, 0 if equal, 1 if greater.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
