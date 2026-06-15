# Elementor Outputs

This folder is the **local Elementor output workspace** for the 1st Providence rebuild.

## Folders

- **`elementor-templates/`** — Local output location for generated Elementor page and section templates (ignored by Git)
- **`private-templates/`** — Local folder for private or client-sensitive templates (always ignored by Git)
- **`references/`** — Approved public reference materials (committed to public repository with owner approval)
- **`section-maps/`** — Markdown documentation of page section structures (committed to public repository)

## Rules

1. **Generated Elementor templates** go in `elementor-templates/` and are ignored by Git by default.
2. **Private templates** go in `private-templates/` and are completely ignored by Git.
3. **Public reference exports** go in `references/exports/` only when explicitly approved for public use.
4. **Section maps** (Markdown files) go in `section-maps/` and are always committed.
5. Every Elementor build task that requires a page, section, or component must produce a real `.json` Elementor template.
6. Markdown-only output is insufficient when a task asks for a template or export.

See [REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md](../docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md) for detailed guidance on the output workflow.

See [AGENTS.md](../AGENTS.md) for rules on what to commit and what to keep private.
