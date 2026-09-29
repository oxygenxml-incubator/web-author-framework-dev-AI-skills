Package [ro.sync.exml.editor.quickassist](package-summary.md)

# Interface SimpleQuickAssistProcessor
    @API(type=INTERNAL, src=PUBLIC) public interface SimpleQuickAssistProcessor
Quick assist processor for quick fixes and quick assists.
A processor can provide just quick fixes, just quick assists or both.

This interface can be implemented by clients.

## Method Summary
  All MethodsInstance MethodsAbstract MethodsDefault Methods
Modifier and Type

Method

Description
 boolean [canAssist](#canAssist(ro.sync.exml.workspace.api.editor.page.WSEditorPage,int))([WSEditorPage](../../workspace/api/editor/page/WSEditorPage.md) editorPage, int offset)
Tells whether this assistant has assists for the given invocation context.
  [IQuickAssistProposal](IQuickAssistProposal.md)[] [computeQuickAssistProposals](#computeQuickAssistProposals(ro.sync.exml.workspace.api.editor.page.WSEditorPage,int))([WSEditorPage](../../workspace/api/editor/page/WSEditorPage.md) editorPage, int offset)
Returns a list of quick assist and quick fix proposals for the given invocation context.
  default short [getPriority](#getPriority())()

## Method Details

### canAssist

boolean canAssist([WSEditorPage](../../workspace/api/editor/page/WSEditorPage.md) editorPage, int offset)

Tells whether this assistant has assists for the given invocation context.
  Parameters: editorPage - The current editor page. Can be null if the editor page cannot be determined. offset - the offset where quick assist was invoked. Returns: true if the assistant has a proposal for the given context
### computeQuickAssistProposals

[IQuickAssistProposal](IQuickAssistProposal.md)[] computeQuickAssistProposals([WSEditorPage](../../workspace/api/editor/page/WSEditorPage.md) editorPage, int offset)

Returns a list of quick assist and quick fix proposals for the given invocation context.
  Parameters: editorPage - The current editor page. Can be null if the editor page cannot be determined. offset - the offset where quick assist was invoked. Returns: an array of completion proposals or null if no proposals are available
### getPriority

default short getPriority()
  Returns: The priority. One of the constants in ro.sync.exml.editor.quickassist.IQuickAssistProcessor
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
