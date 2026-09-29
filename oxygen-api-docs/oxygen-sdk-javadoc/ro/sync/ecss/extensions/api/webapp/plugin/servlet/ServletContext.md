Package [ro.sync.ecss.extensions.api.webapp.plugin.servlet](package-summary.md)

# Interface ServletContext
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface ServletContext
ServletContext interface inspired from HTTP Servlet 5.0.
  Since: 26
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getAttribute](#getAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Returns the servlet container attribute with the given name, or null if there is no attribute by that name.
  [Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> [getAttributeNames](#getAttributeNames())()
Returns an Enumeration containing the attribute names available within this ServletContext.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getContextPath](#getContextPath())()
Returns the context path of the web application.
  [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [getRealPath](#getRealPath(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path)
Returns a String containing the real path for a given virtual path.
  void [removeAttribute](#removeAttribute(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)
Removes the attribute with the given name from this ServletContext.
  void [setAttribute](#setAttribute(java.lang.String,java.lang.Object))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) object)
Binds an object to a given attribute name in this ServletContext.

## Method Details

### getRealPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getRealPath([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) path)

Returns a String containing the real path for a given virtual path. For example, the path "/index.html" returns the absolute file path on the server's filesystem would be served by a request for "http://host/contextPath/index.html", where contextPath is the context path of this ServletContext.. The real path returned will be in a form appropriate to the computer and operating system on which the servlet container is running, including the proper path separators. This method returns null if the servlet container cannot translate the virtual path to a real path for any reason (such as when the content is being made available from a .war archive).
  Parameters: path - String specifying a virtual path Returns: a String specifying the real path, or null if the translation cannot be performed
### getContextPath

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) getContextPath()

Returns the context path of the web application. The context path is the portion of the request URI that is used to select the context of the request. The context path always comes first in a request URI. The path starts with a "/" character but does not end with a "/" character. For servlets in the default (root) context, this method returns "". It is possible that a servlet container may match a context by more than one context path. In such cases the HttpServletRequest.getContextPath() will return the actual context path used by the request and it may differ from the path returned by this method. The context path returned by this method should be considered as the prime or preferred context path of the application.
  Returns: The context path of the web application, or "" for the default (root) context
### getAttribute

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Returns the servlet container attribute with the given name, or null if there is no attribute by that name.
An attribute allows a servlet container to give the servlet additional information not already provided by this interface. See your server documentation for information about its attributes. A list of supported attributes can be retrieved using getAttributeNames.

The attribute is returned as a java.lang.Object or some subclass.

Attribute names should follow the same convention as package names. The Jakarta Servlet specification reserves names matching java.\*, javax.\*, and sun.\*.

  Parameters: name - a String specifying the name of the attribute Returns: an Object containing the value of the attribute, or null if no attribute exists matching the given name. Throws: [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the argument name is null See Also:
        * [getAttributeNames()](#getAttributeNames())

### getAttributeNames

[Enumeration](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Enumeration.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html)> getAttributeNames()

Returns an Enumeration containing the attribute names available within this ServletContext.
Use the [getAttribute(java.lang.String)](#getAttribute(java.lang.String)) method with an attribute name to get the value of an attribute.

  Returns: an Enumeration of attribute names See Also:
        * [getAttribute(java.lang.String)](#getAttribute(java.lang.String))

### setAttribute

void setAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name, [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) object)

Binds an object to a given attribute name in this ServletContext. If the name specified is already used for an attribute, this method will replace the attribute with the new to the new attribute.
If listeners are configured on the ServletContext the container notifies them accordingly.

If a null value is passed, the effect is the same as calling removeAttribute().

Attribute names should follow the same convention as package names. The Jakarta Servlet specification reserves names matching java.\*, javax.\*, and sun.\*.

  Parameters: name - a String specifying the name of the attribute object - an Object representing the attribute to be bound Throws: [NullPointerException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/NullPointerException.html) - if the name parameter is null
### removeAttribute

void removeAttribute([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) name)

Removes the attribute with the given name from this ServletContext. After removal, subsequent calls to [getAttribute(java.lang.String)](#getAttribute(java.lang.String)) to retrieve the attribute's value will return null.
If listeners are configured on the ServletContext the container notifies them accordingly.

  Parameters: name - a String specifying the name of the attribute to be removed
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
