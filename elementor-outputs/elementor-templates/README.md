# Generated Elementor Templates

This is the **required local output folder** for all generated Elementor page, section, and component templates.

Every Elementor build task that requires a page, section, or component must produce a real `.json` Elementor template saved here. Markdown-only output is not sufficient.

## Important

- Files in this folder are **ignored by Git** by default
- Do **not** commit generated templates unless the owner explicitly approves publishing a specific file
- All `.json` files in this folder should be treated as **local output**
- To share an Elementor template publicly, the owner must move it to `../references/exports/` and approve the commit

## Naming Format

When exporting an Elementor template, use this naming format:

**Page body templates:**
```
page-name-page-body-template.json
```

**Section templates:**
```
page-name-section-name-template.json
```

**Component templates:**
```
page-name-component-name-template.json
```

## Examples

**Page body templates:**
- `homepage-body-template.json`
- `nurse-aide-page-body-template.json`
- `medication-management-page-body-template.json`
- `electrocardiogram-technician-ekg-page-body-template.json`

**Section templates:**
- `ekg-why-students-choose-section-template.json`
- `nurse-aide-schedule-section-template.json`
- `medication-management-comparison-section-template.json`

**Component templates:**
- `homepage-cta-button-template.json`
- `nurse-aide-testimonial-carousel-template.json`

**Global templates:**
- `header-mega-menu-template.json`
- `footer-contact-section-template.json`

## Workflow

1. Build the Elementor page, section, or component
2. Review the structure against the relevant blueprint (see `docs/`)
3. Verify styles match the style guide (see `docs/STYLE_GUIDE.md`)
4. Export as JSON from Elementor
5. Save the `.json` file here with the correct naming format
6. Update the relevant section map in `../section-maps/` if the page structure changed
7. Commit only the updated section map and public documentation (not this template)

If the owner approves sharing a template publicly:
1. Move the `.json` file to `../references/exports/`
2. Stage and commit with public files
3. Update public documentation links if needed

See [AGENTS.md](../../AGENTS.md) for detailed rules on when to commit.

See [REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md](../../docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md) for complete output workflow guidance.
