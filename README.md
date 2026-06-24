# gogdocs

This repository contains the `gogcli` documentation site rebuilt with [Docsalot](https://docsalot.dev/).

The content was imported from the upstream `gogcli` docs sources and reshaped into a Docsalot documentation project with:

- `layout.json` for navigation, branding, colors, and tabs
- MDX pages for the imported guides, reference material, and command documentation
- Docsalot UI components such as cards, tabs, and accordions on key landing pages

## Docsalot references

- Docsalot: <https://docsalot.dev/>
- Docsalot CLI onboarding: <https://docs.docsalot.dev/cli/index>
- Live Docsalot-hosted site for this project: <https://gogcli-docs.docsalot.dev>

## Run locally

Docsalot recommends an agent-first workflow: install the CLI, install the Docsalot skill, and then let Claude, Codex, or another coding agent drive the docs lifecycle.

From the Docsalot CLI onboarding guide:

```bash
npm install -g docsalot-cli
docsalot --version
docsalot skills install
```

Once the CLI is installed, preview this repository locally from the repo root:

```bash
docsalot docs preview --dir .
```

Because this repository itself is the docs root and contains `layout.json`, `--dir .` points the preview command at the current folder.

## Typical workflow

Use your coding agent with prompts like:

- `use docsalot cli to run a preview for this docs repo`
- `use docsalot cli to update the docs and publish the latest version`
- `use docsalot cli to reorganize navigation in layout.json`

If you want the exact manual workflows and CLI command reference, use the published Docsalot CLI docs:

<https://docs.docsalot.dev/cli/index>
