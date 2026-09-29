Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface GroupChangesForMultiplePeersStrategy
    All Superinterfaces: [SaveStrategy](SaveStrategy.md)   All Known Implementing Classes: [DefaultSaveStrategy](DefaultSaveStrategy.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface GroupChangesForMultiplePeersStrategyextends [SaveStrategy](SaveStrategy.md)
Details required when saving a concurrently edited document. Used to write a single snapshot of the document with changes made from the last save, where the snapshot may be capturing changes made by multiple peers. It facilitates a minimum number of writes to the file server per save.
  Since: 23.1.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) [openConnection](#openConnection(java.net.URL,ro.sync.ecss.extensions.api.webapp.ce.PeerContext,java.util.List))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) documentUrl, [PeerContext](PeerContext.md) committer, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PeerContext](PeerContext.md)> authors)
This method will be called whenever a peer within a concurrent editing session triggers either a save or a auto-save.

## Method Details

### openConnection

[URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) openConnection([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) documentUrl, [PeerContext](PeerContext.md) committer, [List](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/List.html)<[PeerContext](PeerContext.md)> authors)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

This method will be called whenever a peer within a concurrent editing session triggers either a save or a auto-save. Called a single time for each document, allowing a minimum number of writes to the file server. It facilitates storing a revision for all peers together, writing only once per save to the file server.
  Parameters: documentUrl - The document URL. May be used to directly open a connection to the CMS on behalf of the committer. Note that it has the UserInfo of the committer. committer - The context of the peer that triggered either a save or a auto-save. authors - The context of peers whose changes are about to be saved onto the URL connection. Note that committer may or may not be an author. Returns: A connection where to write the new revision. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If fails to open the connect.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
