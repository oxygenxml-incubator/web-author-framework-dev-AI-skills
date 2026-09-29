Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface SessionStore
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface SessionStore
A per-session key value store (sessionId, key, value). The invalidate method will be called when a session expires. Users of this interface do not need to call this method directly. All implementations should be thread-safe.
  Since: 20.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 <T> T [computeIfAbsent](#computeIfAbsent(java.lang.String,java.lang.String,java.util.function.Supplier))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<T> supplier)
If the specified key is not already associated with a value (or is mapped to null), attempts to compute its value using the given mapping function and enters it into this store unless null.
  <T> T [computeIfAbsentWithoutSessionCookieRefresh](#computeIfAbsentWithoutSessionCookieRefresh(java.lang.String,java.lang.String,java.util.function.Supplier))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<T> supplier)
If the specified key is not already associated with a value (or is mapped to null), attempts to compute its value using the given mapping function and enters it into this store unless null.
  <T> T [get](#get(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Returns the value to which the specified key is mapped, or null if the key is not mapped to any value.
  <T> T [getAndDel](#getAndDel(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Returns the value to which the specified key is mapped, or null if the key is not mapped to any value.
  void [invalidate](#invalidate(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId)
Removes all keys associated with the given session id.
  void [invalidateAll](#invalidateAll())()
Removes all keys from the store.
  <T> void [put](#put(java.lang.String,java.lang.String,T))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)
Associates the specified value with the specified sessionId and key.
  <T> T [putIfAbsent](#putIfAbsent(java.lang.String,java.lang.String,T))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)
If the specified key is not already associated with a value associates it with the given value and returns null, else returns the current value.
  <T> T [putIfAbsentWithoutSessionCookieRefresh](#putIfAbsentWithoutSessionCookieRefresh(java.lang.String,java.lang.String,T))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)
If the specified key is not already associated with a value associates it with the given value and returns null, else returns the current value.
  <T> void [putWithoutSessionCookieRefresh](#putWithoutSessionCookieRefresh(java.lang.String,java.lang.String,T))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)
Associates the specified value with the specified sessionId and key.
  void [refreshSessionCookie](#refreshSessionCookie(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId)
Before a login, or before storing any data on the user session that gives additional privileges, it is recommended to refresh the session cookie to prevent session fixation attacks.
  void [remove](#remove(java.lang.String,java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)
Removes the mapping for a key from this store.

## Method Details

### get

<T> T get([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Returns the value to which the specified key is mapped, or null if the key is not mapped to any value. If the value is not an instance of the requested type T a [ClassCastException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassCastException.html) will be thrown.
  Parameters: sessionId - The id of the session for which to return the value of a key. key - The key whose associated value is to be returned. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. Returns: The value to which the specified key is mapped, or null if the key is not mapped to any value.
### getAndDel

<T> T getAndDel([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Returns the value to which the specified key is mapped, or null if the key is not mapped to any value. Deletes the mapped value before returning. If the value is not an instance of the requested type T a [ClassCastException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassCastException.html) will be thrown.
  Parameters: sessionId - The id of the session for which to return the value of a key. key - The key whose associated value is to be returned. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. Returns: The value to which the specified key is mapped, or null if the key is not mapped to any value.
### computeIfAbsent

<T> T computeIfAbsent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<T> supplier)

If the specified key is not already associated with a value (or is mapped to null), attempts to compute its value using the given mapping function and enters it into this store unless null. If the computed value is not an instance of the requested type T a [ClassCastException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassCastException.html) will be thrown. This method will refresh the session cookie. See [refreshSessionCookie(String)](#refreshSessionCookie(java.lang.String)).
  Parameters: sessionId - The id of the session for which to return the value of a key. key - The key with which the specified value is to be associated. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. supplier - The function to supply a value. Returns: The current (existing or computed) value associated with the specified key, or null if the computed value is null.
### computeIfAbsentWithoutSessionCookieRefresh

<T> T computeIfAbsentWithoutSessionCookieRefresh([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, [Supplier](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/function/Supplier.html)<T> supplier)

If the specified key is not already associated with a value (or is mapped to null), attempts to compute its value using the given mapping function and enters it into this store unless null. If the computed value is not an instance of the requested type T a [ClassCastException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassCastException.html) will be thrown. This method will not refresh the session cookie. See [refreshSessionCookie(String)](#refreshSessionCookie(java.lang.String)). \*
  Parameters: sessionId - The id of the session for which to return the value of a key. key - The key with which the specified value is to be associated. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. supplier - The function to supply a value. Returns: The current (existing or computed) value associated with the specified key, or null if the computed value is null. Since: 26.0
### putIfAbsent

<T> T putIfAbsent([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)

If the specified key is not already associated with a value associates it with the given value and returns null, else returns the current value. If the value is not an instance of the requested type T a [ClassCastException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassCastException.html) will be thrown. This method will refresh the session cookie. See [refreshSessionCookie(String)](#refreshSessionCookie(java.lang.String)). \*
  Parameters: sessionId - The session id with which the specified value is to be associated. key - The key with which the specified value is to be associated. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. value - The value associated with the specified keys. Returns: The current value associated with the specified keys.
### putIfAbsentWithoutSessionCookieRefresh

<T> T putIfAbsentWithoutSessionCookieRefresh([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)

If the specified key is not already associated with a value associates it with the given value and returns null, else returns the current value. If the value is not an instance of the requested type T a [ClassCastException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/ClassCastException.html) will be thrown. This method will not refresh the session cookie. See [refreshSessionCookie(String)](#refreshSessionCookie(java.lang.String)). \*
  Parameters: sessionId - The session id with which the specified value is to be associated. key - The key with which the specified value is to be associated. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. value - The value associated with the specified keys. Returns: The current value associated with the specified keys. Since: 26.0
### put

<T> void put([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)

Associates the specified value with the specified sessionId and key. If the store previously contained a mapping for the sessionId and key, the old value is replaced by the specified value. This method will refresh the session cookie. See [refreshSessionCookie(String)](#refreshSessionCookie(java.lang.String)).
  Parameters: sessionId - The session id with which the specified value is to be associated. key - The key with which the specified value is to be associated. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. value - The value to be associated with the specified keys.
### putWithoutSessionCookieRefresh

<T> void putWithoutSessionCookieRefresh([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key, T value)

Associates the specified value with the specified sessionId and key. If the store previously contained a mapping for the sessionId and key, the old value is replaced by the specified value. This method will not refresh the session cookie. See [refreshSessionCookie(String)](#refreshSessionCookie(java.lang.String)).
  Parameters: sessionId - The session id with which the specified value is to be associated. key - The key with which the specified value is to be associated. The key should be name-spaced because this store may be used by multiple plugins. ex: plugin-name.key-name. value - The value to be associated with the specified keys. Since: 26.0
### remove

void remove([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId, [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) key)

Removes the mapping for a key from this store.
  Parameters: sessionId - The session id for which to remove the associated value. key - The key for which to remove the associated value.
### invalidate

void invalidate([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId)

Removes all keys associated with the given session id.
  Parameters: sessionId - The session id for which to invalidate all keys.
### refreshSessionCookie

void refreshSessionCookie([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) sessionId)

Before a login, or before storing any data on the user session that gives additional privileges, it is recommended to refresh the session cookie to prevent session fixation attacks. If you refresh the session cookie on a HTTP request, all concurrent requests will fail with status code 400. To limit this impact it is recommended to call this method only on HTTP requests that take very a short time to complete.
  Parameters: sessionId - The ID of the session. Since: 26.0
### invalidateAll

void invalidateAll()

Removes all keys from the store.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
