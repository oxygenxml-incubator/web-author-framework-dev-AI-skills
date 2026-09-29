Package [ro.sync.exml.workspace.api.standalone.project](package-summary.md)

# Interface ProjectChangeListener
    @API(type=EXTENDABLE, src=PUBLIC) public interface ProjectChangeListener
Project change listener. Gets notified when another project is loaded.
  Since: 21.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [projectChanged](#projectChanged(java.net.URL,java.net.URL))([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) oldProjectURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) newProjectURL)
The project has changed.

## Method Details

### projectChanged

void projectChanged([URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) oldProjectURL, [URL](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/net/URL.html) newProjectURL)

The project has changed.
  Parameters: oldProjectURL - The URL of the old project. newProjectURL - The URL of the new project.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
