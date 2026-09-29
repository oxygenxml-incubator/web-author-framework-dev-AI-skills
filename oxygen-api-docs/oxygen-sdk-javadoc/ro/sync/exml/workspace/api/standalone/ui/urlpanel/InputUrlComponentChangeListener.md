Package [ro.sync.exml.workspace.api.standalone.ui.urlpanel](package-summary.md)

# Interface InputUrlComponentChangeListener
    @API(type=EXTENDABLE, src=PUBLIC) public interface InputUrlComponentChangeListener
Notifies changes in [InputUrlComponentProvider](InputUrlComponentProvider.md) components.
  Since: 23.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [urlModified](#urlModified())()
Callback when the URL was modified.
  void [urlSelected](#urlSelected(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Callback when a new URL(different from the last selection) is selected.

## Method Details

### urlModified

void urlModified()

Callback when the URL was modified.

### urlSelected

void urlSelected([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Callback when a new URL(different from the last selection) is selected.
  Parameters: url - The url, or null if it is not a valid url.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
