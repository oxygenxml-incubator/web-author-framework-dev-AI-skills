Package [ro.sync.ecss.extensions.api.highlights](package-summary.md)

# Interface AuthorPersistentHighlightsFilter
    @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorPersistentHighlightsFilter
Filter for the [AuthorPersistentHighlight](AuthorPersistentHighlight.md) presented in the author page, callouts section and review panel.
  Since: 12
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 boolean [isFiltered](#isFiltered(ro.sync.ecss.extensions.api.highlights.AuthorPersistentHighlight))([AuthorPersistentHighlight](AuthorPersistentHighlight.md) persistentHighlight)
Check if the persistent highlight should not be displayed.

## Method Details

### isFiltered

boolean isFiltered([AuthorPersistentHighlight](AuthorPersistentHighlight.md) persistentHighlight)

Check if the persistent highlight should not be displayed.
  Parameters: persistentHighlight - The [AuthorPersistentHighlight](AuthorPersistentHighlight.md) to be checked. Returns: true if the persistent highlight must be filtered.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
