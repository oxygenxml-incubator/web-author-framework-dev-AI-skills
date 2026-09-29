Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface ReferenceErrorResolver
    All Known Implementing Classes: [ReferenceErrorResolverExt](ReferenceErrorResolverExt.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface ReferenceErrorResolver
Resolver for errors concerning references. It will offer solutions for solving the current reference error.

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 void [resolveError](#resolveError(ro.sync.ecss.extensions.api.AuthorAccess))([AuthorAccess](AuthorAccess.md) authorAccess)
Offers solutions to the current reference error.

## Method Details

### resolveError

void resolveError([AuthorAccess](AuthorAccess.md) authorAccess)

Offers solutions to the current reference error.
  Parameters: authorAccess - Access to the author page.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
