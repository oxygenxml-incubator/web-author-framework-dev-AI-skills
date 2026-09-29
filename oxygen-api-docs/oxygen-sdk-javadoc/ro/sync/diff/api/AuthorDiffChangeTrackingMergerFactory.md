Package [ro.sync.diff.api](package-summary.md)

# Class AuthorDiffChangeTrackingMergerFactory

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.diff.api.AuthorDiffChangeTrackingMergerFactory
   @API(type=NOT_EXTENDABLE, src=PUBLIC) public class AuthorDiffChangeTrackingMergerFactory extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Factory for creating mergers with change tracking highlights. A merger can be used to compare XML documents and save the comparison results as a document with tracked changes.
  Since: 26.1
## Method Summary
  All MethodsStatic MethodsConcrete Methods
Modifier and Type

Method

Description
 static [AuthorDiffChangeTrackingMerger](AuthorDiffChangeTrackingMerger.md) [createChangeTrackingMergePerformer](#createChangeTrackingMergePerformer())()
Creates a merger with change tracking highlights for a pair of XML documents compared.
  static [AuthorDiffDirectoriesChangeTrackingMerger](AuthorDiffDirectoriesChangeTrackingMerger.md) [createDirectoryChangeTrackingMergePerformer](#createDirectoryChangeTrackingMergePerformer())()
Creates a merger with change tracking highlights for a pair of directories compared.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Method Details

### createChangeTrackingMergePerformer

public static [AuthorDiffChangeTrackingMerger](AuthorDiffChangeTrackingMerger.md) createChangeTrackingMergePerformer() throws [DiffException](DiffException.md)

Creates a merger with change tracking highlights for a pair of XML documents compared.
  Returns: An Author Difference Merge performer with change tracking highlights. Throws: [DiffException](DiffException.md) - When it fails to create the merger.
### createDirectoryChangeTrackingMergePerformer

public static [AuthorDiffDirectoriesChangeTrackingMerger](AuthorDiffDirectoriesChangeTrackingMerger.md) createDirectoryChangeTrackingMergePerformer() throws [DiffException](DiffException.md)

Creates a merger with change tracking highlights for a pair of directories compared.
  Returns: A Directory Difference Merge performer with change tracking highlights. Throws: [DiffException](DiffException.md) - When it fails to create the merger.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
