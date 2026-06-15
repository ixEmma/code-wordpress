# 1st Providence Meet Our Trainers Page Section Map

## Page Body Section List

1. Meet Our Trainers Hero Banner
2. Blue Intro Section
3. Trainer Cards Section
4. Career CTA Section
5. Map Section

This template is body-only. It excludes the global header, navigation, logo area, global footer, footer social icons, footer links, legal links, copyright, and footer contact details.

## Design Direction

Healthcare education and trainer credibility page. The layout follows the reference: full-width dark image hero, centered blue intro block, two white trainer biography cards on a light gray field, reused dark image CTA, and a full-width map.

## Class Names Used

- `provtrain-page`
- `provtrain-hero`
- `provtrain-hero-overlay`
- `provtrain-hero-title`
- `provtrain-intro`
- `provtrain-intro-inner`
- `provtrain-intro-title`
- `provtrain-intro-text`
- `provtrain-card-section`
- `provtrain-card-grid`
- `provtrain-card`
- `provtrain-photo`
- `provtrain-name`
- `provtrain-role`
- `provtrain-bio`
- `provtrain-cta`
- `provtrain-cta-overlay`
- `provtrain-cta-title`
- `provtrain-cta-text`
- `provtrain-cta-button`
- `provtrain-map`

## Section 1: Meet Our Trainers Hero Banner

### Section Goal

Introduce the page below the existing global header with a healthcare support image and centered white uppercase page title.

### Container Hierarchy

```txt
Meet Our Trainers Hero Banner
  Hero Inner Container
    Heading widget: MEET OUR TRAINERS
```

### Widget List

- Heading widget

### Global Styles Needed

- White text: `#FFFFFF`
- Dark navy overlay: `#142C3F`
- Hero H1 typography from the project lock

### Spacing Values

- Desktop minimum height: 300px
- Tablet minimum height: 240px
- Mobile minimum height: 190px
- Desktop padding: 70px top/bottom, 20px left/right
- Tablet padding: 54px top/bottom
- Mobile padding: 42px top/bottom
- Inner max width: 1180px

### Typography Specs

- Hero title: 45px desktop, 38px tablet, 32px mobile
- Weight: 900
- Line height: 1.1
- Uppercase, centered, white

### Responsive Notes

- Background image is cover-sized and center-positioned.
- Title stays centered vertically and horizontally.

### Quality Check

- Uses Elementor Container and Heading widgets.
- Does not include or modify the global header.

## Section 2: Blue Intro Section

### Section Goal

Explain why trainer quality matters and establish the credibility of the training team before showing individual trainers.

### Container Hierarchy

```txt
Blue Intro Section
  HTML widget: scoped page CSS
  Intro Inner Container
    Heading widget
    Text Editor widget with three paragraphs
```

### Widget List

- HTML widget for scoped CSS
- Heading widget
- Text Editor widget

### Global Styles Needed

- Providence blue: `#004990`
- White text: `#FFFFFF`
- H2 typography from the project lock
- Body typography from the project lock

### Spacing Values

- Desktop padding: 70px top/bottom, 20px left/right
- Tablet padding: 55px top/bottom, 22px left/right
- Mobile padding: 40px top/bottom, 18px left/right
- Inner max width: 1120px
- Inner content gap: 22px

### Typography Specs

- Intro heading: 34px desktop, 30px tablet, 26px mobile, line height 1.2, weight 800
- Intro paragraphs: 16px desktop/tablet, 15px mobile, line height 1.7

### Responsive Notes

- Text remains centered on every breakpoint.
- Paragraph width is constrained by the 1120px inner container.

### Quality Check

- All intro copy is editable in Elementor.
- Section uses the requested `provtrain-intro` and `provtrain-intro-inner` classes.

## Section 3: Trainer Cards Section

### Section Goal

Show Emelia Korkor and Leticia Kusi in two separate editable white trainer cards, side by side on desktop and stacked on mobile.

### Container Hierarchy

```txt
Trainer Cards Section
  Trainer Card Grid Container
    Trainer Card - Emelia Korkor
      Image widget
      Heading widget: name
      Text Editor widget: role lines
      Text Editor widget: bio
    Trainer Card - Leticia Kusi
      Image widget
      Heading widget: name
      Text Editor widget: role
      Text Editor widget: bio
```

### Widget List

- Container widgets
- Image widgets
- Heading widgets
- Text Editor widgets

### Global Styles Needed

- Light gray background: `#F1F1F1`
- White card background: `#FFFFFF`
- Trainer name blue: `#004990`
- Main text: `#333333`
- Soft card shadow: `0 12px 28px rgba(0,0,0,0.08)`

### Spacing Values

- Desktop section padding: 70px top, 90px bottom, 20px left/right
- Tablet section padding: 60px top, 70px bottom, 22px left/right
- Mobile section padding: 45px top, 55px bottom, 18px left/right
- Grid max width: 1120px
- Desktop grid gap: 40px
- Mobile grid gap: 30px
- Card padding desktop: 45px top/bottom, 38px left/right
- Card padding mobile: 35px top/bottom, 24px left/right

### Typography Specs

- Trainer name: 20px desktop, 19px mobile, line height 1.2, weight 900, uppercase
- Role: 14px, italic, line height 1.5
- Bio: 14px, line height 1.7

### Responsive Notes

- Desktop: 2-column CSS grid.
- Mobile: 1-column grid at max-width 767px.
- Cards align to the top and keep natural heights.
- Images are 165px square desktop and 145px square mobile with object-fit cover.

### CSS Exception

Elementor can handle much of this with containers, but scoped CSS is used to enforce the exact two-column grid, top alignment, card shadow, and square image crop. CSS only targets `provtrain-*` classes.

### Quality Check

- Trainers are not plain text.
- Each trainer is inside a separate white card.
- Images, names, roles, and bios are editable Elementor widgets.

## Section 4: Career CTA Section

### Section Goal

Use the same conversion CTA style from the Testimonials page to encourage contact after the trainer bios.

### Container Hierarchy

```txt
Career CTA Section
  CTA Inner Container
    Heading widget
    Text Editor widget
    Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget

### Global Styles Needed

- White text: `#FFFFFF`
- Dark navy overlay: `#003049`
- Button background: `#A72D34`
- Button hover: `#8F252B`
- Project button typography and padding lock

### Spacing Values

- Desktop minimum height: 390px
- Tablet minimum height: 350px
- Mobile minimum height: 320px
- Desktop padding: 95px top/bottom, 20px left/right
- Mobile padding: 65px top/bottom, 20px left/right
- Inner max width: 980px
- Inner gap: 18px

### Typography Specs

- CTA heading: 34px desktop, 30px tablet, 26px mobile, line height 1.2, weight 800
- CTA body: 16px desktop/tablet, 15px mobile, line height 1.6
- CTA button: 14px desktop/tablet, 13px mobile, uppercase, weight 800, 1.5px letter spacing

### Responsive Notes

- Text and button stay centered.
- Background image remains cover-sized.

### Quality Check

- Button link is editable and currently set to `#`.
- Uses the established 1st Providence red button style.

## Section 5: Map Section

### Section Goal

Show the Woodbridge location in a full-width editable Elementor Google Maps widget.

### Container Hierarchy

```txt
Map Section
  Google Maps widget
```

### Widget List

- Google Maps widget

### Spacing Values

- Section padding: 0
- Desktop map height: 340px
- Tablet map height: 310px
- Mobile map height: 260px

### Responsive Notes

- Map remains full-width.
- Scroll prevention is enabled for better mobile usability.

### Quality Check

- Address is editable in the Google Maps widget:
  `1549 Old Bridge Rd Suite 208, Woodbridge, VA 22192, USA`

## Manual Replacement Notes

- Hero image is a healthcare support placeholder and should be replaced with the exact caregiver/gloved-hands image from the live site or approved media library.
- Emelia Korkor image is a placeholder portrait and should be replaced with her actual trainer photo.
- Leticia Kusi image is a placeholder portrait and should be replaced with her actual trainer photo.
- CTA image uses the same healthcare team placeholder style as the Testimonials page and can be replaced with the approved site CTA image.
- CTA button link is currently `#` and should be updated to the real Contact page URL when ready.

## Elementor Compatibility Notes

- Template uses Elementor Containers and native Elementor widgets, with one scoped HTML widget for grid/card/image CSS.
- The template is designed as a page body import and should be placed between the existing global header and footer.
- Repeated typography and button values follow the established 1st Providence project lock.
- The template does not modify Site Settings, header templates, footer templates, or unrelated pages.
