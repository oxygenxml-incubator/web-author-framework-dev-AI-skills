Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Interface MoveRenameResult
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface MoveRenameResult
Result of a move rename operation

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> [getModifiedResources](#getModifiedResources())()

 boolean [isSuccesfull](#isSuccesfull())()

## Method Details

### isSuccesfull

boolean isSuccesfull()
  Returns: true if the move rename was successfull
### getModifiedResources

[List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html)> getModifiedResources()
  Returns: the list of modified resources.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
