# Build Lessons

## Date

2026-05-27

## Build Name

1st Providence Homepage Body Elementor Template

## Reference Files Used

- `AGENTS.md`
- `codex-skills/elementor-global-styles-site-settings.md`
- `codex-skills/elementor-system-architecture.md`
- `codex-skills/elementor-senior-design-system.md`
- `codex-skills/distinctive-frontend-design.md`
- `elementor-outputs/references/REFERENCE_INDEX.md`
- `elementor-outputs/section-maps/reference-analysis-report.md`
- `elementor-outputs/references/exports/elementor-1458-2026-03-17 hero-section.json`
- `elementor-outputs/references/exports/elementor-1635-2026-03-17FAQ.json`
- `elementor-outputs/references/exports/elementor-2536-2026-05-07- Merchandise page full.json`
- `elementor-outputs/references/exports/elementor-about-section-2026-03-19.json`
- `elementor-outputs/screenshots/homepage-full-reference.png.png`

Note: `elementor-outputs/references/global-styles-site-settings.md` was requested but was not present at that path. The build used the explicit global style values supplied in the task.

## Elementor Export Patterns Reused

- Top-level Elementor export shape: `content`, `page_settings`, `version`, `title`, and `type`.
- Modern `container` elements only.
- Native editable widgets: `heading`, `text-editor`, `button`, `image`, and `google_maps`.
- Full-width outer containers with boxed inner containers for content rhythm.
- Split row layouts for hero-style and mission-style sections.
- Card-row pattern adapted from the about and merchandise references.
- Background image plus blue overlay pattern adapted from the hero reference and homepage screenshot.

## What Was Generated

- `elementor-outputs/elementor-templates/homepage-body-template.json`
- `elementor-outputs/section-maps/homepage-body-section-map.md`
- `elementor-outputs/section-maps/BUILD_LESSONS.md`

The generated template includes these body-only sections:

- Hero section
- Welcome / badges / accreditation section
- Three image link cards section
- Mission section
- Testimonials section
- CTA banner section
- Map section

The generated template excludes:

- Header
- Navigation
- Logo area
- Footer
- Footer social links
- Legal links
- Copyright
- Footer contact details

## What Needs Testing After Import

- Import the JSON into Elementor and confirm it appears as a page/body template.
- Confirm Containers are active and no legacy Sections/Columns were created.
- Confirm remote placeholder images display or replace them with media-library images.
- Add the real badge and accreditation logo assets.
- Confirm Google Maps widget renders with the Woodbridge address.
- Confirm desktop, tablet, and mobile stacking behavior.
- Confirm Elementor Site Settings include Nunito Sans and the global color tokens.
- Confirm button links point to the intended contact destination.
- Regenerate Elementor CSS after import if styling appears stale.

## Risks or Assumptions

- The exact global site-settings markdown under `elementor-outputs/references/` was missing, so the supplied color/font list was treated as the visual source of truth.
- The screenshot file existed as `homepage-full-reference.png.png`, not `homepage-full-reference.png`.
- The generated image URLs are replaceable placeholders and should be swapped for approved 1st Providence media assets.
- Global styles are documented in the section map instead of being imported as generated global variable IDs, because generated IDs may not map cleanly to the active Elementor Kit.
- The map uses the native Elementor `google_maps` widget; if the target install disables that widget, replace it manually after import.
- The template was generated body-only and should be imported into a page/template that already handles header and footer separately.

## Import Fix Applied

After the first import attempt, Elementor returned `Invalid File`.

Fixes applied:

- Rewrote `homepage-body-template.json` as UTF-8 without BOM. The first generated file had a BOM prefix, while the working reference exports start directly with `{`.
- Compacted the JSON to match the reference export style.
- Changed `page_settings` from an empty array to an object with `hide_title: yes`.
- Removed generated top-level `global_variables` and kept the global style system documented in the section map instead.

---

## Date

2026-05-28

## Build Name

Contact Page Body Template

## Reference Screenshot Used

- `elementor-outputs/screenshots/contact-page-reference.png` was requested but was not present on disk.
- The attached contact page screenshot in the prompt was used as the visual reference.

## Reference Exports Used

- `AGENTS.md`
- `codex-skills/elementor-global-styles-site-settings.md`
- `codex-skills/elementor-system-architecture.md`
- `codex-skills/elementor-senior-design-system.md`
- `codex-skills/distinctive-frontend-design.md`
- `elementor-outputs/references/global-styles-site-settings.md`
- `elementor-outputs/references/REFERENCE_INDEX.md`
- `elementor-outputs/section-maps/reference-analysis-report.md`

## Elementor Patterns Reused

- Top-level Elementor JSON export shape with `content`, `page_settings`, `version`, `title`, and `type`.
- Modern Elementor `container` elements only.
- Full-width outer containers with boxed inner containers.
- Two-column desktop layout that stacks on mobile.
- Native editable widgets: `heading`, `text-editor`, `form`, and `image`.
- Replaceable Image widgets for accreditation badges.

## What Was Generated

- `elementor-outputs/elementor-templates/contact-page-body-template.json`
- `elementor-outputs/section-maps/contact-page-section-map.md`
- Appended this entry to `elementor-outputs/section-maps/BUILD_LESSONS.md`

The generated contact page body includes:

- Page title banner
- Contact information + Elementor Pro form section
- Accreditation badge row section

The generated template excludes:

- Header
- Navigation
- Logo area
- Footer
- Footer social links
- Legal links
- Copyright
- Footer contact details

## What Needs Testing After Import

- Confirm Elementor imports the JSON as a page/body template.
- Confirm Containers are active and no legacy Sections or Columns appear.
- Confirm Elementor Pro Form widget renders.
- Configure form actions, recipient email, confirmation message, and anti-spam/reCAPTCHA if needed.
- Replace the three badge Image widgets with approved 1st Providence badge assets.
- Confirm desktop, tablet, and mobile spacing against the contact page screenshot.
- Regenerate Elementor CSS after import if style output looks stale.

## Risks or Assumptions

- Elementor Pro is required for the Form widget.
- The screenshot file path requested by name was missing locally, so the attached prompt image was used.
- Form action settings are intentionally not finalized because target email/action requirements may vary.
- Badge image URLs are empty placeholders so the images remain replaceable in Elementor.
- Global styles are represented as explicit project values because stable Elementor Kit global IDs were not available.

---

## Date

2026-05-28

## Build Name

Class Schedule Page Body Template

## Reference Screenshot Used

- `elementor-outputs/screenshots/class-schedule-page-reference.png` was requested but was not present on disk.
- The attached class schedule page screenshot in the prompt was used as the visual reference.

## Reference Exports Used

- `AGENTS.md`
- `codex-skills/elementor-global-styles-site-settings.md`
- `codex-skills/elementor-system-architecture.md`
- `codex-skills/elementor-senior-design-system.md`
- `codex-skills/distinctive-frontend-design.md`
- `elementor-outputs/references/global-styles-site-settings.md`
- `elementor-outputs/references/REFERENCE_INDEX.md`
- `elementor-outputs/section-maps/reference-analysis-report.md`

## Elementor Patterns Reused

- Top-level Elementor export shape with `content`, `page_settings`, `version`, `title`, and `type`.
- Modern Elementor `container` elements only.
- Full-width hero and CTA background-image sections with dark blue overlays.
- Boxed inner containers for readable content.
- Native editable widgets: `heading`, `text-editor`, `button`, and `google_maps`.
- Google Maps section pattern from the existing homepage body template.

## What Was Generated

- `elementor-outputs/elementor-templates/class-schedule-page-body-template.json`
- `elementor-outputs/section-maps/class-schedule-page-section-map.md`
- Appended this entry to `elementor-outputs/section-maps/BUILD_LESSONS.md`

The generated class schedule page body includes:

- Class Schedule hero banner
- Class schedule table section
- CTA banner section
- Map section

The generated template excludes:

- Header
- Logo area
- Navigation
- Footer
- Footer social links
- Legal links
- Copyright
- Footer contact details

## What Needs Testing After Import

- Confirm Elementor imports the JSON as a page/body template.
- Confirm Containers are active and no legacy Sections or Columns appear.
- Replace hero and CTA background images with approved media-library assets.
- Confirm the Text Editor schedule table is readable and horizontally scrollable on mobile.
- Update the Contact Us button link.
- Confirm the Google Maps widget renders the Woodbridge address.
- Regenerate Elementor CSS after import if styling appears stale.

## Risks or Assumptions

- The screenshot file path requested by name was missing locally, so the attached prompt image was used.
- The schedule table uses a Text Editor HTML table fallback because the inspected references did not include a native table widget.
- Table content is editable inside one Text Editor widget, but individual cells are not separate Elementor widgets.
- Inline table CSS is used to preserve the screenshot-like table and mobile horizontal scroll without JavaScript.
- Google Maps widget may require manual configuration or replacement depending on the target Elementor setup.
- Background image URLs are replaceable placeholders and should be swapped with approved 1st Providence assets.

---

## Date

2026-05-28

## Build Name

Tuition Page Body Template

## Reference Screenshot Used

- `elementor-outputs/screenshots/tuition-page-reference.png` was requested but was not present on disk.
- The attached tuition page screenshot in the prompt was used as the visual reference.

## Reference Exports Used

- `AGENTS.md`
- `codex-skills/elementor-global-styles-site-settings.md`
- `codex-skills/elementor-system-architecture.md`
- `codex-skills/elementor-senior-design-system.md`
- `codex-skills/distinctive-frontend-design.md`
- `elementor-outputs/references/global-styles-site-settings.md`
- `elementor-outputs/references/REFERENCE_INDEX.md`
- `elementor-outputs/section-maps/reference-analysis-report.md`

## Elementor Patterns Reused

- Top-level Elementor export shape with `content`, `page_settings`, `version`, `title`, and `type`.
- Modern Elementor `container` elements only.
- Full-width hero and CTA background-image sections with dark blue overlays.
- Centered table section using a boxed inner container.
- Two-column content/image layout that stacks on mobile.
- Native editable widgets: `heading`, `text-editor`, `image`, `button`, and `google_maps`.
- Google Maps section pattern from the existing homepage and class schedule templates.

## What Was Generated

- `elementor-outputs/elementor-templates/tuition-page-body-template.json`
- `elementor-outputs/section-maps/tuition-page-section-map.md`
- Appended this entry to `elementor-outputs/section-maps/BUILD_LESSONS.md`

The generated tuition page body includes:

- Tuition hero banner
- Tuition table section
- Enroll Today section
- CTA banner section
- Map section

The generated template excludes:

- Header
- Logo/navigation
- Footer
- Footer social links
- Legal links
- Copyright
- Footer contact details

## What Needs Testing After Import

- Confirm Elementor imports the JSON as a page/body template.
- Confirm Containers are active and no legacy Sections or Columns appear.
- Replace hero, enroll, and CTA images with approved media-library assets.
- Confirm the Text Editor tuition table is readable and horizontally scrollable on mobile.
- Update Enroll Now and Contact Us button links.
- Confirm the Google Maps widget renders the Woodbridge address.
- Regenerate Elementor CSS after import if styling appears stale.

## Risks or Assumptions

- The screenshot file path requested by name was missing locally, so the attached prompt image was used.
- The tuition table uses a Text Editor HTML table fallback because the inspected references did not include a native table widget.
- Table content is editable inside one Text Editor widget, but individual cells are not separate Elementor widgets.
- Inline table CSS is used to preserve the screenshot-like table and mobile horizontal scroll without JavaScript.
- Google Maps widget may require manual configuration or replacement depending on the target Elementor setup.
- Image URLs are replaceable placeholders and should be swapped with approved 1st Providence assets.

---

## Date

2026-05-28

## Build Name

Student Resources Page Body Template

## Reference Screenshot Used

- `elementor-outputs/screenshots/student-resources-page-reference.png` was requested but was not present on disk.
- The attached student resources page screenshot in the prompt was used as the visual reference.

## Reference Exports Used

- `AGENTS.md`
- `codex-skills/elementor-global-styles-site-settings.md`
- `codex-skills/elementor-system-architecture.md`
- `codex-skills/elementor-senior-design-system.md`
- `codex-skills/distinctive-frontend-design.md`
- `elementor-outputs/references/global-styles-site-settings.md`
- `elementor-outputs/references/REFERENCE_INDEX.md`
- `elementor-outputs/section-maps/reference-analysis-report.md`

## Elementor Patterns Reused

- Top-level Elementor export shape with `content`, `page_settings`, `version`, `title`, and `type`.
- Modern Elementor `container` elements only.
- Full-width hero and CTA background-image sections with dark overlays.
- Stacked boxed content layout for resource rows.
- Native editable widgets: `heading`, `text-editor`, `button`, and `google_maps`.
- Google Maps section pattern from the existing generated page templates.

## What Was Generated

- `elementor-outputs/elementor-templates/student-resources-page-body-template.json`
- `elementor-outputs/section-maps/student-resources-page-section-map.md`
- Appended this entry to `elementor-outputs/section-maps/BUILD_LESSONS.md`

The generated student resources page body includes:

- Student Resources hero banner
- Resource links section
- CTA banner section
- Map section

The generated template excludes:

- Header
- Logo area
- Navigation
- Footer
- Footer social links
- Legal links
- Copyright
- Footer contact details

## What Needs Testing After Import

- Confirm Elementor imports the JSON as a page/body template.
- Confirm Containers are active and no legacy Sections or Columns appear.
- Replace hero and CTA background images with approved media-library assets.
- Replace all `#` resource link placeholders with final URLs.
- Confirm resource button hover color changes to CTA Red.
- Confirm longer resource labels wrap cleanly on mobile.
- Confirm the Google Maps widget renders the Woodbridge address.
- Regenerate Elementor CSS after import if styling appears stale.

## Risks or Assumptions

- The screenshot file path requested by name was missing locally, so the attached prompt image was used.
- Resource rows are Elementor Button widgets styled as white link rows so each item has editable text and URL fields.
- Final URLs are unknown, so each resource item uses `#` as a placeholder.
- Elementor Button hover style control names can vary by version, so hover color should be checked after import.
- Google Maps widget may require manual configuration or replacement depending on the target Elementor setup.
- Background image URLs are replaceable placeholders and should be swapped with approved 1st Providence assets.
