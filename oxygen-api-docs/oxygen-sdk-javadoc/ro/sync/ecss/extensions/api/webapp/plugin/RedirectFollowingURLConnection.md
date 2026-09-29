Package [ro.sync.ecss.extensions.api.webapp.plugin](package-summary.md)

# Interface RedirectFollowingURLConnection
    @API(src=PUBLIC, type=EXTENDABLE) public interface RedirectFollowingURLConnection
Marker interface that indicates that the URLConnection follows redirects. Let's assume you want to open a document identified by an URL docURL. If your URLConnection implements this interface, instead of using docURL as the system ID of the edited document, oXygen will call connection.getURL() and use that URL instead. This interface is useful if the URL used to open the document is a proxy URL which will redirect to the actual document URL.
  Since: 18
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
