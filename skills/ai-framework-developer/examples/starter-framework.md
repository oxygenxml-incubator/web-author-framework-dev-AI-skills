# Starter framework example

Self-contained scaffold for a brand-new (standalone) framework: folder layout, a `.exf` covering the most common pieces, `catalog.xml`, and a development-scaffold CSS that makes every element visible during early authoring.

Use this only when scaffolding a framework from scratch. For an extension over a bundled framework (DITA, DocBook, …), the smaller "Minimal extension example" in [exf-structure.md](../exf-structure.md) is enough.

## Folder layout

Place under `<KIT_DIR>/tomcat/work/Catalina/localhost/oxygen-xml-web-author/user-frameworks/MyFramework/` — the Web Author user-frameworks dir lives **inside the expanded webapp work directory**, not at the kit root:

```
MyFramework/
  my-framework.exf
  catalog.xml
  schemas/
    <schema-file>.xsd        # or .rng / .dtd / ...
  templates/
    <template>.xml
  css/
    main.css
  resources/                 # optional, classpath entries (Java extensions, etc.)
```

## `.exf`

Covers the common pieces — templates, classpath, catalog, CSS:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<script xmlns="http://www.oxygenxml.com/ns/framework/extend"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://www.oxygenxml.com/ns/framework/extend
    http://www.oxygenxml.com/ns/framework/extend/frameworkExtensionScript.xsd">
  <name>My Framework</name>
  <description/>
  <priority>High</priority>

  <associationRules>
    <!-- Replace the wildcards with the real root element / namespace
         once known. Leaving "*" matches any XML doc and is only useful
         while developing. -->
    <addRule namespace="*" rootElementLocalName="*" fileName="*" publicID="*"
             javaRuleClass="" attributeLocalName="*" attributeNamespace="*"
             attributeValue="*"/>
  </associationRules>

  <documentTemplates>
    <addEntry path="${frameworkDir}/templates"/>
  </documentTemplates>

  <classpath>
    <addEntry path="${framework}/resources"/>
  </classpath>

  <xmlCatalogs>
    <addEntry path="${framework}/catalog.xml"/>
  </xmlCatalogs>

  <author>
    <css>
      <addCss path="${framework}/css/main.css"/>
    </css>
  </author>
</script>
```

## `catalog.xml`

Maps schema URIs declared in documents to the actual files shipped in the framework:

```xml
<catalog xmlns="urn:oasis:names:tc:entity:xmlns:xml:catalog">
  <uriSuffix uriSuffix="<schema-file-name>.xsd" uri="./schemas/<schema-file-name>.xsd"/>
</catalog>
```

## Dev-scaffold `css/main.css`

Makes every element visible — useful as a starting point before real styling lands. Strip once real styling exists.

```css
* {
  display: block;
}

/* Show element name before each element. */
*:before(1001) {
  content: oxy_name() " ";
  font-size: 0.75rem;
  font-family: monospace;
  background-color: lightgray;
}
```

## Next steps

1. Drop the folder under `user-frameworks/`.
2. Restart Web Author per the `ai-framework-developer` rules (full stop+start; `user-frameworks/` is scanned at startup only).
3. Tail `tomcat/logs/oxygen.log` for `Loading user uploaded frameworks from:` to confirm the extension loaded.

Reference: <https://www.oxygenxml.com/doc/versions/28.1.0/ug-waCustom/topics/wa-create-framework-from-scratch.html>
