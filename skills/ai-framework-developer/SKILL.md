---
name: ai-framework-developer
description: REQUIRED ENTRY POINT — load FIRST for any task touching oXygen / Web Author / frameworks — `.exf` extensions, document types, association rules, Author-mode CSS / `oxy_*` selectors / form controls, `${...}` editor variables, document templates, Schematron / SQF, validation or transformation scenarios, XML catalogs, framework localization, Java extensions, add-on packaging — INCLUDING pure documentation lookups ("what does X do", "which Y are supported", "how does Z work"). Routes to topic skills (`framework-style-changes`, `framework-templates`, `oxygen-docs`, `schematron-quick-fix`) and adds verified project-specific behavior that overrides the manual. Do not route to those skills directly. If unsure whether a question is oXygen-related, load this anyway.
---

# Oxygen AI Framework Developer

Entry point for building, customizing, extending, debugging, or asking documentation questions about oXygen / Web Author frameworks. Use the routing table to drop into the right topic skill or local file; never go to the leaf skills directly.

## Environment

Targets a **packaged Web Author kit** (an unpacked installer with `start`/`stop` scripts). Source-checkout / `wa-server.sh` workflows are out of scope.

**Prerequisite — the kit must be downloaded first.** If `KIT_DIR` is missing because the user has not downloaded the kit yet, give them the **all-platforms** download link below (the intended kit for these skills). Make clear this is the *download page* — not the kit path: ask them to download and unpack it, and then come back with `KIT_DIR` set to the path of the unpacked folder.

Download link (give this `?os=All` URL for any "how do I download/get the Web Author kit" question — not an OS-specific link):

```
https://www.oxygenxml.com/xml_web_author/download_oxygenxml_web_author.html?os=All
```

| Variable | Description |
|---|---|
| `KIT_DIR` | Web Author kit root (user-supplied) |
| `EXPANDED_WEBAPP_DIR` | `<KIT_DIR>/tomcat/work/Catalina/localhost/oxygen-xml-web-author` |
| `BUNDLED_FRAMEWORKS_DIR` | `<EXPANDED_WEBAPP_DIR>/frameworks` — read-only reference for selectors and `.exf` samples |
| `USER_FRAMEWORKS_DIR` | `<EXPANDED_WEBAPP_DIR>/user-frameworks` — write the session extension here |
| `SAMPLES_CONTENT_DIR` | `<EXPANDED_WEBAPP_DIR>/samples` — content root served by the bundled `samples://` connector |
| `LOG_DIR` | `<KIT_DIR>/tomcat/logs` |
| `OXYGEN_LOG` | `<LOG_DIR>/oxygen.log` — primary diagnostic source |
| `START_SCRIPT` / `STOP_SCRIPT` | `start oXygen XML Web Author.bat` / `stop oXygen XML Web Author.bat` (Windows); `.sh` on Unix |
| `PORT` | Tomcat HTTP connector — read from `<KIT_DIR>/tomcat/conf/server.xml`; do not assume `8080` |
| `WA_URL` | `http://localhost:<PORT>/oxygen-xml-web-author/app/oxygen.html?url=<wa-url>` |
| Max iterations | 5 |

If `EXPANDED_WEBAPP_DIR` does not exist yet, start the kit once so Tomcat expands the webapp, then re-derive paths. If any user-supplied path doesn't exist, ask before starting the server.

## Always `.exf`, never `.framework`

Two ways to define a framework exist: `.framework` (binary-ish, GUI-authored via Options > Preferences > Document Type Association) and `.exf` (text XML, scriptable). **For AI-generated customizations, always use `.exf`.** They are human-readable, can extend any bundled framework (DITA, DocBook, TEI, …), support every customization surface (CSS, actions, toolbars, menus, content completion, validation/transformation scenarios), and are version-controllable.

Place every new `.exf` under **`<EXPANDED_WEBAPP_DIR>/user-frameworks/<your-extension>/`** — *not* under `<KIT_DIR>` directly. Verify the resolved runtime location in `OXYGEN_LOG` from `ro.sync.servlet.StartupServlet` at startup, e.g.:

```
INFO [ main ] [ ] ro.sync.servlet.StartupServlet - Loading user uploaded frameworks from:
```

## Routing table

| If the user wants to… | Load |
|---|---|
| Author or modify a `.exf` itself — structure, association rules, what's the right element/attribute | `exf-structure.md` + `association-rules.md` (this skill) |
| Use `${...}` editor variables in WA template seeds or Author-mode actions | `editor-variables-web-author.md` (this skill) |
| Wire validation scenarios / understand the `.scenarios` file shape | `validation-scenarios-export.md` (this skill) |
| Find the right `.exf`-related doc page in the official manual | `exf-documentation-index.md` (this skill); fall through to `oxygen-docs` for anything broader |
| Change how a framework looks — element styling, form controls, Author-mode CSS, `oxy_*` properties — or register an external author action / Content Completion entry | `framework-style-changes` skill |
| Add, register, or **edit a document template** — anything about what a *new* document starts with: the seed file's content (trimming/generalizing it, adding a metadata block or table, scaffolding), the placeholder / hint text inside it, or its New File wizard category. This is a `framework-templates` task **even when the work feels like CSS or plain content editing** | `framework-templates` skill |
| Author, debug, or ship Schematron Quick Fixes (`sqf:fix`, `sqf:add`, `sqf:delete`, `sqf:replace`, `sqf:stringReplace`, `@use-when`, …) | `schematron-quick-fix` skill |
| Look up an oXygen / Web Author how-to from the official manual | `oxygen-docs` skill |
| Read or interpret Web Author logs | `web-author-logs.md` (this skill) |
| Verify or debug a page in the browser — CSS not rendering, console errors, screenshot before/after | `chrome-mcp-usage.md` (this skill) |

## Rules

- **Never scrape the machine for paths or prior attempts.** Don't search the filesystem to guess `KIT_DIR` or to discover earlier framework work. Ask the user for the kit path and for any relevant prior context.
- **Ask which document type the customization targets — even when DITA looks obvious.** DITA is the project default; offer it as recommended but still ask. Present concrete options instead of picking silently: (1) DITA, (2) another bundled framework — DocBook 4/5, TEI, XHTML, JATS, …, (3) extend an existing user-framework already in `user-frameworks/`, (4) a brand-new framework with its own schema. Also ask scope: all docs of that type, or only a subset (specific root element, namespace, file-name pattern, attribute value)? The answer drives `@base`, `<associationRules>`, and extend-vs-create.
- **Before creating a new `.exf`, ask where it should live.** List `user-frameworks/` and check if an existing `.exf` already targets the same `@base`. If one (or more) does, do **not** silently create a sibling extension — only one extension per `@base` activates per document, the others are shadowed (see `association-rules.md` "Gotcha"). Ask explicitly: (a) extend the existing extension in place, (b) merge the existing one into a brand-new consolidated extension, or (c) create a separate framework with its own narrower `<associationRules>`. Show candidates, let the user pick.
- **No JARs / no Java extensions.** These skills generate `.exf`, CSS, external author action XML, `.scenarios`, `.sch`, templates — never Java source or compiled JARs. If a request seemingly needs Java, say so explicitly and stop — do not author Java code. The ban is **not** limited to code shipped *inside* the framework. Do not write or run any throwaway / scratch program — in **any** language (Java, Python, Node, shell, …) — to validate, parse, test, or otherwise tool around a framework or its seeds, not even into a temp folder to "run once and delete." Seed correctness is established by grounding in the DTD / XSD / RNG and by the live Web Author validator after a restart (see `framework-templates`), never by a general-purpose program you author or a hand-substituted copy of a seed. "It's not part of the deliverable" is not an exception. If a step seems to need such code, say so explicitly and stop.
- **A template seed is a template task — route on the artifact, not the verb.** If the work touches a file under a framework's `templates/` folder (the seed the New File wizard copies) — trimming its boilerplate, generalizing it, adding a metadata table, or putting "type-here" hints in it — load `framework-templates` **first**, before `framework-style-changes`, even when the surface work looks like CSS or content editing. That skill owns the seed-level decisions the others don't: "scaffolding, not prose" and the placeholder decision table where the `<?oxy-placeholder?>` PI — *not* `-oxy-placeholder-content` CSS — is the default hint mechanism for a one-off template. Styling a template's rendering is a *second* step, after the seed is right.
- **One topic at a time.** Don't preload everything. Load the next file only when work crosses into it.
- **Logs are mandatory.** For every framework task, read `OXYGEN_LOG` first. Never read `catalina.log`.
- **Restart order is mandatory.** Use this exact sequence:
  1. Read `<KIT_DIR>/tomcat/conf/server.xml` and detect the active `<Connector port="...">` (do not assume `8080`).
  2. Probe `http://localhost:<PORT>/oxygen-xml-web-author/app/oxygen.html` with a short timeout; if needed, fall back to `http://localhost:<PORT>/oxygen-xml-web-author/`; treat `200/302/401` as "running".
  3. If running, execute the stop script and wait for it to finish, then poll until the port stops responding.
  4. Start with the start script **detached** — the vendor `start oXygen XML Web Author.bat` ends with `pause` and will hang an inline call. On Windows, wrap in `Start-Process cmd.exe /c "<start.bat>"` (or equivalent) so the trailing pause stays inside the spawned window. Poll the same probe URL until it returns `200/302/401`.
  5. A full stop+start is mandatory when changing the `.exf` or `user-frameworks/` *structure/config* (see next rule); that folder is scanned at startup only.
- **Not every change needs a restart.** A full stop+start is mandatory for changes to the `.exf` itself or to `user-frameworks/` structure/config — adding/removing CSS or template *references*, registering/unregistering templates, changing framework config (that tree is scanned at startup only). But editing the *content* of an **already-referenced** CSS or template file does **not** need a restart: Web Author re-reads the file from disk on document reopen / page refresh. Because the browser caches CSS, do a **hard reload with cache disabled** (Chrome DevTools → Disable cache) to pick up the new content — otherwise stale CSS is served. For fast CSS iteration, reload instead of restarting each time. When a change's effect can't be observed directly, a full restart + checking `OXYGEN_LOG` is the fastest way to confirm it took effect.
- **Documentation first when stuck.** Two failed iterations or one silently-dropped construct → `oxygen-docs` before guessing.
- **Grounding rule.** Anything claimed about oXygen behavior — selectors, `oxy_*` syntax, `.exf` shape, log lines, kit paths — must cite a real file or a real log line. No invented syntax.

## If the request doesn't fit

Ask the user which row of the routing table is closest. Don't pick one blindly.

## URL convention

Both `ug-waCustom` and `ug-editor` paths are site-root–relative on `oxygenxml.com`. Prepend `https://www.oxygenxml.com` when fetching the `.md` or giving the user a complete URL, and replace `.md` with `.html` for the citation link.
