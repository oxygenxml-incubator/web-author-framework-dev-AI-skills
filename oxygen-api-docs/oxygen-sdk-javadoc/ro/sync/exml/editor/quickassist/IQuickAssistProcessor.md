Package [ro.sync.exml.editor.quickassist](package-summary.md)

# Interface IQuickAssistProcessor
    @API(type=INTERNAL, src=PUBLIC) public interface IQuickAssistProcessor
Quick assist processor for quick fixes and quick assists.
A processor can provide just quick fixes, just quick assists or both.

This interface can be implemented by clients.

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final short [PRIORITY_HIGH](#PRIORITY_HIGH)
A quick assist processor with high priority.
  static final short [PRIORITY_LOW](#PRIORITY_LOW)
A quick assist processor with low priority.
  static final short [PRIORITY_NORMAL](#PRIORITY_NORMAL)
A quick assist processor with normal priority.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [canAssist](#canAssist(ro.sync.exml.editor.quickassist.IQuickAssistInvocationContext))([IQuickAssistInvocationContext](IQuickAssistInvocationContext.md) invocationContext)
Tells whether this assistant has assists for the given invocation context.
  [IQuickAssistProposal](IQuickAssistProposal.md)[] [computeQuickAssistProposals](#computeQuickAssistProposals(ro.sync.exml.editor.quickassist.IQuickAssistInvocationContext))([IQuickAssistInvocationContext](IQuickAssistInvocationContext.md) invocationContext)
Returns a list of quick assist and quick fix proposals for the given invocation context.
  short [getPriority](#getPriority())()
The priority assigned with this processor.

## Field Details

### PRIORITY_LOW

static final short PRIORITY_LOW

A quick assist processor with low priority.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.editor.quickassist.IQuickAssistProcessor.PRIORITY_LOW)

### PRIORITY_NORMAL

static final short PRIORITY_NORMAL

A quick assist processor with normal priority.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.editor.quickassist.IQuickAssistProcessor.PRIORITY_NORMAL)

### PRIORITY_HIGH

static final short PRIORITY_HIGH

A quick assist processor with high priority.
  See Also:
        * [Constant Field Values](../../../../../constant-values.md#ro.sync.exml.editor.quickassist.IQuickAssistProcessor.PRIORITY_HIGH)

## Method Details

### getPriority

short getPriority()

The priority assigned with this processor. The processors are requested depending on this priority, only the proposals of the first processor will be presented.
  Returns: The priority assigned with this processor.
### canAssist

boolean canAssist([IQuickAssistInvocationContext](IQuickAssistInvocationContext.md) invocationContext)

Tells whether this assistant has assists for the given invocation context.
  Parameters: invocationContext - the invocation context Returns: true if the assistant has a fix for the given annotation
### computeQuickAssistProposals

[IQuickAssistProposal](IQuickAssistProposal.md)[] computeQuickAssistProposals([IQuickAssistInvocationContext](IQuickAssistInvocationContext.md) invocationContext)

Returns a list of quick assist and quick fix proposals for the given invocation context.
  Parameters: invocationContext - the invocation context Returns: an array of completion proposals or null if no proposals are available
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
