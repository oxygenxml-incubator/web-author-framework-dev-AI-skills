# Web Author Logs

Server-side diagnosis via `oxygen.log`.

## Locations

- `KIT_DIR` — unpacked Web Author kit root.
- `<KIT_DIR>/tomcat/logs/oxygen.log` — the only file worth reading for framework / `oxy_*` / template / validation failures. All `ro.sync.*` stack traces land here.
- Logger config: `logback.xml` shipped with the kit — temporarily enable targeted loggers, repro, revert.

## Skip these — they don't carry Web Author runtime failures

`tomcat/logs/catalina.*`, `localhost.*`, `host-manager.*`, `license-servlet.log`, `webapp-start.log`. Also avoid tailing the bottom of `oxygen.log` — that's usually filter-chain boilerplate.

## Reading flow

1. Jump to today's date in `oxygen.log`:
   ```bash
   awk '/^YYYY-MM-DD/{flag=1} flag' "$KIT_DIR/tomcat/logs/oxygen.log" | head -200
   ```
2. Narrow by `ro.sync.*` package likely involved: `ro.sync.template`, `ro.sync.util.editorvars`, `ExtensionsManager`, `SandboxSecurityManager`.
3. Search for `ERROR`, `WARN`, `Exception`, `Caused by`.
4. Confirm framework scan entries for your `user-frameworks/` extension appear after a full kit restart (see `SKILL.md`).

## Common grounded gotcha: "Failed to create new file" from a template

Silent UI failure on New File from a custom template → grep `oxygen.log` for `AccessControlException` together with `FileTemplate.getContentInfo` or `RESTFileBrowser.saveNewFile`.

## URL convention

Both `ug-waCustom` and `ug-editor` paths are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching the `.md` or giving the user a complete URL, and replace `.md` with `.html` for the citation link.
