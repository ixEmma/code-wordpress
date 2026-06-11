# Personal Care Aide (PCA) Program Page Blueprint

## Scope

Build the Personal Care Aide (PCA) program page body only. Do not edit, copy, or recreate the global header or footer.

This blueprint is public-safe documentation for implementation in Elementor. It does not include Elementor exports, screenshots, media assets, private templates, database content, or finished client page output.

## Design Direction

Healthcare education program page matching the provided PCA reference: compact caregiving image hero, strong Providence-blue intro, clean two-column requirements section, established dark healthcare career CTA, and full-width map directly above the global footer.

## Reference Observations

- The header and footer are global site chrome and must remain outside the page-body template.
- The hero uses a hands/caregiving image with a dark navy overlay and centered white uppercase title.
- The intro is a full-width Providence-blue band with centered white text.
- The details section is sparse and practical: image left, program requirements right, red CTA button.
- The final CTA matches the established dark medical-team background treatment used on other program pages.
- The map sits directly above the global footer.

## Page Body Section List

1. Hero Banner
2. Blue Intro Section
3. Personal Care Aide Details Section
4. Final Healthcare Career CTA Section
5. Map Section

## Class Names

Use only the PCA page prefix below for page-specific classes:

- `provpca-page`
- `provpca-hero`
- `provpca-hero-overlay`
- `provpca-hero-inner`
- `provpca-hero-title`
- `provpca-intro`
- `provpca-intro-inner`
- `provpca-intro-title`
- `provpca-intro-text`
- `provpca-details`
- `provpca-details-inner`
- `provpca-details-grid`
- `provpca-details-image`
- `provpca-details-content`
- `provpca-details-title`
- `provpca-details-subtitle`
- `provpca-details-list`
- `provpca-button`
- `provpca-career-cta`
- `provpca-career-overlay`
- `provpca-career-inner`
- `provpca-career-title`
- `provpca-career-text`
- `provpca-career-button`
- `provpca-map-section`

## Global Styles To Reuse

- Font family: Nunito Sans through Elementor Site Settings.
- Providence blue: `#004990`.
- Dark navy: `#001932`.
- Dark red button: `#A72D34`.
- Button hover red: `#8F252B`.
- White: `#FFFFFF`.
- Main text: `#1F2933`.
- Hero H1: 45px desktop, 38px tablet, 32px mobile, weight 900, line height 1.1-1.15.
- H2 section heading: 34px desktop, 30px tablet, 26px mobile, weight 800, line height 1.2.
- H3/card heading: 22px desktop, 20px tablet, 19px mobile, weight 800, line height 1.25.
- Body text: 16px desktop/tablet, 15px mobile, line height 1.6-1.7.
- Buttons: uppercase, 14px desktop/tablet, 13px mobile, weight 800, 1.5px letter spacing, 4-6px radius, 14px 30px desktop padding, 12px 24px mobile padding.

Do not change Elementor global Site Settings for this page. Use scoped CSS only when Elementor controls cannot match the reference, such as grid behavior, image cropping, overlay opacity, or map height.

## Section 1: Hero Banner

### Section Goal

Introduce the PCA program with a compact caregiving image banner and centered program name.

### Container Hierarchy

```txt
PCA Hero Banner
  Hero Inner Container
    Heading widget: PERSONAL CARE AIDE (PCA)
```

### Widget List

- Heading widget
- Editable section background image
- Elementor background overlay

### Content

Heading:

```txt
PERSONAL CARE AIDE (PCA)
```

### Image Direction

Use an approved caregiving image similar to the reference: hands holding/supporting another person's hand, caregiver support, patient care, or home-care assistance. Do not commit the image to the public repo.

### Spacing Values

- Full-width section.
- Desktop height: around 300px.
- Tablet height: around 240px.
- Mobile height: around 190px.
- Background size: cover.
- Background position: center, adjusted to keep the caregiving interaction visible.

### Typography Specs

- Color: `#FFFFFF`.
- Text transform: uppercase.
- Font weight: 900.
- Font size: use global Hero H1 where possible; if a page-specific match is needed, keep near 42px desktop, 34px tablet, 28px mobile.
- Line height: 1.1.
- Text align: center.

### Responsive Notes

Keep the heading centered vertically and horizontally at every breakpoint. Avoid cropping the main hands/caregiving subject out of view.

## Section 2: Blue Intro Section

### Section Goal

Summarize the PCA program value proposition and Medicaid Waivers care context.

### Container Hierarchy

```txt
PCA Blue Intro
  Intro Inner Container
    Heading widget
    Text Editor widget
```

### Widget List

- Heading widget
- Text Editor widget

### Content

Heading:

```txt
The Personal Care Aide program teaches students the basics of providing personal care services under Medicaid Waivers.
```

Body:

```txt
In this course, the student will learn the requirements that are necessary for safely and effectively provide personal care assistance to residents and clients.
```

### Global Styles Needed

- Background: Providence blue `#004990`.
- Text: white `#FFFFFF`.
- Inner max width: 1120px.
- Heading max width: around 980px.
- Body max width: around 1000px.

### Spacing Values

- Desktop padding: 70px top, 75px bottom, 24px sides.
- Tablet padding: 58px top/bottom, 22px sides.
- Mobile padding: 42px top/bottom, 22px sides.
- Heading bottom margin: around 22px.

### Typography Specs

- Intro heading: use global H2; if matching the reference requires a stronger value, keep near 34-36px desktop, 30px tablet, 25-26px mobile, weight 900, line height 1.22.
- Body: 15-16px, line height around 1.75.

### Responsive Notes

Text remains centered on all breakpoints. Keep line length readable rather than stretching the paragraph edge to edge.

## Section 3: Personal Care Aide Details Section

### Section Goal

Present the PCA program requirements and primary `GET STARTED` action in a clean image-and-content layout.

### Container Hierarchy

```txt
PCA Details Section
  Details Inner Container
    Details Grid Container
      Details Image Container
        Image widget
      Details Content Container
        Heading widget
        Heading widget: Requirements:
        Text Editor widget with bullet list
        Button widget
```

### Widget List

- Image widget
- Two Heading widgets
- Text Editor widget
- Button widget

### Content

Heading:

```txt
Personal Care Aide (PCA)
```

Subheading:

```txt
Requirements:
```

Bullet list:

```txt
Valid Identification card (driver's license, state ID, passport)
Students must be at least 18 years of age
```

Button:

```txt
GET STARTED
```

Button link:

```txt
#
```

### Image Direction

Use an editable Elementor Image widget showing a caregiver helping an older adult with a walker, personal care support, senior care, or home-care assistance. Keep the image rectangular like the reference unless a global image radius is already in use.

### Global Styles Needed

- Background: white `#FFFFFF`.
- Details heading: Providence blue `#004990`.
- Body/list text: `#1F2933`.
- Button: project button lock.

### Spacing Values

- Desktop padding: 85px top/bottom, 24px sides.
- Tablet padding: 65px top/bottom, 22px sides.
- Mobile padding: 45px top/bottom, 22px sides.
- Inner max width: 1120px.
- Desktop column gap: around 70px.
- Tablet column gap: around 40px.
- Mobile stack gap: around 30px.
- Image height: around 300px desktop, 240px mobile.

### Typography Specs

- Details title: use global H2/H3 hierarchy; for screenshot match, keep near 32px desktop and 26px mobile, weight 900, line height 1.2.
- Requirements subheading: 16px, weight 900, line height 1.4.
- List text: 15px, line height 1.7.
- Button: project button lock.

### Responsive Notes

Desktop uses two columns with image left and content right. Mobile stacks image first, content second. Keep text left aligned; if the mobile composition feels unbalanced, center only the heading and button while keeping the list readable.

## Section 4: Final Healthcare Career CTA Section

### Section Goal

Close with the established 1st Providence healthcare career CTA and a contact action.

### Container Hierarchy

```txt
PCA Career CTA
  Career Inner Container
    Heading widget
    Text Editor widget
    Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget
- Editable section background image
- Elementor background overlay

### Content

Heading:

```txt
Are You Ready to Start Your Career in Healthcare?
```

Body:

```txt
We're here to help you take the next step! Contact us today to enroll in our high-quality training programs today.
```

Button:

```txt
CONTACT US
```

Button link:

```txt
#
```

### Image Direction

Use the approved dark healthcare surgical/medical team CTA background already used across other 1st Providence pages where available.

### Global Styles Needed

- Dark navy overlay: `rgba(0, 25, 50, 0.75)` or Elementor equivalent.
- White heading and body text.
- Button: project button lock.

### Spacing Values

- Desktop padding: 95px top/bottom, 24px sides.
- Tablet padding: 75px top/bottom, 22px sides.
- Mobile padding: 60px top/bottom, 22px sides.
- Inner max width: 1120px.

### Typography Specs

- CTA heading: use global H2; if matching the reference requires a stronger value, keep near 34-36px desktop, 30px tablet, 27px mobile, weight 900, line height 1.2.
- CTA text: 16px desktop, 15px mobile, line height 1.65.
- Button: project button lock.

### Responsive Notes

Keep all text centered. Background image remains cover-sized and should keep the surgical team faces/medical context recognizable.

## Section 5: Map Section

### Section Goal

Show the Woodbridge location directly above the global footer.

### Container Hierarchy

```txt
PCA Map Section
  Google Maps widget
```

### Widget List

- Elementor Google Maps widget preferred

### Content

Address:

```txt
1549 Old Bridge Rd Suite 208
Woodbridge, VA 22192
```

### Spacing Values

- Desktop height: 360-420px.
- Tablet height: 320px.
- Mobile height: 260px.
- Full width.

### Responsive Notes

Map should sit flush above the global footer like the reference. Enable scroll prevention if available so mobile users do not get trapped in the map while scrolling the page.

## Scoped CSS Guidance

Prefer Elementor controls and global styles first. Add scoped page CSS only for:

- `overflow-x: hidden` on `.provpca-page`.
- Fixed responsive hero, image, and map heights.
- Details grid columns and mobile stacking.
- Controlled image `object-fit: cover`.
- Page-specific overlay opacity if Elementor controls cannot reproduce it.
- Button hover consistency if global button hover does not apply inside this template.

Do not use broad selectors or classes from other pages. Do not add styles to the global header or footer.

## Manual Image Replacement Notes

- Hero background: replace with approved caregiving/hands/support image.
- Details image: replace with approved caregiver helping older adult, walker support, or home-care assistance image.
- Final CTA background: reuse the approved dark healthcare surgical/medical team CTA image.
- Do not commit any selected media assets to this public repository.

## Button Link Notes

- Details `GET STARTED`: currently `#`.
- Final CTA `CONTACT US`: currently `#`.
- Replace placeholders only when final URLs are confirmed in the private WordPress implementation.

## Elementor Compatibility Notes

- Use Elementor Containers only; do not use legacy Sections or Columns.
- Use native Elementor Heading, Text Editor, Image, Button, and Google Maps widgets.
- Keep text, images, buttons, background images, and map editable in Elementor.
- Keep this page body separate from the global header and footer.
- Do not modify Elementor Site Settings for this page.
- Do not flatten sections into a single text block.

## Quality Check

- Page order is exactly: hero banner, blue intro section, PCA details section, final CTA section, map section.
- Header and footer are not duplicated or modified.
- All typography, colors, buttons, and spacing follow the established 1st Providence global design system.
- Page-specific classes use only the `provpca-*` prefix.
- Button links remain placeholders until final URLs are available.
- No Elementor export JSON, screenshots, media assets, backups, or database files are added to the public repo.
