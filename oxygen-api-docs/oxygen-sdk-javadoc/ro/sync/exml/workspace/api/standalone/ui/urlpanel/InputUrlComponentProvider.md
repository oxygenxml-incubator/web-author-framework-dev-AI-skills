Package [ro.sync.exml.workspace.api.standalone.ui.urlpanel](package-summary.md)

# Interface InputUrlComponentProvider
    @API(type=EXTENDABLE, src=PUBLIC) public interface InputUrlComponentProvider
Gives access to an URL chooser component similar to the ones in the application. The component can be added to Swing-based panels.
  Since: 23.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [addChangeListener](#addChangeListener(ro.sync.exml.workspace.api.standalone.ui.urlpanel.InputUrlComponentChangeListener))([InputUrlComponentChangeListener](InputUrlComponentChangeListener.md) listener)
Adds a listener that notifies when the url is changed.
  [JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) [getJComponent](#getJComponent())()
Get the Java component to add to the layout.
  [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) [getUrl](#getUrl())()
Gets the presented [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getUrlText](#getUrlText())()
Obtain the selected URL text from the url combobox.
  void [removeChangeListener](#removeChangeListener(ro.sync.exml.workspace.api.standalone.ui.urlpanel.InputUrlComponentChangeListener))([InputUrlComponentChangeListener](InputUrlComponentChangeListener.md) listener)
Remove the listener that notifies when the url is changed.
  void [setEnabled](#setEnabled(boolean))(boolean enabled)
Enables or disable the components (the combo, the editor variables and the actions button)
  void [setUrl](#setUrl(java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)
Sets the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) to be presented.
  void [setUrlLabel](#setUrlLabel(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) urlPresenterLabelText)
Changes the text of the label associated with the URL presenter component.
  void [setUrlText](#setUrlText(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newURL)
Set the new url directly inside the component.

## Method Details

### getUrl

[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) getUrl() throws [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html)

Gets the presented [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html).
  Returns: The presented URL. Can be null. Throws: [MalformedURLException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/MalformedURLException.html) - If the presented data cannot be converted to a URL.
### setUrl

void setUrl([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) url)

Sets the [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) to be presented.
  Parameters: url - The URL to be presented.
### getUrlText

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getUrlText()

Obtain the selected URL text from the url combobox. It will return the exact value of the combobox, without expanding any editor variable.
  Returns: Return the selected URL text from the url combobox.
### setUrlText

void setUrlText([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) newURL)

Set the new url directly inside the component. Can contain unexpanded editor variables.
  Parameters: newURL - The new URL.
### setEnabled

void setEnabled(boolean enabled)

Enables or disable the components (the combo, the editor variables and the actions button)
  Parameters: enabled - true to enable.
### setUrlLabel

void setUrlLabel([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) urlPresenterLabelText)

Changes the text of the label associated with the URL presenter component. By default the presented label is URL
  Parameters: urlPresenterLabelText - A new text for the label associated with the URL presenter component. If null, the label will be hidden.
### getJComponent

[JComponent](https://docs.oracle.com/en/java/javase/17/docs/api/java.desktop/javax/swing/JComponent.html) getJComponent()

Get the Java component to add to the layout.
  Returns: The java component to add to layout.
### addChangeListener

void addChangeListener([InputUrlComponentChangeListener](InputUrlComponentChangeListener.md) listener)

Adds a listener that notifies when the url is changed.
  Parameters: listener - The listener that notifies when the url is changed.
### removeChangeListener

void removeChangeListener([InputUrlComponentChangeListener](InputUrlComponentChangeListener.md) listener)

Remove the listener that notifies when the url is changed.
  Parameters: listener - The listener that notifies when the url is changed.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
