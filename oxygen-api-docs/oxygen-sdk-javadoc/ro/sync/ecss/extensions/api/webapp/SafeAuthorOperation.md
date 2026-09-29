Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Interface SafeAuthorOperation
    @API(type=EXTENDABLE, src=PUBLIC) [@Deprecated](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Deprecated.html) public interface SafeAuthorOperation Deprecated.
This interface is not used anymore as marker interface for operations that can be invoked via REST API with user supplied arguments. These AuthorOperations must be instead annotated with [WebappRestSafe](WebappRestSafe.md) annotation.

In Web Author, [AuthorOperation](../AuthorOperation.md)s that implement this marker interface can be invoked via a REST API with user supplied arguments. An operation that simply inserts an XML fragment would be considered safe, while one that executes some JavaScript code provided by the user would be considered unsafe.
  Since: 19.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
