Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet.http](package-summary.md)

# Interface HttpSession
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface HttpSession
HttpSession interface inspired from HTTP Servlet 5.0. See also: [SessionStore](../../../SessionStore.md) [WebappPluginWorkspace.getSessionStore()](../../../access/WebappPluginWorkspace.md#getSessionStore())
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getId](#getId())()
Returns a string containing the unique identifier assigned to this session.

## Method Details

### getId

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getId()

Returns a string containing the unique identifier assigned to this session. The identifier is assigned by the servlet container and is implementation dependent.
  Returns: a string specifying the identifier assigned to this session
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
