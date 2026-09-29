Package [ro.sync.exml.plugin.urlstreamhandler](package-summary.md)

# Interface CacheableUrlConnection
    @API(src=PUBLIC, type=EXTENDABLE) public interface CacheableUrlConnection
Marker interface that should be implemented by a URL connection and which instructs oXygen that it makes sense to cache data read from such a connection. For example, a connection that connects to a remote server to retrieve data should implement this interface while a connection that reads data from the local file system may not.

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
