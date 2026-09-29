Package [ro.sync.ecss.extensions.api.content](package-summary.md)

# Interface ClipboardFragmentInformation
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ClipboardFragmentInformation
Provides information about a fragment in the clipboard. The fragment received in the callback can either be directly processed or a new fragment can be set instead. An easy way to modify the fragment XML content is like this:
```

  public void process(ClipboardFragmentInformation fragmentInformation) {
   AuthorDocumentFragment frag = fragmentInformation.getFragment();
   try {
     String xmlContent = authorAccess.getDocumentController().serializeFragmentToXML(frag);
     //Modify the XML content here.....

     //Re-create a new fragment from the XML
     AuthorDocumentFragment newFragment = authorAccess.getDocumentController().createNewDocumentFragmentInContext(xmlContent, authorAccess.getEditorAccess().getCaretOffset());

     fragmentInformation.setFragment(newFragment);
   } catch (BadLocationException e) {
     e.printStackTrace();
   } catch (AuthorOperationException e) {
     e.printStackTrace();
   }
 }
```

  Since: 12.2
## Method Summary
  All MethodsInstance MethodsAbstract MethodsDeprecated Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getClipboardObjectID](#getClipboardObjectID())()
Get an unique ID of this object taken from the clipboard.
  [AuthorDocumentFragment](../node/AuthorDocumentFragment.md) [getFragment](#getFragment())()
Get the fragment which will be pasted/dropped.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getFragmentOriginalLocation](#getFragmentOriginalLocation())()  Deprecated.
from Oxygen 24 because it modifies the system ID at consecutive Paste, setting the systemID as current editor location.
   [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getLocationOfLastPaste](#getLocationOfLastPaste())()
Get the fragment original location or the location where it was last pasted.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getOriginalLocation](#getOriginalLocation())()
The URL of the file from which the fragment was copied.
  int [getPurposeID](#getPurposeID())()
Get the purpose for which this fragment is used.
  void [setFragment](#setFragment(ro.sync.ecss.extensions.api.node.AuthorDocumentFragment))([AuthorDocumentFragment](../node/AuthorDocumentFragment.md) newFragment)
Set a new fragment replacing the original one which will be pasted/dropped.

## Method Details

### getPurposeID

int getPurposeID()

Get the purpose for which this fragment is used. One of the constants:
        * [AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_COPY](../AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_COPY)
        * [AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_CUT](../AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_CUT)
        * [AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_DND_COPY](../AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_DND_COPY)
        * [AuthorSchemaAwareEditingHandler.CREATE_FRAGMENT_PURPOSE_DND_MOVE](../AuthorSchemaAwareEditingHandler.md#CREATE_FRAGMENT_PURPOSE_DND_MOVE)

  Returns: The purpose for which this fragment is used.
### getClipboardObjectID

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getClipboardObjectID()

Get an unique ID of this object taken from the clipboard. For example if multiple pastes are made with same content, the same object ID is returned.
  Returns: An unique ID of this object taken from the clipboard.
### getFragmentOriginalLocation

[@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getFragmentOriginalLocation()
 Deprecated.
from Oxygen 24 because it modifies the system ID at consecutive Paste, setting the systemID as current editor location.

Get the URL of the file from which the fragment was copied. If the fragment was pasted from outside of Oxygen, the original location is null.
  Returns: The URL of the file from which the fragment was copied. If the fragment was pasted from outside of Oxygen, the original location is null.
### getFragment

[AuthorDocumentFragment](../node/AuthorDocumentFragment.md) getFragment()

Get the fragment which will be pasted/dropped.
  Returns: The fragment which will be pasted/dropped.
### setFragment

void setFragment([AuthorDocumentFragment](../node/AuthorDocumentFragment.md) newFragment)

Set a new fragment replacing the original one which will be pasted/dropped.
  Parameters: newFragment - The fragment which will be pasted/dropped. Since: 13
### getOriginalLocation

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getOriginalLocation()

The URL of the file from which the fragment was copied. If the fragment was pasted from outside of Oxygen, the original location is null.
  Returns: URL of the file from which the fragment was copied. Since: 24.0
### getLocationOfLastPaste

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getLocationOfLastPaste()

Get the fragment original location or the location where it was last pasted. Can be null
  Returns: the fragment original location or the location where it was last pasted. Since: 24.0
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
