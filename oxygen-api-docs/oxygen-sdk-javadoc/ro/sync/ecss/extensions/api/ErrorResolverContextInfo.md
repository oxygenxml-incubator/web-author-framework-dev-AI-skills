Package [ro.sync.ecss.extensions.api](package-summary.md)

# Class ErrorResolverContextInfo

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.ErrorResolverContextInfo
   @API(type=EXTENDABLE, src=PUBLIC) public class ErrorResolverContextInfo extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
Class that contains some information about the current error.

## Constructor Summary
 Constructors
Constructor

Description
 [ErrorResolverContextInfo](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Constructor.
  [ErrorResolverContextInfo](#%3Cinit%3E(ro.sync.ecss.extensions.api.AuthorAccess,ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorNode](node/AuthorNode.md) contextNode)
Constructor.

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [AuthorAccess](AuthorAccess.md) [getAuthorAccess](#getAuthorAccess())()
Obtain the author access.
  [AuthorNode](node/AuthorNode.md) [getContextNode](#getContextNode())()
Get the error context node.
  void [setAuthorAccess](#setAuthorAccess(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Sets the author access.
  void [setContextNode](#setContextNode(ro.sync.ecss.extensions.api.node.AuthorNode))([AuthorNode](node/AuthorNode.md) contextNode)
Set the error context node.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### ErrorResolverContextInfo

public ErrorResolverContextInfo([AuthorAccess](AuthorAccess.md) authorAccess)

Constructor.
  Parameters: authorAccess - The [AuthorAccess](AuthorAccess.md).
### ErrorResolverContextInfo

public ErrorResolverContextInfo([AuthorAccess](AuthorAccess.md) authorAccess, [AuthorNode](node/AuthorNode.md) contextNode)

Constructor.
  Parameters: authorAccess - The [AuthorAccess](AuthorAccess.md). contextNode - The error context node.
## Method Details

### getAuthorAccess

public [AuthorAccess](AuthorAccess.md) getAuthorAccess()

Obtain the author access.
  Returns: Returns the author access.
### setAuthorAccess

public void setAuthorAccess([AuthorAccess](AuthorAccess.md) authorAccess)

Sets the author access.
  Parameters: authorAccess - The new author access.
### getContextNode

public [AuthorNode](node/AuthorNode.md) getContextNode()

Get the error context node.
  Returns: Returns the error context node.
### setContextNode

public void setContextNode([AuthorNode](node/AuthorNode.md) contextNode)

Set the error context node.
  Parameters: contextNode - The error context node.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
