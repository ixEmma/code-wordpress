# Elementor Reference Index

This folder contains existing Elementor JSON exports that Codex can study before generating new Elementor templates.

## Rule

These files are reference material only.

Do not overwrite these files.
Do not treat these as final homepage output files.
Use them to understand Elementor JSON structure, widget settings, container structure, spacing patterns, and export format.

## Reference Files

### exports/elementor-1458-2026-03-17 hero-section.json

Purpose:
Use this as a reference for Elementor hero section structure.

Study for:
- Container hierarchy
- Hero layout
- Heading, text, image, and CTA structure
- Responsive settings if available

### exports/elementor-1635-2026-03-17FAQ.json

Purpose:
Use this as a reference only if the homepage requires an FAQ or accordion-style section.

Study for:
- Repeated content structure
- FAQ widget or accordion pattern
- Spacing and section grouping

### exports/elementor-2536-2026-05-07- Merchandise page full.json

Purpose:
Use this as a broad reference for a larger Elementor page export.

Study for:
- Full page JSON structure
- Multi-section organization
- Container nesting patterns
- Repeated global style usage

### exports/elementor-about-section-2026-03-19.json

Purpose:
Use this as a reference for about, intro, or content-image sections.

Study for:
- Text and image layout
- Section spacing
- Content hierarchy
- Responsive stacking

## Important Boundary

The current 1st Providence rebuild should only create new generated files inside:

../elementor-templates/
../section-maps/

Do not edit the files in this references folder unless explicitly asked.

### global-styles-site-settings.md

Purpose:
Use this as the main global style and Elementor Site Settings reference for the 1st Providence rebuild.

Study for:
- Global colors
- Global fonts
- Typography sizes
- Button styles
- Link colors
- Section backgrounds
- Hero overlay
- Dark section styling

Important:
Before generating Elementor templates, use this file to define the global style map.