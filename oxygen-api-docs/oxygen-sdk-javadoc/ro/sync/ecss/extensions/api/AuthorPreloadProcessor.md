Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorPreloadProcessor
    @API(type=EXTENDABLE, src=PUBLIC) public interface AuthorPreloadProcessor
This processor is notified before the Author document is loaded and renderer. It can be used to set various pseudo classes to elements before the content is presented visually.
  Since: 23.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [documentAboutToBeLoaded](#documentAboutToBeLoaded(ro.sync.ecss.extensions.api.node.AuthorDocument,ro.sync.ecss.extensions.api.AuthorPseudoClassController))([AuthorDocument](node/AuthorDocument.md) document, [AuthorPseudoClassController](AuthorPseudoClassController.md) pseudoClassController)
A document is about to be loaded.

## Method Details

### documentAboutToBeLoaded

void documentAboutToBeLoaded([AuthorDocument](node/AuthorDocument.md) document, [AuthorPseudoClassController](AuthorPseudoClassController.md) pseudoClassController)

A document is about to be loaded.
  Parameters: document - The document. pseudoClassController - The pseudo class controller. Use this interface to set or remove pseudo classes from elements.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
