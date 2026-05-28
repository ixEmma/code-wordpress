# 1st Providence Class Schedule Page Section Map

## Page Body Section List

1. Class Schedule Hero Banner
2. Class Schedule Table Section
3. CTA Banner Section
4. Map Section

This template is body-only. It excludes the header, logo area, navigation, footer, footer social links, legal links, copyright, and footer contact details.

## Section 1: Class Schedule Hero Banner

### Section Goal

Create the visual page opener shown in the screenshot: a full-width medical training image with dark blue overlay and centered white `CLASS SCHEDULE` title.

### Container Hierarchy

```txt
Hero Banner Container
  Hero Inner Container
    Heading widget: CLASS SCHEDULE
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
- Inner max width: 1180px
- Padding: 70px desktop, 54px tablet, 44px mobile

### Typography Specs

- Page title: 45px desktop, 38px tablet, 32px mobile
- Weight: 900
- Line height: 1.1
- Uppercase, centered, white

### Responsive Behavior

- Background image remains cover/center.
- Title remains centered on all breakpoints.
- Section compresses on mobile without including any header content.

## Section 2: Class Schedule Table Section

### Section Goal

Display the visible class schedule rows from the screenshot in a centered, clean, bordered table.

### Container Hierarchy

```txt
Schedule Section Container
  Schedule Inner Container
    Text Editor widget with editable table markup
```

### Widget List

- Text Editor widget

### Global Styles Used

- White background: `#FFFFFF`
- Header row: Healthcare Blue `#1F5F8F`
- Text: Body Dark Gray `#333333`
- Borders: light gray `#D7DEE5`
- Font family: Nunito Sans

### Spacing Values

- Section padding desktop: 58px top, 64px bottom, 20px sides
- Section padding tablet: 48px top/bottom, 20px sides
- Section padding mobile: 40px top/bottom, 16px sides
- Table max-width: 1120px

### Typography Specs

- Table header: 12px desktop, uppercase, 800, white
- Table body: 13px desktop, 12px mobile, line height 1.45, dark gray
- These are a table-specific compact exception documented here because the screenshot table is dense and would not fit cleanly at normal body size.

### Table Strategy

Elementor core/Pro does not provide a stable native table widget in the reference exports. To keep the schedule importable and editable, the generated template uses a native Text Editor widget containing semantic HTML table markup.

Editability tradeoff:

- All table text is editable inside the Elementor Text Editor widget.
- Individual cells are not separate Elementor widgets.
- The table wrapper uses inline CSS for horizontal overflow so the wide table does not break mobile layouts.

### Responsive Behavior

- Desktop: centered full table.
- Tablet/mobile: table remains readable through horizontal scroll.
- The table wrapper prevents the table from forcing page overflow.

## Section 3: CTA Banner Section

### Section Goal

Recreate the screenshot's full-width medical/surgical blue CTA banner below the table, with centered heading, supporting text, and Contact Us button.

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

- CTA heading: 34px desktop, 30px tablet, 26px mobile, weight 800, line height 1.2
- Supporting text: 16px desktop/tablet, 15px mobile, line height 1.6
- Button: 14px desktop/tablet, 13px mobile, 800, uppercase, 1.5px letter spacing

### Responsive Behavior

- Text and button remain centered.
- Background image remains cover/center.
- Button stays editable and uses locked CTA style.

## Section 4: Map Section

### Section Goal

Add the full-width map area visible above the footer in the screenshot, without including footer content.

### Container Hierarchy

```txt
Map Section Container
  Google Maps widget
```

### Widget List

- Google Maps widget

### Global Styles Used

- No typography required.
- Section uses full-width map treatment.

### Spacing Values

- No section padding.
- Map height: 430px desktop, 360px tablet, 320px mobile.

### Map Strategy

The generated JSON uses Elementor's native `google_maps` widget because the existing homepage body template already uses this widget successfully. If the target install disables the widget or requires API configuration, replace it manually with Elementor Google Maps or another approved map widget.

### Responsive Behavior

- Full-width map.
- Height reduces on tablet/mobile.
- No footer content below the map is included.

## Known Import Risks

- The requested screenshot path `elementor-outputs/screenshots/class-schedule-page-reference.png` was not present locally; the attached screenshot in the prompt was used as the visual reference.
- The schedule uses a Text Editor HTML table fallback because the inspected Elementor references did not include a native table widget.
- The table has inline CSS for table borders, spacing, and mobile horizontal scroll.
- Background image URLs are replaceable placeholders and should be replaced with approved site media.
- Google Maps widget may require Elementor/WordPress map support and may need API or widget configuration after import.
- Stable Elementor Kit global token IDs are not available, so project style values are represented directly in the generated JSON.

## Manual Replacement Steps In Elementor

1. Import `class-schedule-page-body-template.json`.
2. Confirm the template is placed between the existing site header and footer.
3. Replace the hero background image with the approved class schedule/training image.
4. Edit schedule rows inside the Text Editor table as class dates change.
5. Replace the CTA background image with the approved surgical/medical image if needed.
6. Update the Contact Us button link.
7. Confirm the Google Maps widget address and zoom.
8. Test horizontal table scrolling on mobile.
9. Regenerate Elementor CSS if imported styling appears stale.
