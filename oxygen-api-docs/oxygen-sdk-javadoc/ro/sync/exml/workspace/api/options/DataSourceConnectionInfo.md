Package [ro.sync.exml.workspace.api.options](package-summary.md)

# Interface DataSourceConnectionInfo
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DataSourceConnectionInfo
Provides properties values for a Data source.
  Since: 14.1
## Field Summary
 Fields
Modifier and Type

Field

Description
 static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [CONNECTION_NAME](#CONNECTION_NAME)
Property ID for the unique name of the connection.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [DRIVER_NAME](#DRIVER_NAME)
Property ID for the driver name used to access the database.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [HOST_NAME](#HOST_NAME)
Property ID for the host name to connect to.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [INITIAL_DATABASE](#INITIAL_DATABASE)
Property ID for the initial database from server to connect to.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [PORT](#PORT)
Property ID for the port used to connect to host.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [URL](#URL)
Property ID for the URL used to connect to the database.
  static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [WEBDAV_URL](#WEBDAV_URL)
Property ID for the WEBDAV URL.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) [getProperty](#getProperty(java.lang.String))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyId)
Used to return properties values for a data source connection.

## Field Details

### DRIVER_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) DRIVER_NAME

Property ID for the driver name used to access the database. It can not be null.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.options.DataSourceConnectionInfo.DRIVER_NAME)

### HOST_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) HOST_NAME

Property ID for the host name to connect to. For relational databases it can be null.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.options.DataSourceConnectionInfo.HOST_NAME)

### INITIAL_DATABASE

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) INITIAL_DATABASE

Property ID for the initial database from server to connect to. It can be null.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.options.DataSourceConnectionInfo.INITIAL_DATABASE)

### PORT

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) PORT

Property ID for the port used to connect to host. For relational databases can be included into the URL.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.options.DataSourceConnectionInfo.PORT)

### CONNECTION_NAME

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) CONNECTION_NAME

Property ID for the unique name of the connection.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.options.DataSourceConnectionInfo.CONNECTION_NAME)

### URL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) URL

Property ID for the URL used to connect to the database. It can be null.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.options.DataSourceConnectionInfo.URL)

### WEBDAV_URL

static final [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) WEBDAV_URL

Property ID for the WEBDAV URL. Some databases can be accessed using a WEBDAV URL. It can be null.
  See Also:
        * [Constant Field Values](../../../../../../constant-values.md#ro.sync.exml.workspace.api.options.DataSourceConnectionInfo.WEBDAV_URL)

## Method Details

### getProperty

[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html) getProperty([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) propertyId)

Used to return properties values for a data source connection.
  Parameters: propertyId - The property identifier. Returns: The value of the property identified by the propertyId. The propertyId can be one of the Id constants defined in the [DataSourceConnectionInfo](DataSourceConnectionInfo.md).
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
