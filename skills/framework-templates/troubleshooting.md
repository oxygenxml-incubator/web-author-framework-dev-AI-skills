# Troubleshooting & Verification

How to verify a templates extension loaded correctly, and what to check when it didn't. Every failure mode below is a real, observed Web Author behavior — not theoretical.

## Verifying after restart

**Browser (Chrome DevTools MCP)** — see `chrome-mcp-usage.md` in the `ai-framework-developer` skill. Open the New File wizard and confirm:

1. The category path appears under the expected root (e.g. `DITA → Workout`).
2. Each template label matches the configured `displayName` (or filename if `displayName` is omitted).
3. Selecting a template produces seed content with `${id}` replaced, the cursor at `${caret}`, and `<?oxy-placeholder?>` PIs rendered as hints.

**Without the MCP** — tell the user the MCP isn't installed and that, for a better experience, they can install it from <https://github.com/ChromeDevTools/chrome-devtools-mcp>. Otherwise, post the WA URL plus the three checks and ask for manual confirmation.

**Quick check without driving the wizard** — open `http://localhost:<PORT>/oxygen-xml-web-author/app/template-chooser.html`. It renders the merged tree the dashboard's New File flow uses, including all categories from user-uploaded frameworks. Grep `document.body.innerText` for your category / template names. Prefer this over the REST endpoint — the chooser works with the existing browser session, while `/rest/<ver>/actions/templates` is auth-gated and CSRF-filtered.

## If a template doesn't appear

Diagnose top-down.

### 1. `addEntry path` points at the parent `templates/` dir

Load succeeds silently; nothing shows up. **Fix**: `path="…/templates/<Category Folder>"`. One `<addEntry>` per category.

### 2. Multiple `.exf` extensions of the same base framework

Two extensions both `base="DITA"`, both `priority=High` — WA binds the doctype to one extension's identity and silently drops contributions from the other. Symptom: A's templates appear, B's don't, no error in the log.

- **Fix**: consolidate into a single `.exf` (one `<author>` block, one `<documentTemplates>` block, etc.). Don't run parallel extensions of the same base.
- Also recorded in user memory `feedback_one_exf_per_base_framework.md`. If you see two `.exf` files with the same base, fold one into the other before anything else.

### 3. `${framework}` (URL form) breaks the templates loader on Windows

`${framework}` resolves to a `file:/D:/...` URL. The templates loader passes that to `File.exists()` without stripping `file:`; the SecurityManager then denies a path literally starting with `"file:\D:\..."`. Symptom in `OXYGEN_LOG`:

```
WARN ro.sync.template.d - Templates directory cannot be accessed:
  file:/D:/.../templates/<Category>
java.security.AccessControlException: access denied ("java.io.FilePermission"
  "file:\D:\...\templates\<Category>" "read")
```

- **Fix**: use `${frameworkDir}` instead — same directory, plain file-path form, no `file:` prefix.
- The same bug doesn't bite `<addCss>` because the CSS loader strips the `file:` prefix correctly.

Reference: <https://www.oxygenxml.com/doc/ug-editor/topics/editor-variables.html>.

### 4. `category.properties` in the wrong place

Must live in the same folder as the `.dita` / `<Name>.properties` pair.

### 5. `categoryPath=` malformed

No leading slash. Forward slashes only. No backslashes.

### 6. `.exf`'s `base=` case-mismatch

`DITA`, not `dita`. Mismatches fail at framework-load time, not at XML validation — the `.exf` itself looks fine.

### 7. Wrong `type=` in `<Name>.properties`

For DITA, `type=dita` is required for the template to appear in DITA Maps Manager flows. Anything else and it silently disappears from those entry points.

### 8. Log silence ≠ success

`OXYGEN_LOG` shows:

- `Loading user uploaded frameworks from:` — kit found the extension.
- `Templates directory cannot be accessed: …` — the Windows `${framework}` bug.
- Validation messages mentioning your `.exf` — `.exf` rejected outright.

But cases (1) "wrong path" and (2) "parallel extensions" produce *nothing* in the log. Don't assume silent log = working extension; verify in the browser or via the chooser HTML. Use `web-author-logs.md` in the `ai-framework-developer` skill to grep `oxygen.log`.

## If the wizard shows the template but creating a file fails

- Seed `.dita` is malformed — open it directly in WA first; fix XML errors before re-testing the wizard path.
- Placeholder typos like `$ {id}` or `${Id}` won't be expanded — they appear literally in the saved file.
- `<?oxy-placeholder?>` PI in an element that contains other content or whitespace — the PI won't render. Strip whitespace inside the element.

## When stuck

After two failed iterations or one silently-dropped construct: stop guessing and switch to `oxygen-docs`. Start from the topics in `doc-references.md`. Templates failures are a known soft-fail area in Web Author and the docs name behaviors that aren't visible from the local kit alone.
