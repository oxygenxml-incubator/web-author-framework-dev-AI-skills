Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface AuthorPseudoClassController
    All Known Subinterfaces: [AuthorDocumentController](AuthorDocumentController.md)   @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface AuthorPseudoClassController
Controls setting and resetting pseudo classes.
  Since: 23
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [removePseudoClass](#removePseudoClass(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)
Removes a pseudo class from the given element.
  void [setPseudoClass](#setPseudoClass(java.lang.String,ro.sync.ecss.extensions.api.node.AuthorElement))([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)
Sets a pseudo class in the specified element.

## Method Details

### setPseudoClass

void setPseudoClass([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)

Sets a pseudo class in the specified element.

This change \*IS NOT\* subject to undo/redo.

What is good for: You can use a non standard (custom) pseudo class to impose a style change on a specific element. For instance you can have CSS styles matching a custom pseudo-class, like the one below:

```

   section:access-control-user {
      display:block;
   } 
   section {
      display:none;
   } 

```

By setting the pseudoClass "access-control-user", the element section will become visible.

Another example:

```

   *:caret-visited {
      color:red;
   } 

```

You could create an [AuthorCaretListener](AuthorCaretListener.md) that sets the caret-visited pseudo class to the element at the caret location. The effect will be that all the elements traversed by the caret become red.
  Parameters: pseudoClass - Name of the pseudo class being set. element - The [AuthorElement](node/AuthorElement.md) whose attribute is changing. Since: 15.2
### removePseudoClass

void removePseudoClass([String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) pseudoClass, [AuthorElement](node/AuthorElement.md) element)

Removes a pseudo class from the given element. This change \*IS NOT\* subject to undo/redo.
  Parameters: pseudoClass - Name of the pseudo class being set. element - The [AuthorElement](node/AuthorElement.md) whose attribute will be removed. Since: 15.2
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
