Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorResourceBundle
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorResourceBundle
Gives access to translate keys. The translation files should all be located in a separate directory (usually named "i18n") in the specific framework's directory. This particular "i18n" directory should be explicitly added to the document type's class path list in the Document Type Edit dialog. Their names should be formatted like this: **translation\*.xml**Only one translation file will be used to translate the keys to values. How is this translation file detected? The first file which matches the same GUI language that Oxygen uses in the Preferences will be used. If no such file exists, the first encountered translation will be used. If no such file exists, the methods will return the same key which is given for translation.
  Since: 14
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [composeMessage](#composeMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) descriptionWithEditorVariables)
Compose a message for the given description which may contain more than one keys referenced using editor variables.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Gets a message for the given key from this resource bundle.

## Method Details

### getMessage

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Gets a message for the given key from this resource bundle.
  Parameters: key - The key for the desired string Returns: the string for the given key Throws: [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if key is null
### composeMessage

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) composeMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) descriptionWithEditorVariables)

Compose a message for the given description which may contain more than one keys referenced using editor variables. The key contains "${i18n(key)}" editor variables which will be expanded.
  Parameters: descriptionWithEditorVariables - the key for the desired string. Example: The description: '${i18n(key1)} and ${i18n(key2)}' will be composed to: 'value1 and value2' where 'value1' is obtained by calling getMessage('key1'). Returns: the string for the given key Throws: [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if descriptionWithEditorVariables is null
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
