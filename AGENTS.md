# 1st Providence Rebuild — Codex Instructions

## Project Goal

This project is for rebuilding the 1st Providence homepage body using WordPress and Elementor.

The build should be modern, editable, responsive, and compatible with current Elementor container-based layouts.

## Main Rules

1. Do not touch the header unless explicitly requested.
2. Do not touch the footer unless explicitly requested.
3. Build homepage body content only unless the task says otherwise.
4. Use Elementor Containers, not legacy Sections or Columns.
5. Prefer native Elementor widgets over custom HTML.
6. Keep all text, images, buttons, cards, and layout content editable inside Elementor.
7. Use global styles for repeated colors, typography, buttons, spacing, borders, radius, and visual treatments.
8. Do not repeatedly hardcode the same colors or font settings inside individual widgets.
9. Do not use unnecessary custom CSS or JavaScript unless Elementor cannot achieve the design.
10. Work section by section. Do not generate the full homepage blindly.

## 1st Providence Project Typography and Button Lock

These typography and button values apply only to the 1st Providence rebuild project.

Do not treat these values as universal defaults for future websites. If this Codex skill folder is reused in another project, the new project must define its own typography, colors, and button system inside that project's AGENTS.md or project-specific reference files.

For this 1st Providence project, maintain the established Elementor Site Settings typography and button system unless the user explicitly changes it.

### Typography

Hero H1:
- Desktop: 45px
- Tablet: 38px
- Mobile: 32px
- Line height: 1.1-1.15
- Weight: 900

H2 Section Heading:
- Desktop: 34px
- Tablet: 30px
- Mobile: 26px
- Line height: 1.2
- Weight: 800

H3 / Card Heading:
- Desktop: 22px
- Tablet: 20px
- Mobile: 19px
- Line height: 1.25
- Weight: 800

Body Text:
- Desktop: 16px
- Tablet: 16px
- Mobile: 15px
- Line height: 1.6-1.7
- Weight: 400/500

Hero Subtitle:
- Desktop: 24px
- Tablet: 21px
- Mobile: 18px
- Line height: 1.35-1.45
- Weight: 600/700

Button Text:
- Desktop: 14px
- Tablet: 14px
- Mobile: 13px
- Line height: 1.0
- Weight: 800

### Button Style

Use the established 1st Providence button system:

- Font family: Nunito Sans
- Font weight: 800 ExtraBold
- Text transform: Uppercase
- Letter spacing: 1.5px
- Text color: #FFFFFF
- Background color: #A72D34
- Hover background: #8F252B
- Border radius: 4-6px
- Desktop padding: 14px top/bottom, 30px left/right
- Mobile padding: 12px top/bottom, 24px left/right

### Enforcement Rule

When creating or updating Elementor templates for this project:
- Do not invent new typography sizes unless the user explicitly requests a change.
- Do not invent new button styles unless the section requires a unique exception.
- Use the project Site Settings values first.
- Any exception must be documented in the relevant section map.

## Skill Files

Use these supporting instruction files when relevant:

### Elementor debugging

Read these before diagnosing WordPress, Elementor, preview, REST API, cache, server, or editor issues:

- `codex-skills/wordpress-elementor-debugging.md`
- `codex-skills/elementor-system-architecture.md`

### Elementor design and layout

Read these before planning or building Elementor homepage sections:

- `codex-skills/elementor-senior-design-system.md`
- `codex-skills/distinctive-frontend-design.md`
- `codex-skills/elementor-global-styles-site-settings.md`

### Instruction file maintenance

Read this before creating, rewriting, or auditing Codex instruction files:

- `codex-skills/codex-instruction-authoring.md`

## Homepage Build Workflow

When building the homepage body:

1. Analyze the reference section first.
2. Identify the section goal.
3. Define the container structure.
4. List the required Elementor widgets.
5. Identify global styles needed.
6. Define desktop, tablet, and mobile behavior.
7. Build with Elementor Containers only.
8. Keep everything editable in Elementor.
9. Validate that the section does not affect the header or footer.
10. Document the section in a section map.

## Output Expectations

For Elementor section planning, provide:

1. Section goal.
2. Reference analysis.
3. Container hierarchy.
4. Widget list.
5. Global styles needed.
6. Spacing values.
7. Typography specs.
8. Responsive notes.
9. Quality check.

For debugging, provide:

1. Diagnosis.
2. Suspected layer.
3. Root cause analysis.
4. Recommended debug steps.
5. Fix plan.
6. Rollback plan.

## Hard Boundaries

Do not:

1. Modify header or footer unless asked.
2. Use legacy Elementor Sections or Columns for new builds.
3. Generate static HTML when editable Elementor widgets can be used.
4. Invent unsupported Elementor widget names.
5. Modify unrelated pages, templates, or global settings without permission.
6. Ignore global styles.
7. Overbuild with unnecessary nested containers.
8. Apply random AI-style gradients, glows, or cards without design reason.
