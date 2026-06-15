# Private Templates

This folder is for **private, local-only, or client-sensitive** Elementor templates.

## Important

- Files in this folder are **completely ignored by Git** and will never be committed
- Do **not** move private templates into public reference folders without explicit owner approval
- Use this folder for:
  - Client-sensitive page layouts
  - Production-only Elementor exports
  - Early draft versions
  - Day-to-day working templates
  - Unreleased designs

## What Goes Here

- `*.json` files that contain proprietary or confidential layouts
- Production-only Elementor exports
- Draft templates not yet approved for inclusion in the main rebuild
- Any Elementor work that should remain completely private

## What Does NOT Go Here

- Public learning materials (use `../elementor-templates/`)
- Approved reference exports (use `../references/exports/`)
- Section maps and documentation (use `../section-maps/`)

## Publishing Private Templates

If the owner decides to publish a private template:

1. Review the template for any sensitive data
2. Get explicit owner approval
3. Move the file to `../references/exports/`
4. Update documentation if needed
5. Stage and commit with other public files

Never commit files from this folder.

See [AGENTS.md](../../AGENTS.md) for complete commit rules.
