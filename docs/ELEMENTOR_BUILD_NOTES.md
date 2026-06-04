# Elementor Build Notes

## Build Method

All page body plans use Elementor Containers and native widgets wherever possible. The rebuild avoids legacy Sections and Columns.

Editable content should use:

- Heading widgets for headings.
- Text Editor widgets for paragraphs, lists, and inline links.
- Button widgets for calls to action.
- Image widgets for page images.
- Icon widgets for benefit grids.
- Google Maps widget for map sections.

## Header And Footer Boundary

The header and footer are global. Program page bodies must begin below the header and end above the footer.

Do not copy header or footer markup into page-body templates.

## Scoped CSS Guidance

Scoped CSS is acceptable only for:

- Responsive grid layouts.
- Controlled image cropping.
- Icon circle treatments.
- Button hover consistency.
- Section-specific overlap behavior that cannot be safely handled with Elementor controls.

Avoid custom JavaScript for normal page sections.

## Completed Page Body Blueprints

- Testimonials
- Meet Our Trainers
- Nurse Aide
- Medication Aide 68 Hour
- Medication Management
- Electrocardiogram Technician

## Import Notes

This public repository does not include Elementor JSON exports. Production imports should be handled from private project storage only.

After importing any private Elementor template, verify:

- Header and footer remain global.
- Body sections appear in the documented order.
- Text, images, icons, buttons, and map widgets are editable.
- Mobile stacking is clean.
- Button links have been replaced with final URLs.
