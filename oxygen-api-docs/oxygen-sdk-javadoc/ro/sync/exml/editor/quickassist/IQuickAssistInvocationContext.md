Package [ro.sync.exml.editor.quickassist](package-summary.md)

# Interface IQuickAssistInvocationContext<P>
    Type Parameters: P - The editor page we are dealing in.   @API(type=INTERNAL, src=PUBLIC) public interface IQuickAssistInvocationContext<P>
Platform independent(Eclipse vs SA) invocation context for the quick assists.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [P](IQuickAssistInvocationContext.md) [getEditorPage](#getEditorPage())()
Returns the editor for this context.
  int [getOffset](#getOffset())()
Returns the offset where quick assist was invoked.

## Method Details

### getOffset

int getOffset()

Returns the offset where quick assist was invoked.
  Returns: the invocation offset.
### getEditorPage

[P](IQuickAssistInvocationContext.md) getEditorPage()

Returns the editor for this context.
  Returns: the editor or null if not available
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
