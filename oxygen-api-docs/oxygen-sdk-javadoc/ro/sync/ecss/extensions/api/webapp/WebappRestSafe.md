Package [ro.sync.ecss.extensions.api.webapp](package-summary.md)

# Annotation Interface WebappRestSafe
    @API(type=NOT_EXTENDABLE, src=PUBLIC) [@Retention](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/Retention.html)([RUNTIME](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/RetentionPolicy.html#RUNTIME)) [@Target](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/Target.html)([TYPE](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/annotation/ElementType.html#TYPE)) public @interface WebappRestSafe
Annotation that should be placed on AuthorOperations to indicate that they are safe to be invoked in Web Author via a REST API with user supplied arguments. An operation that simply inserts an XML fragment would be considered safe, while one that executes some JavaScript code provided by the user would be considered unsafe. If the operation has parameters with type [ArgumentDescriptor.TYPE_XPATH_EXPRESSION](../ArgumentDescriptor.md#TYPE_XPATH_EXPRESSION), these parameters are checked to be safe to execute before the operation is invoked.
  Since: 19.1
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
