Package [ro.sync.ecss.extensions.api](package-summary.md)

# Annotation Interface WebappCompatible
    @API(type=NOT_EXTENDABLE, src=PUBLIC) [@Retention](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/Retention.html)([RUNTIME](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/RetentionPolicy.html#RUNTIME)) [@Target](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/Target.html)([TYPE](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/ElementType.html#TYPE)) public @interface WebappCompatible
Annotation that should be placed on AuthorOperations to indicate whether they are suitable to be invoked from the WebApp. An action that has in its configuration an operation that is not webapp compatible will not be available in webapp. If the annotation is not present, we assume that the operation is not webapp compatible. One reason for an operation not to be webapp-compatible is that it shows a Swing dialog.

## Optional Element Summary
 Optional Elements
Modifier and Type

Optional Element

Description
 boolean [value](#value())
Whether the author operation is WebApp compatible.

## Element Details

### value

boolean value

Whether the author operation is WebApp compatible.
  Returns: true if the author operation is WebApp compatible.   Default: true
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
