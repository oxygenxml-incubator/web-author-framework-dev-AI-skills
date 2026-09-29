Package [ro.sync.ecss.extensions.api.webapp.doctype](package-summary.md)

# Class DocumentTypeInfoRepository

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.doctype.DocumentTypeInfoRepository
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class DocumentTypeInfoRepository extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class used to retrieve information about the registered document types.

## Constructor Summary
 Constructors
Constructor

Description
 [DocumentTypeInfoRepository](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentTypeInfo](DocumentTypeInfo.md)> [getAllDocumentTypeInfos](#getAllDocumentTypeInfos())()
Returns information about all document types.
  [DocumentTypeInfo](DocumentTypeInfo.md) [getDocumentTypeInfo](#getDocumentTypeInfo(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)
Returns information about the document type with the given id.
  [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getErrorDocumentTypes](#getErrorDocumentTypes())()
Finds all the .framework files that for some reason could not be loaded.
  static [DocumentTypeInfoRepository](DocumentTypeInfoRepository.md) [getInstance](#getInstance())()

 void [removeErrorDocumentType](#removeErrorDocumentType(java.io.File))([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkDescriptor)
Removes the errorDocumentType with the given descriptor path from the errors list.
  static void [setInstance](#setInstance(ro.sync.ecss.extensions.api.webapp.doctype.DocumentTypeInfoRepository))([DocumentTypeInfoRepository](DocumentTypeInfoRepository.md) instance)

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DocumentTypeInfoRepository

public DocumentTypeInfoRepository()

## Method Details

### getInstance

public static [DocumentTypeInfoRepository](DocumentTypeInfoRepository.md) getInstance()
  Returns: Returns the instance.
### setInstance

public static void setInstance([DocumentTypeInfoRepository](DocumentTypeInfoRepository.md) instance)
  Parameters: instance - The instance to set.
### getDocumentTypeInfo

public [DocumentTypeInfo](DocumentTypeInfo.md) getDocumentTypeInfo([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) id)

Returns information about the document type with the given id.
  Parameters: id - The id of the document type. Returns: Information about the document type.
### getAllDocumentTypeInfos

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[DocumentTypeInfo](DocumentTypeInfo.md)> getAllDocumentTypeInfos()

Returns information about all document types.
  Returns: Information about all document types.
### getErrorDocumentTypes

public [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getErrorDocumentTypes()

Finds all the .framework files that for some reason could not be loaded.
  Returns: a list of all the .framework file that could not be loaded.
### removeErrorDocumentType

public void removeErrorDocumentType([File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/File.html) frameworkDescriptor)

Removes the errorDocumentType with the given descriptor path from the errors list.
  Parameters: frameworkDescriptor - the .framework file.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
