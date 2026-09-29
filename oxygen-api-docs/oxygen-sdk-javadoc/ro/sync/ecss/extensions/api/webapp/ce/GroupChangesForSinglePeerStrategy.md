Package [ro.sync.ecss.extensions.api.webapp.ce](package-summary.md)

# Interface GroupChangesForSinglePeerStrategy
    All Superinterfaces: [SaveStrategy](SaveStrategy.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface GroupChangesForSinglePeerStrategyextends [SaveStrategy](SaveStrategy.md)
Details required when saving a concurrently edited document. Used to write document snapshots with changes made from the last save, where each snapshot is capturing changes made by a single peer. It facilitates tracking precise authorship of changes, each written revision containing changes by only one author.
  Since: 23.1.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) [openConnection](#openConnection(java.net.URL,ro.sync.ecss.extensions.api.webapp.ce.PeerContext))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) documentUrl, [PeerContext](PeerContext.md) author)
This method will be called whenever a peer within a concurrent editing session triggers either a save or a auto-save.

## Method Details

### openConnection

[URLConnection](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URLConnection.html) openConnection([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) documentUrl, [PeerContext](PeerContext.md) author)throws [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html)

This method will be called whenever a peer within a concurrent editing session triggers either a save or a auto-save. It facilitates storing revisions for each peer individually.
  Parameters: documentUrl - The document URL. Note that it has the UserInfo stripped. author - The context of peer whose only changes are about to be saved onto the URL connection. Returns: A connection where to write the new revision. Throws: [IOException](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/IOException.html) - If fails to open the connect.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
