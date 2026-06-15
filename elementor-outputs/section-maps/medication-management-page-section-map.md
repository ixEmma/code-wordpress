# 1st Providence Medication Management Page Section Map

## Page Body Section List

1. Hero Banner
2. Blue Medication Management Intro Section
3. Two-Column Medication Management Details Section
4. Final Healthcare Career CTA Section
5. Map Section

This template is body-only. It excludes the global header, navigation, logo area, global footer, footer social icons, footer links, legal links, copyright, and footer contact details.

## Design Direction

Healthcare training program page matching the supplied Medication Management reference: a compact image hero, strong Providence-blue explanatory intro, clean two-column course details, established dark medical CTA, and full-width map directly before the global footer.

## Reference Observations

- The header and footer are global site chrome and are not part of this body template.
- The page starts with a short hero banner using a darkened healthcare/classroom writing image.
- The blue intro carries most of the educational explanation and is centered, wide, and text-forward.
- The details section is sparse and practical, with image left and course details right.
- The CTA and map match the visual pattern used across existing 1st Providence pages.

## Class Names Used

- `provmanage-page`
- `provmanage-hero`
- `provmanage-hero-overlay`
- `provmanage-hero-title`
- `provmanage-intro`
- `provmanage-intro-inner`
- `provmanage-intro-title`
- `provmanage-intro-text`
- `provmanage-details`
- `provmanage-details-inner`
- `provmanage-details-grid`
- `provmanage-details-image`
- `provmanage-details-content`
- `provmanage-details-title`
- `provmanage-details-text`
- `provmanage-details-list`
- `provmanage-button`
- `provmanage-career-cta`
- `provmanage-career-overlay`
- `provmanage-career-inner`
- `provmanage-career-title`
- `provmanage-career-text`
- `provmanage-career-button`
- `provmanage-map-section`

## Section 1: Hero Banner

### Section Goal

Introduce the page with the program name in a compact, centered image hero.

### Container Hierarchy

```txt
Medication Management Hero
  HTML widget: scoped page CSS
  Heading widget: MEDICATION MANAGEMENT
```

### Widget List

- HTML widget for scoped CSS
- Heading widget

### Global Styles Needed

- Dark navy overlay: `#001932`
- White hero title
- Nunito Sans/global heading typography

### Spacing Values

- Desktop height: 300px
- Tablet height: 240px
- Mobile height: 190px
- Section padding: 70px desktop, 54px tablet, 42px mobile

### Typography Specs

- Hero title: 42px desktop, 36px tablet, 30px mobile, weight 900, uppercase, line height 1.1

### Responsive Notes

- Background image remains cover-sized and centered.
- Heading stays centered vertically and horizontally.

## Section 2: Blue Medication Management Intro Section

### Section Goal

Explain who the course is for, what the training includes, and the regulatory approval context.

### Container Hierarchy

```txt
Blue Medication Management Intro
  Intro Inner
    Heading widget
    Text Editor widget with three paragraphs
```

### Widget List

- Heading widget
- Text Editor widget

### Global Styles Needed

- Providence blue: `#004990`
- White heading and paragraph text

### Spacing Values

- Desktop padding: 75px top/bottom, 24px sides
- Tablet padding: 60px top/bottom, 22px sides
- Mobile padding: 45px top/bottom, 22px sides
- Inner max width: 1120px
- Heading max width: 980px

### Typography Specs

- Intro heading: 36px desktop, 30px tablet, 26px mobile, weight 900, line height 1.2
- Paragraphs: 15px, line height 1.75

### Responsive Notes

- Text remains centered at all breakpoints.
- Paragraphs keep a readable max width.

## Section 3: Medication Management Details Section

### Section Goal

Present class size, requirements, fee/contact guidance, and the primary `GET STARTED` action.

### Container Hierarchy

```txt
Medication Management Details
  Details Inner
    Details Grid
      Details Image Column
        Image widget
      Details Content
        Heading widget
        Text Editor widget
        Heading widget: Requirements
        Text Editor bullet list
        Text Editor widget
        Button widget
```

### Widget List

- Image widget
- Two Heading widgets
- Three Text Editor widgets
- Button widget

### Global Styles Needed

- White background
- Providence blue heading: `#004990`
- Body text: `#1F2933`
- Button red: `#A72D34`
- Button hover: `#8F252B`

### Spacing Values

- Desktop padding: 85px top/bottom, 24px sides
- Tablet padding: 65px top/bottom, 22px sides
- Mobile padding: 45px top/bottom, 22px sides
- Inner max width: 1120px
- Desktop grid gap: 65px
- Image height: 300px desktop, 240px mobile

### Typography Specs

- Details title: 30px desktop, 26px mobile, weight 900, line height 1.2
- Requirements subheading: 16px, weight 800
- Body/list text: 15px, line height 1.65-1.7
- Button: project button lock, uppercase, 14px desktop, 13px mobile, weight 800, 1.5px letter spacing

### Responsive Notes

- Desktop: image left, text right.
- Mobile: image stacks first, content second.

## Section 4: Final Healthcare Career CTA Section

### Section Goal

Close the page with the established healthcare career CTA and contact action.

### Container Hierarchy

```txt
Final Career CTA
  Career CTA Inner
    Heading widget
    Text Editor widget
    Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget

### Global Styles Needed

- Healthcare surgical team background
- Dark navy overlay: `#001932` at 0.75 opacity
- White text
- Red CTA button

### Spacing Values

- Desktop padding: 95px top/bottom
- Tablet padding: 75px top/bottom
- Mobile padding: 60px top/bottom
- Minimum height: 360px desktop, 330px tablet, 300px mobile

### Typography Specs

- CTA heading: 36px desktop, 30px tablet, 27px mobile, weight 900, line height 1.2
- CTA text: 16px desktop, 15px mobile, line height 1.65
- Button: project button lock

### Responsive Notes

- Text remains centered.
- Background image remains cover-sized and centered.

## Section 5: Map Section

### Section Goal

Show the Woodbridge location directly above the global footer.

### Container Hierarchy

```txt
Map Section
  Google Maps widget
```

### Widget List

- Google Maps widget

### Spacing Values

- Desktop map height: 420px
- Tablet map height: 320px
- Mobile map height: 260px

### Responsive Notes

- Map remains full-width.
- Scroll prevention is enabled.

## Manual Image Replacement Notes

- Hero background: replace with the exact healthcare/classroom/writing image from the screenshot or approved media library.
- Details image: replace with the approved healthcare worker in green scrubs/medication room image.
- Final CTA background: replace with the approved dark healthcare surgical team CTA image if needed.

## Button Link Notes

- Details `GET STARTED`: currently `#`
- Final CTA `CONTACT US`: currently `#`

## Elementor Compatibility Notes

- Template uses Elementor Containers and native Elementor widgets.
- Text, images, buttons, and map are editable in Elementor.
- One scoped HTML widget handles page-specific CSS for responsive grids, image crops, and shared hover states.
- No global header, footer, Site Settings, or unrelated templates are modified.

## Quality Check

- Page order is exactly: hero banner, blue intro, medication management details, final CTA, map.
- No section is flattened into a single text block.
- No legacy Elementor Sections or Columns are used.
- Button styling follows the 1st Providence button lock.
- Header and footer are excluded from the body template.
