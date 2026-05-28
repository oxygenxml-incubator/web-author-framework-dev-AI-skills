# Editor Variables in Web Author

**Web Author only.** Behavior of `${...}` editor variables across the two contexts they appear in framework work:

1. **Document-template seeds** instantiated through the Web Author **New File** wizard (expansion at New-File time).
2. **Author-mode actions and operations** — `.exf` author actions, code templates, operation arguments — where `${ask(...)}` prompts the user at invocation time.

**Do NOT apply these rules to desktop oXygen Editor / Author** — desktop has different (broader) variable support and different context rules, and is not in scope here.

Source: [`/doc/ug-waCustom/topics/webapp_editor_variables.html`](https://www.oxygenxml.com/doc/ug-waCustom/topics/webapp_editor_variables.md). The official page lists which variables Web Author *processes* but does **not** distinguish the contexts in which each is processed (template seed vs. code template vs. Author-mode operation vs. transformation scenario). The tables below add that.

## Variables that expand correctly in template seeds

| Variable | Spec | Notes |
|---|---|---|
| `${id}` | "10-12 letters and digits, app-level unique" | **Regenerates per occurrence** — three uses in one seed yield three different ids. Fine for `id="topic_${id}"`; surprising if you expected a per-document constant. |
| `${uuid}` | "32 hex digits" | Per-occurrence regen, same caveat as `${id}`. |
| `${timeStamp}` | "Unix-format timestamp" | Long string (`yyyyMMddHHmmssSSS`-ish). |
| `${date(pattern)}` | Java SimpleDateFormat | Patterns *without commas* work (`yyyy-MM-dd`, `yyyy-MM-dd'T'HH:mm:ssXXX`, `yyyy`, `MM`, `dd`). Patterns with literal commas break — and you cannot escape them with `${comma}` (date() parses commas as arg separators). |
| `${cfd}`, `${cfdu}` | Parent folder, file path / URL | Work. |
| `${cfn}`, `${cfne}` | File name without / with extension | Include the `filenamePrefix` from the `.properties`, not just the user-typed stem. |
| `${currentFileURL}` | Current file as URL | Resolves to the connector URL (`webdav-http://...`, etc.). |
| `${frameworks}`, `${frameworksDir}` | Frameworks-parent dir, URL / file path | Work. |
| `${home}`, `${homeDir}` | Home dir, URL / file path | Resolve to the **webapp** home (`.../tomcat/work/Catalina/localhost/oxygen-xml-web-author/`), NOT the OS user home. |
| `${env(VAR)}` | OS env variable | Reads the Tomcat JVM's environment. |
| `${system(prop)}` | Java system property | E.g. `${system(user.language)}` → `en`, `${system(os.name)}` → `Windows 11`. |
| `${ps}` | Platform path separator | `;` on Windows, `:` on Unix. |
| `${xpath_eval(expr)}` | Static or dynamic XPath | Works, including with **nested `${...}`** in the expression. Verified: `${xpath_eval(upper-case('hello'))}` → `HELLO`; `${xpath_eval(string-length('${cfn}'))}` → length of the resolved file name. Dynamic XPath against the new document context (`@id`, etc.) is plausible by analogy but not separately verified here. |
| `${makeRelative(base, location)}` | Relativize `location` against `base` | Both args are URLs. Accepts **nested `${...}`** — typically `${makeRelative(${currentFileURL}, <target-url>)}`. **Only relativizes when `base` and `location` share scheme + host.**. |

## Variables that stay literal in template seeds

These do **not** work in WA template seeds — they remain literal, do nothing, or break instantiation:

- `${ask(...)}` — listed as supported in the WA editor-variables docs, but in **template seeds** no dialog is shown at New File time and the variable is not expanded. It **does** work in Author-mode actions / operations (next section).
- `${user.name}`, `${author.name}` — not supported in Web Author.
- `${cf}`, `${ds}`, `${dsu}`
- `${framework}`, `${frameworkDir}` — only the **plural** forms (`${frameworks}`, `${frameworksDir}`) work in seed content. Singular forms stay literal.
- `${xmlCatalogFilesList}`
- `${comma}`, `${caret}`, `${selection}`
- `${configured.ditaot.dir}`, `${dita.dir.url}`
- `${framework(name)}`, `${frameworkDir(name)}`, `${pluginDir(id)}`, `${pluginDirURL(id)}`, `${i18n(key)}`

## Practical guidance for template seeds

1. Stick to the green-table variables above. They are the only ones that reliably expand in this context.
2. Use `${currentFileURL}`, not `${cf}`, for absolute paths.
3. Don't rely on `${ask(...)}` to prompt the author at New-File time — no dialog shows. Bake sensible defaults into the seed and let the author edit, or move the prompt to an Author-mode action triggered after the file opens (next section).

## `${ask(...)}` in Author actions

Outside template seeds, `${ask(...)}` is the standard way to prompt the user at action-invocation time. Use it inside operation arguments in `.exf` author actions, code templates, and Author-mode operations. **Web Author supports a subset of the desktop types.**

Full form:

```
${ask('message', type, ('real1':'rendered1';'real2':'rendered2'; ...), 'default', @id)}
```

| Position | Parameter | Notes |
|---|---|---|
| 1 | `'message'` | Required. Quoted. Used as dialog title for `generic`; prefixed with the type name for the others. |
| 2 | `type` | Optional, defaults to `generic`. See table below. |
| 3 | choices `('real':'rendered'; …)` | Only for `combobox`, `editable_combobox`, `radio`. |
| 4 | `'default'` | Optional. For combobox/radio, can match either a key or a rendered value. |
| 5 | `@id` | Optional. Correlates with `${answer(@id)}` (desktop) — Web Author support not separately verified. |

**Types supported in Web Author** (per `webapp_editor_variables.md`):

| Type | Use |
|---|---|
| `generic` | Plain text input. Default if `type` omitted. |
| `url` | URL input; WA validates the URL. |
| `relative_url` | URL relativized against the current document; falls back to absolute for untitled docs. |
| `password` | Input hidden with bullets. |
| `combobox` | Drop-down; returns `real` for the chosen `rendered`. |
| `editable_combobox` | Drop-down + free text. `rendered` values are ignored in WA — only the key is shown. |
| `radio` | Radio-button group; returns `real` for the chosen `rendered`. |

**Types in desktop but NOT in Web Author** (omit when targeting WA):

- `textarea` — listed in `editor-variables.md` (desktop), not in the WA page. Don't rely on it in WA actions.

**Companion variable `${answer(@id)}` — NOT supported in Web Author.**


Workarounds when the captured value must appear in two places (e.g. an `<xref>` `href` and its text content):

1. Leave the second location empty and let CSS or default rendering fill it (e.g. an `<xref href="..."/>` with no text content — DITA renders the href).
2. Accept two `${ask(...)}` prompts (no `@id` needed); the user types the value twice.
3. Implement a custom Java/JS operation that holds the answer in process and stamps it into multiple positions.

**Nesting `${...}` inside `${ask(...)}`** works (the inner variable is expanded first):

```
${ask('Provide a date', generic, '${date(yyyy-MM-dd)}')}
```

For the full desktop syntax, `@id` + `${answer(...)}`, and `textarea`, see [`/doc/ug-editor/topics/editor-variables.html`](https://www.oxygenxml.com/doc/ug-editor/topics/editor-variables.md).
