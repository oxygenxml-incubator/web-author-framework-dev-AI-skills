Package [ro.sync.document](package-summary.md)

# Interface GhostTextProvider
    @API(type=INTERNAL, src=PUBLIC) public interface GhostTextProvider
Interface for providing ghost text suggestions in the editor. Ghost text appears as semi-transparent text that suggests completions.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [GhostTextSuggestion](GhostTextSuggestion.md) [getSuggestion](#getSuggestion())()

 boolean [isActive](#isActive())()

 boolean [isSuggestionVisible](#isSuggestionVisible())()

## Method Details

### getSuggestion

[GhostTextSuggestion](GhostTextSuggestion.md) getSuggestion()
  Returns: ghost text suggestion for the given position in the document.
### isActive

boolean isActive()
  Returns: true if this provider is currently active and should provide suggestions
### isSuggestionVisible

boolean isSuggestionVisible()
  Returns: true if the ghost text is currently visible
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
