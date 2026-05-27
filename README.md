# Web Author Framework Developer AI Skills

An experimental toolkit that lets you use AI assistants (Claude Code) to help build, customize, and test Oxygen XML Web Author frameworks.

If you author or maintain Web Author frameworks these skills aim to make the work faster and less tedious. You describe what you want in plain language ("style this element in blue with a left border", "add a form control for selecting a product version", "create a Schematron Quick Fix for missing alt text"), and the agent produces the corresponding framework changes inside your kit, which you can then review and try out in the browser.

The skills come with built-in knowledge of Web Author's framework model, CSS extensions, Guided Authoring, content completion, validation scenarios, and Schematron Quick Fixes. Optionally, with Chrome DevTools MCP installed, the agent can also load Web Author in a browser and verify that the changes work as intended.

> ⚠️ Note: Please read the [Disclaimer](#disclaimer) section before using it on anything you care about.

## Prerequisites

The `ai-framework-developer` skill works with a live Web Author environment and requires the following setup.

### 1. Web Author Kit

An unpacked Web Author kit with:

- a valid license
- an administrative user configured

### 2. Claude Code

Claude Code with support for local skills enabled.

### 3. Node.js and npx

The installer is distributed as an npm package and is invoked via `npx`, which ships with Node.js. Install Node.js (LTS recommended) from [nodejs.org](https://nodejs.org/) if it is not already available on your machine.

### 4. Chrome DevTools MCP (optional)

Chrome DevTools MCP enables browser-side verification, allowing the agent to confirm that framework changes render and behave correctly inside a real Web Author instance. While optional, it provides a significantly improved validation and debugging workflow.

The recommended way to install it is as a Claude Code plugin, which includes both the MCP server and its companion skills. In Claude Code, add the marketplace registry:

```
/plugin marketplace add ChromeDevTools/chrome-devtools-mcp
```

Then install the plugin:
```
/plugin install chrome-devtools-mcp@chrome-devtools-plugins
```

Restart Claude Code afterwards and verify the installation with `/skills`.

For full installation options and troubleshooting, see the [Chrome DevTools MCP repository](https://github.com/ChromeDevTools/chrome-devtools-mcp).

## Installation

Install the skills at the **root of your unpacked Web Author kit** — the directory where `startOxygenXMLWebAuthor.sh` / `.bat` are located. This gives the agent access to logs, sample files, and the `user-frameworks/` directory without extra configuration.

### Step 1: Open a terminal at the kit root

```bash
cd /path/to/your/web-author-kit
```

### Step 2: Create a `.claude/` directory

```bash
mkdir .claude
```

This is required due to a known bug in the `skills` installer: if `.claude/` doesn't already exist, the installer silently skips creating the symlinks Claude Code needs to discover the skills. If `.claude/` already exists, you can skip this step (the command will print a harmless "already exists" error).

### Step 3: Install the skills

```bash
npx skills add oxygenxml-incubator/web-author-framework-dev-AI-skills -a claude-code -y
```

This installs all available skills, targets Claude Code, and skips confirmation prompts.

### Step 4: Restart Claude Code

Quit Claude Code completely and start it again from the kit root location so it picks up the new skills from `.claude/skills/`.

### Step 5: Verify

In Claude Code, run `/skills`

You should see the Web Author skills listed. 

## What These Skills Can Do

The skills support a wide range of Web Author framework development tasks, including:

- Styling the Author view using custom CSS
- Enabling Guided Authoring with form controls
- Debugging frameworks using Web Author logs
- Creating custom document templates with editor variables
- Contributing content completion actions
- Defining validation scenarios and Schematron Quick Fixes (SQF)
- Looking up official documentation and citing relevant references
- Verifying changes directly in the browser using Chrome DevTools MCP

These capabilities support both creating frameworks from scratch and extending existing ones.

## Typical Workflow

A typical development workflow looks like this:

1. Install the skills at the Web Author kit root
2. Start Web Author
3. Ask the agent to create or modify a framework extension
4. Review generated changes in `user-frameworks/`
5. Validate behavior in Web Author
6. Optionally use Chrome DevTools MCP for browser-side verification

This workflow supports rapid iteration while keeping framework customization transparent and reviewable.

## Important Safety Notice

⚠️ **The agent can modify your Web Author kit.**

Before accepting changes:

- Review all proposed modifications carefully
- Keep a backup of your Web Author kit
- Prefer working from a copy of the kit during experimentation or development

When installed at the kit root, the agent can read and modify files across the entire Web Author installation, including your existing `user-frameworks/`, built-in frameworks, configuration files, and other internal Web Author resources.

The skills are intended to create and modify **user extensions inside `user-frameworks/`**. However, because the agent has filesystem access to the full kit, incorrect instructions or unintended edits may still affect bundled frameworks or internal files.

These precautions help keep framework development safe and reversible.

## License

This project is licensed under the Apache License 2.0. See the [LICENSE](LICENSE) file for the full text.

## Disclaimer

### 1. Experimental Tooling — Not an Officially Supported Product

This repository provides AI skill sets, scripts, and documentation lookup tools designed to assist developers in creating extensions for Oxygen XML Web Author. It is provided as an **experimental, community-driven toolkit** and is **not** an official, commercially supported component of the Oxygen XML product suite.

### 2. "As-Is" Provision and Limitation of Liability

This software is provided "AS IS", without warranty of any kind, express or implied. The AI agent operates with read/write access to your local Web Author kit. While the skills are engineered to operate strictly within designated extension directories (`user-frameworks/`), AI models can occasionally behave unpredictably or hallucinate file paths.

- **Always review** proposed code changes, file modifications, and terminal commands before accepting them.
- **Always back up** your Web Author kit or use version control (Git) before letting the agent make modifications.
- Oxygen XML shall not be held liable for any data loss, corrupted environments, or production downtime resulting from the use of these AI scripts.

### 3. Data Privacy and Third-Party APIs

This tool orchestrates third-party Large Language Models (LLMs) and external tools (such as Chrome DevTools MCP). By using this toolkit, you acknowledge that:

- Your prompts, local code snippets, log files, and potentially browser screenshots are transmitted to third-party AI providers.
- **Do not use this tool in production environments** or with frameworks, documents, or logs containing sensitive, proprietary, or Personally Identifiable Information (PII) data without explicit authorization from your organization's InfoSec/Compliance department.

### 4. Technical Support Boundary

Issues arising directly from the use of these AI scripts, corrupted local environments, or bugs introduced by AI-generated code are **not covered** by Oxygen XML's standard Technical Support. Please do not open official enterprise support tickets for errors caused by AI automation; use GitHub Issues for community troubleshooting instead.

Copyright 2026 Syncro Soft, SRL.