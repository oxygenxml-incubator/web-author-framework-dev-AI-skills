Package [ro.sync.ecss.extensions.api](package-summary.md)

# Interface StylesFilter
    All Superinterfaces: [Extension](Extension.md)   All Known Implementing Classes: [GeneralStylesFilterExtension](../../../exml/plugin/author/css/filter/GeneralStylesFilterExtension.md)   @API(type=EXTENDABLE, src=PUBLIC) public interface StylesFilterextends [Extension](Extension.md)
Filter for the element styles. Use this to replace the CSS styles associated to an element or a pseudo element.

oXygen supports multiple :before and :after pseudo elements. For example, the selector :before(2) represents a pseudo-element before a 'regular' :before, both of which are contained at the start of an element. The :before and :before(1) are equivalent.

The following rules:

```

  p { content: 'A' }
  p:before(1) { content: 'B'; }
  p:before(2) { content: 'C'; }

```

Result in :

```

  ,-----------------------.
  | ,---. ,---.           |
  | | C | | B | A         |
  | `---' `---'           |
  `-----------------------'

```

So, an implementation of [StylesFilter](StylesFilter.md) receives callbacks for:

1. for each element from the document object model
2. for each :before and :after pseudo-element, no matter if they were defined in the CSS or not for the parent element.
3. for each :before(n) and :after(n), with n >= 2, pseudo-element, but only if they have been defined in the the CSS for the parent element.

 The level of the pseudo-element can be determined by using [Styles.getPseudoLevel()](../../css/Styles.md#getPseudoLevel()).

**Important:**  To use higher level pseudo elements (':before(n)', ':after(n)' with n >= 2) make sure you specify them in your CSS, having a content property. The content property specified for them can be later replaced by the [StylesFilter](StylesFilter.md).

 oXygen collects all the pseudo element levels from the CSS use these to probe the [StylesFilter](StylesFilter.md).

For example, having the following CSS:

```


    body            { color:blue;}     
    div:before(300) { content: 'D300'}
    p:before(100)   { content: 'P100'}
    p:before        { content: 'P1'}

    a:before(5)     { content: 'A5'}

```

And the XML document:

```

    <body>
      <div>
        <p>
          <a></a>
        </p>
      </div>
    </body>

```

Your implementation will get callbacks like:

```


    filter(body, styles); 
    filter(before(body), styles);    // styles.pseudoLevel = 1;    // Always
    filter(after(body),  styles);    // styles.pseudoLevel = 1;    // Always

    filter(div, styles);                                           // Always
    filter(before(div),  styles);    // styles.pseudoLevel = 1;    // Always
    filter(before(div),  styles);    // styles.pseudoLevel = 300;  // Only if there is a div:before(300) with content in the CSSS.  
    filter(after(div, 1),styles);    // styles.pseudoLevel = 1;    // Always

    filter(p, styles);                                             // Always
    filter(before(p),    styles);    // styles.pseudoLevel = 1;    // Always
    filter(before(p),    styles);    // styles.pseudoLevel = 100;  // Only if there is a p:before(100) with content in the CSSS.
    filter(after(p),     styles);    // styles.pseudoLevel = 1;    // Always

    filter(a, styles);                                              // Always
    filter(before(a),    styles);     // styles.pseudoLevel = 1;    // Always
    filter(before(a),    styles);     // styles.pseudoLevel = 5;    // Only if there is a a:before(5) with content in the CSSS.
    filter(after(a),     styles);     // styles.pseudoLevel = 1;    // Always


```

So for each element, each possible level will be probed.

If your StylesFilter implementation also implements the [AuthorExtensionStateListener](AuthorExtensionStateListener.md) API, its "activated" callback will be automatically called with the corresponding [AuthorAccess](AuthorAccess.md).
  See Also:
* [ExtensionsBundle](ExtensionsBundle.md)

## Method Summary
  All MethodsInstance MethodsAbstract Methods
Modifier and Type

Method

Description
 [Styles](../../css/Styles.md) [filter](#filter(ro.sync.ecss.css.Styles,ro.sync.ecss.extensions.api.node.AuthorNode))([Styles](../../css/Styles.md) styles, [AuthorNode](node/AuthorNode.md) authorNode)
Filter the styles for the specified element.

### Methods inherited from interface ro.sync.ecss.extensions.api.[Extension](Extension.md)
 [getDescription](Extension.md#getDescription())
## Method Details

### filter

[Styles](../../css/Styles.md) filter([Styles](../../css/Styles.md) styles, [AuthorNode](node/AuthorNode.md) authorNode)

Filter the styles for the specified element. A common use-case is to change only some of the CSS properties from the original styles and keep the others. To this end, one should use [Styles.setProperty(int, Object)](../../css/Styles.md#setProperty(int,java.lang.Object)) on the original styles and return them.
  Parameters: styles - The original CSS styles associated with the specified authorNode. This object should only be used for the lifetime of the method. It shouldn't be kept in a cache. authorNode - The node to filter the CSS style for. If this node points to a processing instruction, a CDATA or a comment then the real node can be obtained by casting this object to [ArtificialNode](node/ArtificialNode.md) and using [ArtificialNode.getWrappedNode()](node/ArtificialNode.md#getWrappedNode()). The node can be part of the document object model, or a pseudo element (A :before or an :after). To obtain the pseudo level (distance of the pseudo element from its parent), use [Styles.getPseudoLevel()](../../css/Styles.md#getPseudoLevel()). Returns: The customized CSS style that will be associated with the given node. If the returned object is null then the original styles will be used.
© Copyright [Syncro Soft SRL](http://www.sync.ro) 2002 - 2026. All rights reserved.
