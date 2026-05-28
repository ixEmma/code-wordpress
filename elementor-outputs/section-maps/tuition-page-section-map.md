# 1st Providence Tuition Page Section Map

## Page Body Section List

1. Tuition Hero Banner
2. Tuition Table Section
3. Enroll Today Section
4. CTA Banner Section
5. Map Section

This template is body-only. It excludes the header, logo/navigation, footer, footer social links, legal links, copyright, and footer contact details.

## Section 1: Tuition Hero Banner

### Section Goal

Create the screenshot-style tuition opener: full-width medical training background image, dark blue overlay, and centered white `TUITION` title.

### Container Hierarchy

```txt
Tuition Hero Container
  Hero Inner Container
    Heading widget: TUITION
```

### Widget List

- Heading widget

### Global Styles Used

- Deep Blue overlay: `#142C3F`
- White text: `#FFFFFF`
- Nunito Sans project heading typography

### Spacing Values

- Desktop minimum height: 290px
- Tablet minimum height: 240px
- Mobile minimum height: 210px
- Padding: 70px desktop, 54px tablet, 44px mobile
- Inner max width: 1180px

### Typography Specs

- Page title: 45px desktop, 38px tablet, 32px mobile
- Weight: 900
- Line height: 1.1
- Uppercase, centered, white

### Responsive Behavior

- Background remains cover/center.
- Title remains centered.
- No header content is included.

## Section 2: Tuition Table Section

### Section Goal

Display the tuition/program costs from the screenshot in a centered clean table with blue header row and light borders.

### Container Hierarchy

```txt
Tuition Table Section
  Tuition Table Inner Container
    Text Editor widget with editable table markup
```

### Widget List

- Text Editor widget

### Global Styles Used

- White background: `#FFFFFF`
- Table header: Healthcare Blue `#1F5F8F`
- Body text: `#333333`
- Borders: `#D7DEE5`
- Font family: Nunito Sans

### Spacing Values

- Section padding desktop: 58px top, 70px bottom, 20px sides
- Section padding tablet: 48px top/bottom, 20px sides
- Section padding mobile: 40px top/bottom, 16px sides
- Table max-width: 980px

### Typography Specs

- Table header: 12px desktop, uppercase, 800, white
- Table body: 13px desktop, 12px mobile, line height 1.45, dark gray
- These compact table values are a documented table-specific exception because the screenshot table is dense and the project body size would not fit the layout cleanly.

### Table Strategy

The generated template uses a native Elementor Text Editor widget containing semantic HTML table markup. This is the safest importable option because the inspected reference exports do not include a native Elementor table widget.

Editability tradeoff:

- All table text is editable inside Elementor's Text Editor widget.
- Individual table cells are not separate Elementor widgets.
- Inline table styles preserve the screenshot-like table and mobile horizontal scrolling without JavaScript.

### Responsive Behavior

- Desktop: centered table.
- Tablet/mobile: horizontal scrolling prevents layout breakage.

## Section 3: Enroll Today Section

### Section Goal

Recreate the screenshot's two-column enrollment block with student image on the left and heading, policy bullets, and Enroll Now button on the right.

### Container Hierarchy

```txt
Enroll Today Section
  Enroll Inner Container
    Image Column
      Image widget
    Content Column
      Heading widget
      Text Editor widget with bullet list
      Button widget
```

### Widget List

- Image widget
- Heading widget
- Text Editor widget
- Button widget

### Global Styles Used

- White background: `#FFFFFF`
- Healthcare Blue heading: `#1F5F8F`
- Body Dark Gray: `#333333`
- CTA Red: `#A72D34`
- CTA Red Hover: `#8F252B`
- Nunito Sans typography and button lock

### Spacing Values

- Section padding desktop: 36px top, 78px bottom, 20px sides
- Section padding tablet: 36px top, 66px bottom
- Section padding mobile: 28px top, 56px bottom
- Inner max width: 980px
- Desktop column gap: 70px
- Mobile column gap: 32px

### Typography Specs

- Heading: 34px desktop, 30px tablet, 26px mobile, weight 800, line height 1.2
- Bullet body: 16px desktop/tablet, 15px mobile, line height 1.6
- Button: 14px desktop/tablet, 13px mobile, 800, uppercase, 1.5px letter spacing

### Responsive Behavior

- Desktop: two columns, image left and content right.
- Mobile: image stacks first, text second.
- Button remains editable and uses locked CTA styling.

## Section 4: CTA Banner Section

### Section Goal

Recreate the full-width surgical/medical CTA banner with centered text and Contact Us button.

### Container Hierarchy

```txt
CTA Banner Container
  CTA Inner Container
    Heading widget
    Text Editor widget
    Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget

### Global Styles Used

- Deep Blue overlay: `#142C3F`
- White text: `#FFFFFF`
- CTA Red: `#A72D34`
- CTA Red Hover: `#8F252B`
- Nunito Sans project typography and button lock

### Spacing Values

- Desktop minimum height: 420px
- Tablet minimum height: 360px
- Mobile minimum height: 330px
- Padding desktop: 92px top/bottom, 20px sides
- Padding mobile: 68px top/bottom, 20px sides
- Inner max width: 980px
- Widget gap: 18px

### Typography Specs

- Heading: 34px desktop, 30px tablet, 26px mobile, weight 800
- Supporting text: 16px desktop/tablet, 15px mobile, line height 1.6
- Button: project locked button typography

### Responsive Behavior

- Text and button stay centered.
- Background remains cover/center.

## Section 5: Map Section

### Section Goal

Add the full-width map area visible above the footer in the screenshot without including footer content.

### Container Hierarchy

```txt
Map Section Container
  Google Maps widget
```

### Widget List

- Google Maps widget

### Global Styles Used

- No typography required.
- Full-width map treatment.

### Spacing Values

- No section padding.
- Map height: 430px desktop, 360px tablet, 320px mobile.

### Map Strategy

The generated JSON uses Elementor's native `google_maps` widget because the existing homepage and class schedule body templates use this Elementor-compatible pattern. If the target install cannot render it, replace it manually with Elementor Google Maps or an approved map widget.

### Responsive Behavior

- Full-width map.
- Height reduces on tablet/mobile.
- No footer content is included below the map.

## Known Import Risks

- The requested screenshot path `elementor-outputs/screenshots/tuition-page-reference.png` was not present locally; the attached screenshot in the prompt was used as the visual reference.
- The tuition table uses a Text Editor HTML table fallback because the inspected references do not include a native table widget.
- Table styling uses inline CSS for import safety and mobile horizontal scroll.
- Background and student image URLs are placeholders and should be replaced with approved media-library images.
- Google Maps may need manual configuration depending on the target Elementor/WordPress setup.
- Stable Elementor Kit global token IDs are unavailable, so project style values are represented directly in JSON.

## Manual Replacement Steps In Elementor

1. Import `tuition-page-body-template.json`.
2. Confirm it is placed between the existing site header and footer.
3. Replace the hero background image with the approved tuition/training image.
4. Edit tuition rows inside the Text Editor table as prices change.
5. Replace the Enroll Today student image with approved media.
6. Update the Enroll Now and Contact Us button links.
7. Replace the CTA background image if needed.
8. Confirm the Google Maps widget address and zoom.
9. Test table horizontal scrolling on mobile.
10. Regenerate Elementor CSS if imported styles look stale.
