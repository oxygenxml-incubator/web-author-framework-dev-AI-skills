Package [ro.sync.ecss.extensions.api.component.listeners](package-summary.md)

# Interface AuthorComponentListener
    @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorComponentListener
Author component listener

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [documentTypeChanged](#documentTypeChanged())()
The editor document type changed (for example from Docbook to DITA).
  void [loadedDocumentChanged](#loadedDocumentChanged())()
The loaded document changed.
  void [modifiedStateChanged](#modifiedStateChanged(boolean))(boolean modified)
The modified state of the component changed

## Method Details

### modifiedStateChanged

void modifiedStateChanged(boolean modified)

The modified state of the component changed
  Parameters: modified - true if the edited text in the component is modified, false otherwise
### loadedDocumentChanged

void loadedDocumentChanged()

The loaded document changed. load(URL, Reader) was called

### documentTypeChanged

void documentTypeChanged()

The editor document type changed (for example from Docbook to DITA).

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
