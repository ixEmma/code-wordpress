# 1st Providence Medication Aide 68 Hour Page Section Map

## Page Body Section List

1. Top Hero Intro Section
2. Red Why Become Feature Section
3. Benefits Icon Grid Section
4. How To Register Section
5. Final Career CTA Section
6. Map Section

This template is body-only. It excludes the global header, navigation, logo area, global footer, footer social icons, footer links, legal links, copyright, and footer contact details.

## Design Direction

Healthcare education program page matching the supplied Medication Aide reference: light gray split intro, dark red career value band with overlapping clinical imagery, spacious benefits grid, practical registration details, dark medical-team CTA, and editable location map.

## Reference Observations

- The page uses the existing Providence blue and dark red palette without decorative gradients or extra effects.
- The hero is compact and text-led, with the medical image supporting the program offer.
- The red feature section depends on a strong horizontal color band and vertically oversized image.
- Benefits are intentionally airy, not card-heavy, with simple editable icons and red subheads.
- Registration content is utilitarian and scannable, with image, hours, and schedule aligned in three columns.
- The final CTA follows the established dark healthcare-image banner pattern already used in other 1st Providence pages.

## Class Names Used

- `provmed68-page`
- `provmed68-hero-intro`
- `provmed68-hero-inner`
- `provmed68-hero-content`
- `provmed68-hero-title`
- `provmed68-hero-text`
- `provmed68-button-row`
- `provmed68-button`
- `provmed68-hero-image`
- `provmed68-red-feature`
- `provmed68-red-inner`
- `provmed68-red-image-wrap`
- `provmed68-red-image`
- `provmed68-red-content`
- `provmed68-red-title`
- `provmed68-red-text`
- `provmed68-benefits`
- `provmed68-benefits-inner`
- `provmed68-section-heading`
- `provmed68-heading-rule`
- `provmed68-benefit-grid`
- `provmed68-benefit-item`
- `provmed68-benefit-icon`
- `provmed68-benefit-title`
- `provmed68-benefit-text`
- `provmed68-register`
- `provmed68-register-inner`
- `provmed68-register-heading`
- `provmed68-register-rule`
- `provmed68-register-intro`
- `provmed68-register-grid`
- `provmed68-register-image`
- `provmed68-hours`
- `provmed68-schedule`
- `provmed68-list`
- `provmed68-career-cta`
- `provmed68-career-overlay`
- `provmed68-map-section`

## Section 1: Top Hero Intro Section

### Section Goal

Introduce the 68-hour Medication Aide certification, location, hybrid format, and immediate actions.

### Container Hierarchy

```txt
Medication Aide Hero Intro
  HTML widget: scoped page CSS
  Hero Inner
    Hero Content
      Heading widget
      Text Editor widget
      Button Row
        Button widget: GET STARTED
        Button widget: GET DIRECTIONS
    Hero Image
      Image widget
```

### Widget List

- HTML widget for scoped layout CSS
- Heading widget
- Text Editor widget
- Container widget for button row
- Two Button widgets
- Image widget

### Global Styles Needed

- Light gray background: `#F1F1F1`
- Providence blue: `#004990`
- Main text: `#1F2933`
- Button red: `#A72D34`
- Button hover red: `#8F252B`
- Image radius: 8px

### Spacing Values

- Desktop padding: 70px top and bottom
- Tablet padding: 55px top and bottom
- Mobile padding: 42px top, 45px bottom
- Inner max width: 1120px
- Desktop grid gap: 70px

### Typography Specs

- Hero H1: 40px desktop, 34px tablet, 30px mobile, weight 900, line height 1.1
- Body: 15px, line height 1.7
- Buttons: project button lock, 13px, uppercase, weight 800, 1.5px letter spacing

### Responsive Notes

- Desktop: two columns, copy left and image right.
- Mobile: stacks copy first and image second, with buttons centered.

## Section 2: Red Why Become Feature Section

### Section Goal

Explain the career value of becoming a Medication Aide and recreate the red-band image overlap from the reference.

### Container Hierarchy

```txt
Why Become Feature
  Red Feature Inner
    Red Feature Image Wrap
      Image widget
    Red Feature Content
      Heading widget
      Text Editor widget
      Button widget
```

### Widget List

- Image widget
- Heading widget
- Text Editor widget
- Button widget

### Global Styles Needed

- Dark red section background: `#A72D34`
- White heading/body text
- White outline button on red background

### Spacing Values

- Desktop red band uses 0 section padding with image overlap
- Tablet padding: 55px top/bottom
- Mobile padding: 45px top, 50px bottom
- Desktop image: 430px by 430px
- Desktop grid gap: 80px

### Typography Specs

- Heading: 42px desktop, 34px tablet, 30px mobile, weight 900, line height 1.15
- Body: 15px, line height 1.7

### Responsive Notes

- Desktop: image overlaps the red band vertically.
- Mobile: image stacks above the text without aggressive overlap.

## Section 3: Benefits Icon Grid Section

### Section Goal

Show six reasons students choose the program using editable icons and compact benefit copy.

### Container Hierarchy

```txt
Benefits Icon Grid
  Benefits Inner
    Heading widget
    Divider widget
    Benefit Grid
      Benefit Item containers x6
        Icon widget
        Heading widget
        Text Editor widget
```

### Widget List

- Heading widget
- Divider widget
- Six Icon widgets
- Six benefit Heading widgets
- Six Text Editor widgets

### Global Styles Needed

- Light gray background: `#F1F1F1`
- Heading blue: `#004990`
- Icon blue: `#6FA3D9`
- Benefit title red: `#A72D34`
- Rule: `rgba(0,73,144,0.25)`

### Spacing Values

- Desktop padding: 75px top, 80px bottom
- Tablet padding: 60px top/bottom
- Mobile padding: 45px top/bottom
- Desktop grid: 3 columns, 90px column gap, 80px row gap

### Typography Specs

- Section heading: 30px desktop, 28px tablet, 26px mobile, weight 900
- Benefit titles: 18px, weight 900
- Benefit body: 14px, line height 1.6

### Responsive Notes

- Desktop: 3 columns by 2 rows.
- Tablet: 2 columns.
- Mobile: 1 column, centered benefit content.

## Section 4: How To Register Section

### Section Goal

Provide enrollment instructions, program hours, and the 2026 Medication Aide schedule in a practical three-column layout.

### Container Hierarchy

```txt
How To Register
  Register Inner
    Heading widget
    Divider widget
    Text Editor widget
    Register Grid
      Image column
        Image widget
      Program Hours
        Heading widget
        Text Editor list
      Medication Aide Schedule
        Heading widget
        Text Editor list
        Button widget
```

### Widget List

- Heading widget
- Divider widget
- Text Editor widget with enrollment link placeholder
- Image widget
- Two content Heading widgets
- Two Text Editor list widgets
- Button widget

### Global Styles Needed

- White section background
- Register heading red: `#A72D34`
- Rule: `rgba(167,45,52,0.35)`
- Column headings blue: `#004990`
- Button red and hover red from project button lock

### Spacing Values

- Desktop padding: 70px top, 80px bottom
- Tablet padding: 60px top/bottom
- Mobile padding: 45px top/bottom
- Desktop grid columns: `.9fr .85fr .95fr`
- Desktop gap: 55px
- Image height: 270px desktop, 240px mobile

### Typography Specs

- Register heading: 30px desktop, 28px tablet, 26px mobile, weight 900
- Column headings: 22px desktop, 19px mobile, weight 900
- Lists: 15px, line height 1.55

### Responsive Notes

- Desktop: image, hours, and schedule in three columns.
- Tablet: grid gap tightens.
- Mobile: stacks intro, image, program hours, schedule, and button.

## Section 5: Final Career CTA Section

### Section Goal

Close the program body with a high-contrast enrollment/contact call to action.

### Container Hierarchy

```txt
Final Career CTA
  Heading widget
  Text Editor widget
  Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget

### Global Styles Needed

- Healthcare surgical team background image
- Dark navy Elementor background overlay: `#001932` at 0.75 opacity
- White text
- Red button: `#A72D34`

### Spacing Values

- Desktop padding: 95px top/bottom
- Tablet padding: 75px top/bottom
- Mobile padding: 60px top/bottom
- Desktop minimum height: 360px

### Typography Specs

- CTA heading: 38px desktop, 30px tablet, 26px mobile, weight 900
- CTA body: 16px desktop/tablet, 15px mobile
- Button: project button lock

### Responsive Notes

- Text remains centered.
- Background image remains cover-sized and centered.

## Section 6: Map Section

### Section Goal

Show the Woodbridge training location with an editable Elementor Google Maps widget.

### Container Hierarchy

```txt
Map Section
  Google Maps widget
```

### Widget List

- Google Maps widget

### Spacing Values

- Desktop map height: 420px
- Tablet map height: 360px
- Mobile map height: 260px

### Responsive Notes

- Map remains full-width.
- Scroll prevention is enabled to avoid accidental page-scroll capture.

## Manual Image Replacement Notes

- Hero image: replace with the approved close-up syringe or medication vial image with blue glove.
- Red feature image: replace with the approved nurse/medical worker holding IV or medication image.
- Register image: replace with the approved healthcare student image shown in the reference.
- Final CTA background: replace with the approved dark medical/surgical team CTA background if the media library has a better match.

## Button Link Notes

- Hero `GET STARTED`: currently `#`
- Hero `GET DIRECTIONS`: currently `#`
- Red feature `GET STARTED`: currently `#`
- Schedule `GET STARTED`: currently `#`
- Final CTA `CONTACT US`: currently `#`
- Register intro link `Register Now - 1st Providence Enrollment Form`: currently `#`

## Elementor Compatibility Notes

- Template uses Elementor Containers and native Elementor widgets.
- Icons are editable Elementor Icon widgets.
- Images are editable Elementor Image widgets or editable section background images.
- Map is an editable Elementor Google Maps widget.
- A single scoped HTML widget handles page-specific CSS for grids, image crops, red-band overlap, and responsive behavior.
- No global header, footer, Site Settings, or unrelated pages/templates are modified.

## Quality Check

- Header and footer are excluded.
- No legacy Sections or Columns are used.
- Text content matches the supplied request.
- Button styling follows the 1st Providence button lock except the red feature outline button, which is a documented section-specific exception matching the reference.
- Repeated project colors and typography follow the established 1st Providence system.
