Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Class DefaultSaveStrategy

* [java.lang.Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
    * ro.sync.ecss.extensions.api.webapp.ce.DefaultSaveStrategy
   All Implemented Interfaces: [GroupChangesForMultiplePeersStrategy](GroupChangesForMultiplePeersStrategy.md), [SaveStrategy](SaveStrategy.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public final class DefaultSaveStrategy extends [Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)implements [GroupChangesForMultiplePeersStrategy](GroupChangesForMultiplePeersStrategy.md)
Default save strategy used when no save strategy is explicitly specified when creating a room. Saves all changes at once, as the user who triggered the save.
  Since: 23.1.1
## Constructor Summary
 Constructors
Constructor

Description
 [DefaultSaveStrategy](#%3Cinit%3E())()

## Method Summary
  All MethodsInstance MethodsConcrete Methods
Modifier and Type

Method

Description
 [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) [openConnection](#openConnection(java.net.URL,ro.sync.ecss.extensions.api.webapp.ce.PeerContext,java.util.List))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) documentUrl, [PeerContext](PeerContext.md) committer, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PeerContext](PeerContext.md)> authors)
This method will be called whenever a peer within a concurrent editing session triggers either a save or a auto-save.

### Methods inherited from class java.lang.[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)
 [clone](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#clone()), [equals](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object)), [finalize](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#finalize()), [getClass](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#getClass()), [hashCode](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#hashCode()), [notify](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notify()), [notifyAll](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#notifyAll()), [toString](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#toString()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait()), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long)), [wait](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#wait(long,int))
## Constructor Details

### DefaultSaveStrategy

public DefaultSaveStrategy()

## Method Details

### openConnection

public [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) openConnection([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) documentUrl, [PeerContext](PeerContext.md) committer, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PeerContext](PeerContext.md)> authors)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)
 Description copied from interface: [GroupChangesForMultiplePeersStrategy](GroupChangesForMultiplePeersStrategy.md#openConnection(java.net.URL,ro.sync.ecss.extensions.api.webapp.ce.PeerContext,java.util.List))
This method will be called whenever a peer within a concurrent editing session triggers either a save or a auto-save. Called a single time for each document, allowing a minimum number of writes to the file server. It facilitates storing a revision for all peers together, writing only once per save to the file server.
  Specified by: [openConnection](GroupChangesForMultiplePeersStrategy.md#openConnection(java.net.URL,ro.sync.ecss.extensions.api.webapp.ce.PeerContext,java.util.List)) in interface [GroupChangesForMultiplePeersStrategy](GroupChangesForMultiplePeersStrategy.md) Parameters: documentUrl - The document URL. May be used to directly open a connection to the CMS on behalf of the committer. Note that it has the UserInfo of the committer. committer - The context of the peer that triggered either a save or a auto-save. authors - The context of peers whose changes are about to be saved onto the URL connection. Note that committer may or may not be an author. Returns: A connection where to write the new revision. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If fails to open the connect. See Also:
        * [GroupChangesForMultiplePeersStrategy.openConnection(java.net.URL, ro.sync.ecss.extensions.api.webapp.ce.PeerContext, java.util.List)](GroupChangesForMultiplePeersStrategy.md#openConnection(java.net.URL,ro.sync.ecss.extensions.api.webapp.ce.PeerContext,java.util.List))

© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
