Package [ro.sync.ecss.extensions.api.webapp.license](package-summary.md)

# Class LicenseEnforcerFilter

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.license.LicenseEnforcerFilter
   All Implemented Interfaces: javax.servlet.Filter   @API(type=NOT_EXTENDABLE, src=PRIVATE) public class LicenseEnforcerFilter extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements javax.servlet.Filter
A servlet filter that MUST be used to license the WebApp. The path of the license file is specified by the [LICENSE_PATH](#LICENSE_PATH)filter parameter configured in the 'web.xml' file. The path is relative to the root of the archive. If not set, the default location is [LICENSE_DEFAULT_PATH](#LICENSE_DEFAULT_PATH).

## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LICENSE_DEFAULT_PATH](#LICENSE_DEFAULT_PATH)
The default path for the license file.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [LICENSE_PATH](#LICENSE_PATH)
The filter parameter specifying the license path.

## Constructor Summary
 Constructors
Constructor

Description
 [LicenseEnforcerFilter](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 void [destroy](#destroy())()

 void [doFilter](#doFilter(javax.servlet.ServletRequest,javax.servlet.ServletResponse,javax.servlet.FilterChain))(javax.servlet.ServletRequest req, javax.servlet.ServletResponse resp, javax.servlet.FilterChain chain)
The method that takes care of executing the request on behalf of the correct user.
  void [init](#init(javax.servlet.FilterConfig))(javax.servlet.FilterConfig config)
Initializes the filter.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Field Details

### LICENSE_PATH

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LICENSE_PATH

The filter parameter specifying the license path.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.license.LicenseEnforcerFilter.LICENSE_PATH)

### LICENSE_DEFAULT_PATH

public static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) LICENSE_DEFAULT_PATH

The default path for the license file.
  See Also:
        * [Constant Field Values](../../../../../../../constant-values.md#ro.sync.ecss.extensions.api.webapp.license.LicenseEnforcerFilter.LICENSE_DEFAULT_PATH)

## Constructor Details

### LicenseEnforcerFilter

public LicenseEnforcerFilter()

## Method Details

### destroy

public void destroy()
  Specified by: destroy in interface javax.servlet.Filter See Also:
        * Filter.destroy()

### doFilter

public void doFilter(javax.servlet.ServletRequest req, javax.servlet.ServletResponse resp, javax.servlet.FilterChain chain)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html), javax.servlet.ServletException

The method that takes care of executing the request on behalf of the correct user.
  Specified by: doFilter in interface javax.servlet.Filter Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) javax.servlet.ServletException
### init

public void init(javax.servlet.FilterConfig config)throws javax.servlet.ServletException

Initializes the filter.
  Specified by: init in interface javax.servlet.Filter Throws: javax.servlet.ServletException
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
