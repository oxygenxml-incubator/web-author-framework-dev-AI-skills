Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface AuthorIdIndex<T>
    Type Parameters: T - The type of the object to be indexed.   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorIdIndex<T>
An index that maps from IDs to objects and viceversa.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 long [getId](#getId(T))([T](AuthorIdIndex.md) object)
Get the id of the given object or a fresh one if none is assigned already.
  [Long](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Long.html) [getIdIfExists](#getIdIfExists(T))([T](AuthorIdIndex.md) object)
Get the id of the given object, or null if the object was not assigned an ID.
  [T](AuthorIdIndex.md) [getObjectById](#getObjectById(long))(long id)
Returns the object with a specified id or null if none exists.

## Method Details

### getObjectById

[T](AuthorIdIndex.md) getObjectById(long id)

Returns the object with a specified id or null if none exists.
  Parameters: id - the id. Returns: the object with the specified id.
### getId

long getId([T](AuthorIdIndex.md) object)

Get the id of the given object or a fresh one if none is assigned already. If this index has not assigned an id already to the given object, a unique id is assigned and returned.
  Parameters: object - The object. Returns: the id associated with the object.
### getIdIfExists

[Long](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Long.html) getIdIfExists([T](AuthorIdIndex.md) object)

Get the id of the given object, or null if the object was not assigned an ID.
  Parameters: object - The object. Returns: the id associated with the object, or null if the ID does not exist.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
