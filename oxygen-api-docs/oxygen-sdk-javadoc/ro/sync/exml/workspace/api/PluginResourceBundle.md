Package [ro.sync.exml.workspace.api](package-summary.md)

# Interface PluginResourceBundle
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface PluginResourceBundle
Bundle used to translate specific messages in the language set in the editor's preferences. The translation file must be located in a directory named "i18n", placed in the plugin's root directory. The translation file name must be: **translation\*.xml** Here is a small sample of an translation XML file structure:
```


 <?xml version="1.0" encoding="UTF-8"?>
 <translation>
    <key value="key_name">
       <comment>key description</comment>
      <val lang="en_US">en_US_translation</val>
      <val lang="de_DE">de_DE_translation</val>
      <val lang="fr_FR">fr_FR_translation</val>
      <val lang="ja_JP">ja_JP_translation</val>
      <val lang="nl_NL">nl_NL_translation</val>
  </key>
 </translation>


```

  Since: 18.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getMessage](#getMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) messageKey)
Get the internationalized message corresponding to the specified key.
  boolean [hasMessage](#hasMessage(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) messageKey)
Check if a translation is available for a message key.

## Method Details

### getMessage

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) messageKey)

Get the internationalized message corresponding to the specified key. As a fallback if a message is not found the key value is returned.
  Parameters: messageKey - The key of the message which is accessed. In the following translation XML sample, the "messageKey" that you can be used to get the message translation is "key_name":
```


 <?xml version="1.0" encoding="UTF-8"?>
 <translation>
     <languageList>
       <language description="English US" lang="en_US"/>
       <language description="German" lang="de_DE"/>
       <language description="French" lang="fr_FR"/>
    </languageList>
    <key value="key_name1">
       <comment>key description1</comment>
      <val lang="en_US">en_US_translation1</val>
      <val lang="de_DE">de_DE_translation1</val>
      <val lang="fr_FR">fr_FR_translation1</val>
  </key>
   <key value="key_name2">
       <comment>key description2</comment>
      <val lang="en_US">en_US_translation2</val>
      <val lang="de_DE">de_DE_translation2</val>
      <val lang="fr_FR">fr_FR_translation2</val>
  </key>
  ........................
 </translation>


```
 Returns: The internationalized message representing the specified key in the language of this bundle. As a fallback if a message is not found the key value is returned. Throws: [ClassCastException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassCastException.html) - if the object found for the given key is not a string
### hasMessage

boolean hasMessage([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) messageKey)

Check if a translation is available for a message key.
  Parameters: messageKey - The message key Returns: true if the message is available for the key. Since: 28 \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\* EXPERIMENTAL - Subject to change \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Please note that this API is not marked as final and it can change in one of the next versions of the application. If you have suggestions, comments about it, please let us know.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
