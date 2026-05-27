# Chrome MCP Usage

Browser-side verification for Web Author. For MCP tool mechanics (lifecycle, `take_snapshot`, `evaluate_script`, screenshots, troubleshooting) read the upstream `chrome-devtools` skill — do not re-explain them here.

## Setup

If `chrome-devtools` MCP tools are unavailable in the current session, install the server before falling back to user-driven verification:

```bash
claude mcp add chrome-devtools -- npx -y chrome-devtools-mcp@latest
```

After running, ask the user to restart Claude Code so the new MCP loads. Only fall back to user-driven verification if the user declines installation.

## References

- Upstream `chrome-devtools` skill (loaded after the MCP is installed)
- Sample doc URL + `<PORT>` lookup — `framework-style-changes` skill (and `ai-framework-developer` for restart rules).

## Web Author verification loop

1. Navigate to the sample URL: `http://localhost:<PORT>/oxygen-xml-web-author/app/oxygen.html?url=samples%3A%2F%2Fsamples%2F<framework>%2F<file>.xml`. Wait for the editor iframe.
2. Confirm framework CSS loaded and won. Bundled rules under `frameworks/<base>/css/core/` and `actions/actions.css` use `!important`; overrides usually need `!important` too.
   - Grep the iframe's inline `<style>` for your selector:
     `document.querySelector('iframe').contentDocument.querySelector('style').textContent`
   - Then `getComputedStyle(targetEl)` to confirm the property values you set.
3. Check the validation rail (`.navigation-rail__notification.validation-notification`) and console for CSS / `oxy_*` errors.
4. Screenshot is after-the-fact evidence, not the primary signal.

Two no-progress iterations → switch to `oxygen-docs` skill for the construct.
