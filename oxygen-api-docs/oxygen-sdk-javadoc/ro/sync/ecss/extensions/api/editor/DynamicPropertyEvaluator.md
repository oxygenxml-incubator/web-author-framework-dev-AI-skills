Package [ro.sync.ecss.extensions.api.editor](package-summary.md)

# Interface DynamicPropertyEvaluator
    @API(type=NOT_EXTENDABLE, src=PUBLIC) public interface DynamicPropertyEvaluator
Some form control properties can't be evaluated at the time the CSS is compiled. For example the [InplaceEditorCSSConstants.PROPERTY_WIDTH](InplaceEditorCSSConstants.md#PROPERTY_WIDTH) can depend on the font size used by the form control (10em). This means that the value of the property can be evaluated only after the form control initializes itself. This evaluator offers methods that can expand such dynamic properties.
  Since: 16.1
## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 int [evaluateHeightProperty](#evaluateHeightProperty(java.util.Map,int))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> arguments, int fontSize)
Evaluates [InplaceEditorCSSConstants.PROPERTY_HEIGHT](InplaceEditorCSSConstants.md#PROPERTY_HEIGHT) to a value.
  int [evaluateWidthProperty](#evaluateWidthProperty(java.util.Map,int))([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> arguments, int fontSize)
Evaluates [InplaceEditorCSSConstants.PROPERTY_WIDTH](InplaceEditorCSSConstants.md#PROPERTY_WIDTH) to a value.

## Method Details

### evaluateWidthProperty

int evaluateWidthProperty([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> arguments, int fontSize)

Evaluates [InplaceEditorCSSConstants.PROPERTY_WIDTH](InplaceEditorCSSConstants.md#PROPERTY_WIDTH) to a value. The value of this property might depend on the font size so the form control must explicitly call this method with the font it uses.
```

 elem {
   content: oxy_textfield(edit, '#text', width, 12em)
 }

```

  Parameters: arguments - Form control arguments. Used to get the value of [InplaceEditorCSSConstants.PROPERTY_WIDTH](InplaceEditorCSSConstants.md#PROPERTY_WIDTH). fontSize - The font size to be used for values that depend on the font, like 20em. Returns: The expanded value or -1 if the property is not set or its value is invalid.
### evaluateHeightProperty

int evaluateHeightProperty([Map](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Map.html)<[String](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/String.html),[Object](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html)> arguments, int fontSize)

Evaluates [InplaceEditorCSSConstants.PROPERTY_HEIGHT](InplaceEditorCSSConstants.md#PROPERTY_HEIGHT) to a value. The value of this property might depend on the font size so the form control must explicitly call this method with the font it uses.
```

 elem {
   content: oxy_video(href, attr(toPlay), width, 12em, height, 12em)
 }

```

  Parameters: arguments - Form control arguments. Used to get the value of [InplaceEditorCSSConstants.PROPERTY_HEIGHT](InplaceEditorCSSConstants.md#PROPERTY_HEIGHT). fontSize - The font size to be used for values that depend on the font, like 20em. Returns: The expanded value or -1 if the property is not set or its value is invalid.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
