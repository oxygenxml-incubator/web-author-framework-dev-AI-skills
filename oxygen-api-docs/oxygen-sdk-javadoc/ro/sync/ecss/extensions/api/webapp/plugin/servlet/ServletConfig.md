Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet](package-summary.md)

# Interface ServletConfig
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ServletConfig
ServletConfig interface inspired from HTTP Servlet 5.0.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getInitParameter](#getInitParameter(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Gets the value of the initialization parameter with the given name.
  [Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getInitParameterNames](#getInitParameterNames())()
Returns the names of the servlet's initialization parameters as an Enumeration of Stringobjects, or an empty Enumeration if the servlet has no initialization parameters.
  [ServletContext](ServletContext.md) [getServletContext](#getServletContext())()
Returns a reference to the [ServletContext](ServletContext.md) in which the caller is executing.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getServletName](#getServletName())()
Returns the name of this servlet instance.

## Method Details

### getServletName

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getServletName()

Returns the name of this servlet instance. The name may be provided via server administration, assigned in the web application deployment descriptor, or for an unregistered (and thus unnamed) servlet instance it will be the servlet's class name.
  Returns: the name of the servlet instance
### getServletContext

[ServletContext](ServletContext.md) getServletContext()

Returns a reference to the [ServletContext](ServletContext.md) in which the caller is executing.
  Returns: a [ServletContext](ServletContext.md) object, used by the caller to interact with its servlet container See Also:
        * [ServletContext](ServletContext.md)

### getInitParameter

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getInitParameter([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Gets the value of the initialization parameter with the given name.
  Parameters: name - the name of the initialization parameter whose value to get Returns: a String containing the value of the initialization parameter, or null if the initialization parameter does not exist
### getInitParameterNames

[Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getInitParameterNames()

Returns the names of the servlet's initialization parameters as an Enumeration of Stringobjects, or an empty Enumeration if the servlet has no initialization parameters.
  Returns: an Enumeration of String objects containing the names of the servlet's initialization parameters
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
