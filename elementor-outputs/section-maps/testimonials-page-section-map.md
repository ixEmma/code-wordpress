# 1st Providence Testimonials Page Section Map

## Confirmed Section Order

1. Testimonials Hero Banner
2. Testimonials Review Card Board
3. Career CTA Section
4. Map Section

This template is body-only. It excludes the global header, navigation, logo area, global footer, footer links, footer social icons, legal links, copyright, and footer contact details.

## Design Direction

Clean healthcare training trust page matching the reference screenshot: a compact image hero, a light gray review board with four visible stacked columns, a dark image CTA, and a full-width map.

## Required Page Classes

- `provx-testimonials-page`
- `provx-hero`
- `provx-hero-overlay`
- `provx-hero-title`
- `provx-review-section`
- `provx-review-board`
- `provx-review-column`
- `provx-review-card`
- `provx-review-stars`
- `provx-review-title`
- `provx-review-text`
- `provx-review-name`
- `provx-career-cta`
- `provx-career-cta-overlay`
- `provx-map-section`

## Section 1: Testimonials Hero Banner

### Section Goal

Introduce the page below the existing global header with a healthcare training image, dark navy overlay, and centered white title.

### Container Hierarchy

```txt
Testimonials Hero Banner Container
  Hero Inner Container
    Heading widget: TESTIMONIALS
```

### Widget List

- Heading widget

### Global Styles Needed

- White text: `#FFFFFF`
- Deep navy overlay: `#142C3F`
- Hero H1 typography from the project lock

### Spacing Values

- Desktop minimum height: 300px
- Tablet minimum height: 260px
- Mobile minimum height: 210px
- Desktop padding: 70px top/bottom, 20px left/right
- Tablet padding: 56px top/bottom
- Mobile padding: 44px top/bottom
- Inner width: 1180px

### Typography Specs

- Hero H1: 45px desktop, 38px tablet, 32px mobile
- Weight: 900
- Line height: 1.1
- Uppercase

### Responsive Notes

- Background image remains cover-sized and center-positioned.
- Section height compresses on mobile while keeping the title centered.

### Quality Check

- Uses an Elementor Container and Heading widget only.
- Does not include or modify the global header.

## Section 2: Testimonials Review Card Board

### Section Goal

Recreate the reference review wall with four explicit desktop columns, natural card heights, white cards, gold stars, blue headings, centered body text, and soft shadows.

### Container Hierarchy

```txt
Testimonials Review Section
  HTML widget: scoped board/card responsive CSS
  Testimonials Review Card Board Container
    Review Column 1 Container
      Review Card Container
        Heading widget: stars
        Heading widget: review title
        Text Editor widget: review body
        Text Editor widget: reviewer name
    Review Column 2 Container
      Review Card Containers
    Review Column 3 Container
      Review Card Containers
    Review Column 4 Container
      Review Card Containers
```

### Column Distribution

- Column 1: Bethlehem Gedefa, Maria Paz, Jennifer Owusu Asiedu, Ross Evadie, Charity Kyerewah, Sydney
- Column 2: Benedicta Oduro, Isatu Sesay, Deborah Dapaah, Charity Kyerewah, Niles Dental, Student Review
- Column 3: Anisa Makaran, Mariam Kella, Paulina Adu-Gyamfi, Mousupa Rahman
- Column 4: Yodit Negasi, Reyna Nieto, Abraham Azumah, Maima Kollimihn, Gabby G

### Widget List

- HTML widget for scoped CSS
- Container widgets for the review board
- Four `provx-review-column` container widgets
- Individual `provx-review-card` containers for every review
- Heading widgets for stars
- Heading widgets for card titles
- Text Editor widgets for testimonial body copy
- Text Editor widgets for reviewer names

### Global Styles Needed

- Light gray section background: `#F1F1F1`
- White card background: `#FFFFFF`
- Review title blue: `#004990`
- Main text: `#333333`
- Gold stars: `#FFC400`
- Soft card shadow: `0 12px 28px rgba(0,0,0,0.08)`
- Nunito Sans typography from the project lock

### Spacing Values

- Outer padding desktop: 70px top, 80px bottom, 20px left/right
- Outer padding tablet: 55px top, 60px bottom, 22px left/right
- Outer padding mobile: 40px top, 45px bottom, 18px left/right
- Board max width: 1180px
- Board grid gap: 24px
- Column vertical gap: 24px
- Card padding: 28px top/bottom, 24px left/right

### Typography Specs

- Review title: 21px desktop, 20px tablet, 19px mobile, line height 1.15, weight 900
- Body text: 14px desktop/tablet/mobile, line height 1.65, weight 400
- Reviewer name: 14px, weight 800
- Stars: 18px, weight 800, 2px letter spacing, gold

### Responsive Notes

- Desktop: `provx-review-board` uses CSS grid with 4 columns.
- Tablet: board becomes 2 columns at max-width 1024px.
- Mobile: board becomes 1 column at max-width 767px.
- Cards keep natural heights and are not forced equal.

### CSS Exception

Elementor Containers do not provide this exact explicit responsive review-board behavior. A scoped HTML widget adds page-specific CSS for only the `provx-*` classes above. It does not target the global header, footer, or unrelated pages.

### Quality Check

- No plain stacked testimonial text is used.
- Every review is a separate editable white card.
- Every card contains stars, title, body, and reviewer name.
- Four visible desktop column containers are present.
- New layout uses Elementor Containers, not legacy Sections or Columns.

## Section 3: Career CTA Section

### Section Goal

Prompt visitors to contact 1st Providence after reading reviews, using the same dark healthcare image CTA pattern shown in the reference.

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
- Deep navy overlay: `#003049`
- Button background: `#A72D34`
- Button hover: `#8F252B`
- Project button typography and padding lock

### Spacing Values

- Desktop minimum height: 360px
- Tablet minimum height: 330px
- Mobile minimum height: 300px
- Desktop padding: 90px top/bottom, 20px left/right
- Mobile padding: 60px top/bottom, 20px left/right
- Inner max width: 980px
- Inner gap: 18px

### Typography Specs

- CTA heading: 34px desktop, 30px tablet, 26px mobile, line height 1.2, weight 800
- Body text: 16px desktop/tablet, 15px mobile, line height 1.6
- Button text: 14px desktop/tablet, 13px mobile, uppercase, weight 800, 1.5px letter spacing

### Responsive Notes

- Text and button stay centered on all breakpoints.
- Background remains cover-sized with center positioning.

### Quality Check

- Button link is the requested editable placeholder `#`.
- Uses the established red button system.

## Section 4: Map Section

### Section Goal

Show the Woodbridge address in a full-width editable Elementor Google Maps widget.

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
- Mobile map height: 260px

### Responsive Notes

- Map remains full-width on all breakpoints.
- Scroll prevention is enabled for better mobile usability.

### Quality Check

- Address is editable in the Google Maps widget:
  `1549 Old Bridge Rd Suite 208, Woodbridge, VA 22192, USA`

## Elementor Compatibility Notes

- Template uses Elementor Containers and native Elementor widgets, with one scoped HTML widget for the responsive board CSS.
- The template is designed as a page body import and should be placed between the existing global header and footer.
- Repeated typography and button values follow the established 1st Providence project lock.
- The template does not modify Site Settings, header templates, footer templates, or unrelated pages.
