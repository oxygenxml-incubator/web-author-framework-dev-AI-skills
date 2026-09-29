Package [ro.sync.ecss.extensions.api.webapp.imagemap](package-summary.md)

# Interface WebappAreaView
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface WebappAreaView
Interface that represents an area on an image map to be rendered in the browser. Instances must be created using the factory methods in [WebappAreaViewFactory](WebappAreaViewFactory.md).
  Since: 25.0
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) [renderToSvg](#renderToSvg())()

## Method Details

### renderToSvg

[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html) renderToSvg()
  Returns: The SVG string to be sent to the browser.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
