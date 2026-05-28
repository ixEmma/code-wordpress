# Elementor Reference Analysis Report

## 1. Reference Files Inspected

Project and instruction files read:

- `AGENTS.md`
- `codex-skills/elementor-global-styles-site-settings.md`
- `codex-skills/elementor-system-architecture.md`
- `codex-skills/elementor-senior-design-system.md`
- `elementor-outputs/references/REFERENCE_INDEX.md`

Elementor JSON exports inspected:

- `elementor-outputs/references/exports/elementor-1458-2026-03-17 hero-section.json`
- `elementor-outputs/references/exports/elementor-1635-2026-03-17FAQ.json`
- `elementor-outputs/references/exports/elementor-2536-2026-05-07- Merchandise page full.json`
- `elementor-outputs/references/exports/elementor-about-section-2026-03-19.json`

No JSON files were modified.

## 2. Containers vs Legacy Sections/Columns

All inspected exports use modern Elementor container structure.

- `hero-section.json`: `type: container`; 6 containers, 8 widgets.
- `FAQ.json`: `type: container`; 13 containers, 12 widgets.
- `Merchandise page full.json`: `type: page`; 45 containers, 72 widgets.
- `about-section.json`: `type: container`; 6 containers, 10 widgets.

No legacy Elementor `section` or `column` element types were found in the inspected exports.

## 3. Common Widget Types Found

Across all exports, the common widget types are:

- `text-editor`: 39 instances.
- `heading`: 26 instances.
- `icon`: 14 instances.
- `image`: 12 instances.
- `button`: 5 instances.
- `divider`: 3 instances.
- `nested-accordion`: 1 instance.
- `rating`: 1 instance.
- `e-button`: 1 instance.

The references mostly rely on native editable Elementor widgets, especially headings, text editors, images, icons, buttons, and containers.

## 4. Common Container/Layout Patterns Found

Common layout patterns:

- Outer full-width container with nested content containers.
- `content_width: full` is used heavily across containers.
- Row-based split layouts appear in the hero, FAQ, about, and merchandise references.
- Column containers are used inside cards, text groups, and stacked mobile-friendly content groups.
- Repeated card-like nested containers appear in the about section and merchandise page.
- The FAQ export uses a two-column structure with an image side and a content/accordion side.
- The hero export uses a text/image split with nested CTA/button grouping.
- The merchandise export is the broadest full-page pattern, with multiple top-level containers and repeated content blocks.

Observed container settings:

- `flex_direction`: mostly `row`, with `column` used for stacked content.
- `flex_gap`: commonly `10px`; also observed `24px`, `25px`, and `40px`.
- `padding`: many containers use zero padding internally, while section-level padding appears at larger values such as `80px` top/bottom and `120px` top / `100px` bottom.
- Responsive padding is present in some exports, especially `20px` mobile side padding.
- Several containers use `css_classes`, `_title`, `hover_parallax`, and some `custom_css` fields.

## 5. Global Style References Found

Only the merchandise full-page export contains clear Elementor global variable references.

Found in `elementor-2536-2026-05-07- Merchandise page full.json`:

- Global variable `e-gv-2337a8d`
  - Label: `Text`
  - Value: `#0d162b`
- Global variable `e-gv-a664fd1`
  - Label: `off-white`
  - Value: `#f4fafd`

No global color or global typography token references were found in the hero, FAQ, or about exports.

Important note: several repeated styles are hardcoded directly in widget/container settings rather than consistently mapped to Elementor Site Settings.

## 6. Repeated Design Patterns

### Colors

Repeated or notable colors found:

- `#FFFFFF`: white background/card color.
- `#0D162B` / `#0d162b`: dark text/global text color in merchandise export.
- `#F4FAFD` / `#f4fafd`: off-white background/global color in merchandise export.
- `#111728`: dark button text in hero export.
- `#0F1826`: heading/title color in hero export.
- `#F7F1F1`: light background in about export.
- `#D88421`, `#F09F3C`, `#F7B766`: warm accent/orange values in hero export.
- `#165D66`: teal accent value in hero export.
- `#2AB4DE`: blue accent in merchandise export.
- `#E4222263`: translucent red hover color in about export.

Recommended global color candidates before future generation:

- Primary
- Accent Warm
- Accent Teal or Blue
- Text Dark
- Background White
- Background Off White
- Muted Background
- Button Text
- Border

### Typography

Typography is not consistently globalized in the exports.

Observed patterns:

- 13 `typography_typography: custom` settings.
- Heading and text alignment frequently set to `center`.
- Mobile heading sizes observed at `28px` and `36px`.
- Some small text sizes observed at `12px` and `14px`.
- One uppercase transform setting was found.

Before creating new templates, heading, body, eyebrow, card title, button, and small/meta typography should be defined as reusable global styles rather than repeated per widget.

### Spacing

Common spacing values:

- `10px` container gap is the most repeated gap.
- Larger gaps found: `24px`, `25px`, `40px`.
- Section-level padding examples:
  - `80px 0 40px 0`
  - `80px 0 80px 0`
  - `120px 0 100px 0`
  - `50px 0 30px 0`
- Mobile padding examples:
  - `20px` all sides.
  - `60px 20px 60px 20px`.
  - `40px 20px 40px 20px`.

Recommended global spacing candidates:

- Section padding desktop: 80px to 120px vertical.
- Section padding mobile: 40px to 60px vertical, 20px horizontal.
- Inner gap: 24px to 40px.
- Small widget gap: 10px.

### Radius and Borders

Repeated radius values:

- `8px`: common card/container radius.
- `50px`: pill button radius.
- `5px`: small radius.
- `24px`: larger card/media radius.

Border settings appear in several containers, but are not consistently abstracted into global style decisions.

### Buttons

Button patterns found:

- Hero CTA button: text `Get a Free Assenssment`, pill radius `50px`.
- Hero phone button: text `703. 496.4300`, pill radius `50px`, text color `#111728`.
- Merchandise CTA buttons: text `Start Your Brand ->`, one centered.
- About CTA button: text `View All Services`.

Recommended future button pattern:

- Global primary button style.
- Global secondary/phone button style if needed.
- Pill radius around `50px` only when it matches the section design.
- Avoid hardcoding repeated colors in each button widget.

## 7. Best Reference for Future Homepage Body Sections

Best broad reference: `elementor-2536-2026-05-07- Merchandise page full.json`.

Reason:

- It is the largest and most complete export.
- It shows multi-section page organization.
- It contains the most container patterns, repeated content groups, and widget variety.
- It is the only export with explicit `global_variables`.
- It gives the clearest view of full-page Elementor export structure.

Best section-specific references:

- Hero sections: `elementor-1458-2026-03-17 hero-section.json`.
- FAQ/accordion sections: `elementor-1635-2026-03-17FAQ.json`.
- About/content-card sections: `elementor-about-section-2026-03-19.json`.

For the 1st Providence homepage rebuild, use the merchandise export as the structural reference, then use the hero/about/FAQ exports only when their section pattern is directly relevant.

## 8. Risks Before Generating New Elementor JSON

- Global styles are inconsistent across the references. Most colors and typography are hardcoded rather than connected to Elementor Site Settings.
- The target Elementor Kit global colors and fonts are not confirmed yet. Generated JSON should not assume unavailable global variable IDs.
- Some exports contain custom CSS fields. New sections should avoid custom CSS unless Elementor widgets/containers cannot achieve the design.
- The FAQ export has relatively deep nesting around the nested accordion. Future templates should avoid unnecessary nesting.
- `content_width: full` is common, but future homepage body sections still need a controlled inner max-width pattern for readable content.
- Some responsive settings are sparse. Desktop, tablet, and mobile behavior must be explicitly planned for each new section.
- Existing image references may point to old/media-library assets and should not be assumed valid for the rebuild.
- Button text includes a typo in the hero reference: `Get a Free Assenssment`.
- The `e-button` widget appears once in the merchandise export. Confirm compatibility before using it in generated templates; prefer the standard native `button` widget when possible.
- Header and footer boundaries must remain protected. Future generated homepage body JSON should not include header/footer template content.

