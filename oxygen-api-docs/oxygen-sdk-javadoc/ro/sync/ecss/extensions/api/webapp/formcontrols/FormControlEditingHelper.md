Package [ro.sync.ecss.extensions.api.webapp.formcontrols](package-summary.md)

# Interface FormControlEditingHelper
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface FormControlEditingHelper
Helper class for editing using form controls.
  Since: 15.2
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDIT_CONTENT](#EDIT_CONTENT)
Constant that indicates that the value to edit represents the content of an element (with possible XML structure)
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [EDIT_TEXT](#EDIT_TEXT)
Constant that indicates that the value to edit represents the text content of an element.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [commitEditedValue](#commitEditedValue(ro.sync.ecss.extensions.api.node.AuthorElement,java.lang.String,java.lang.String))([AuthorElement](../../node/AuthorElement.md) elem, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valueToCommit)
Commits the value edited by the user.
  void [commitEditedValueForProcessingInstruction](#commitEditedValueForProcessingInstruction(ro.sync.ecss.extensions.api.node.AuthorParentNode,java.lang.String,java.lang.String))([AuthorParentNode](../../node/AuthorParentNode.md) elem, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valueToCommit)
Commits the value edited by the user.

## Field Details

### EDIT_CONTENT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDIT_CONTENT

Constant that indicates that the value to edit represents the content of an element (with possible XML structure)
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.formcontrols.FormControlEditingHelper.EDIT_CONTENT)

### EDIT_TEXT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) EDIT_TEXT

Constant that indicates that the value to edit represents the text content of an element.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.formcontrols.FormControlEditingHelper.EDIT_TEXT)

## Method Details

### commitEditedValue

void commitEditedValue([AuthorElement](../../node/AuthorElement.md) elem, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valueToCommit)

Commits the value edited by the user.
  Parameters: elem - The element whose value to edit. toEdit - The attribute name or #CONTENT if we are editing the content of an element or #TEXT to edit the text of the element. null means #TEXT. valueToCommit - The new value to be committed.
### commitEditedValueForProcessingInstruction

void commitEditedValueForProcessingInstruction([AuthorParentNode](../../node/AuthorParentNode.md) elem, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) toEdit, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) valueToCommit)

Commits the value edited by the user.
  Parameters: elem - The processing instruction whose value to edit. toEdit - The attribute name. valueToCommit - The new value to be committed. Since: 21
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
