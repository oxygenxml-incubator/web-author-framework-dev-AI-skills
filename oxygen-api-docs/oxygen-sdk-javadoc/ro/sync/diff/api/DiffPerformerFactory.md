Package [ro.sync.diff.api](package-summary.md)

# Class DiffPerformerFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.diff.api.DiffPerformerFactory
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class DiffPerformerFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Factory used to create a difference performer, used to compare two resources using different algorithms and options.

## Constructor Summary
 Constructors
Constructor

Description
 [DiffPerformerFactory](#%3Cinit%3E())()

## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [AuthorDifferencePerformer](AuthorDifferencePerformer.md) [createAuthorDiffPerformer](#createAuthorDiffPerformer())()
Create an Author difference performer.
  static [DifferencePerformer](DifferencePerformer.md) [createDiffPerformer](#createDiffPerformer())()
Create difference performer.
  static void [registerLicenseKey](#registerLicenseKey(java.io.Reader))([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) licenseReader)
The license key reader to the diff performer factory.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DiffPerformerFactory

public DiffPerformerFactory()

## Method Details

### createDiffPerformer

public static [DifferencePerformer](DifferencePerformer.md) createDiffPerformer() throws [DiffException](DiffException.md)

Create difference performer.
  Returns: a difference performer that can be used to compare two resources using different algorithms and options. Throws: [DiffException](DiffException.md) - When it fails to create the diff performer.
### createAuthorDiffPerformer

public static [AuthorDifferencePerformer](AuthorDifferencePerformer.md) createAuthorDiffPerformer() throws [DiffException](DiffException.md)

Create an Author difference performer.
  Returns: a difference performer that can be used to compare Author documents using different algorithms and options. Throws: [DiffException](DiffException.md) - When it fails to create the diff performer.
### registerLicenseKey

public static void registerLicenseKey([Reader](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/Reader.html) licenseReader)throws [DiffException](DiffException.md)

The license key reader to the diff performer factory.
  Parameters: licenseReader - The reader from where the license should be read. Throws: [DiffException](DiffException.md) - Thrown if the license could not be read.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
