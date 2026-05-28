# 1st Providence Student Resources Page Section Map

## Page Body Section List

1. Student Resources Hero Banner
2. Resource Links Section
3. CTA Banner Section
4. Map Section

This template is body-only. It excludes the header, logo area, navigation, footer, footer social links, legal links, copyright, and footer contact details.

## Section 1: Student Resources Hero Banner

### Section Goal

Create the screenshot-style page opener with a healthcare/caregiving hand image, dark overlay, and centered white `STUDENT RESOURCES` title.

### Container Hierarchy

```txt
Hero Banner Container
  Hero Inner Container
    Heading widget: STUDENT RESOURCES
```

### Widget List

- Heading widget

### Global Styles Used

- Deep Blue overlay: `#142C3F`
- White: `#FFFFFF`
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

- Background image remains cover/center.
- Title remains centered on all breakpoints.
- No header, logo, or navigation content is included.

## Section 2: Resource Links Section

### Section Goal

Recreate the screenshot's soft gray resource area with six centered white horizontal link rows.

### Container Hierarchy

```txt
Resource Links Section
  Resource Links Inner Container
    Resource Link Row Container
      Button widget styled as link row
    Resource Link Row Container
      Button widget styled as link row
    ...
```

### Widget List

- Six Button widgets styled as white link rows

### Global Styles Used

- Soft Light Background: `#F7F9FB`
- Row background: `#FFFFFF`
- Link text: Healthcare Blue `#1F5F8F`
- Hover text: CTA Red `#A72D34`
- Font family: Nunito Sans

### Spacing Values

- Section padding desktop: 76px top, 82px bottom, 20px sides
- Section padding tablet: 62px top/bottom, 20px sides
- Section padding mobile: 48px top/bottom, 18px sides
- Inner max width: 1120px
- Row gap: 22px desktop, 16px mobile
- Row padding via button text padding: 24px top/bottom, 28px left/right

### Typography Specs

- Resource row text: 16px desktop/tablet, 15px mobile
- Weight: 800
- Text transform: uppercase
- Line height: 1.2

### Resource Link Strategy

Each resource item is represented as an editable Elementor Button widget with placeholder URL `#`. The widgets are styled to look like full-width white resource rows rather than CTA buttons.

This is the safest Elementor-importable approach for editable links:

- Button text is editable.
- Button URL is editable.
- Button color and hover color are editable.
- The row can be clicked through the button.

Limitation:

- The visual row is a button widget styled as a link row. If the site requires the entire parent container to be clickable beyond the button area, that can be adjusted manually in Elementor using container link features if supported by the installed version.

### Link Color And Hover Strategy

- Normal text color: Healthcare Blue `#1F5F8F`
- Hover text color: CTA Red `#A72D34`
- Normal background: White `#FFFFFF`
- Hover background: White `#FFFFFF`
- Row containers use subtle box shadow for the screenshot's soft card feel.

### Responsive Behavior

- Rows remain stacked on all breakpoints.
- Button alignment remains left.
- Text wraps naturally on narrow screens.

## Section 3: CTA Banner Section

### Section Goal

Recreate the full-width surgical/medical blue CTA banner with centered heading, supporting text, and Contact Us button.

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

## Section 4: Map Section

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

- Full-width map treatment
- No typography required

### Spacing Values

- No section padding.
- Map height: 430px desktop, 360px tablet, 320px mobile.

### Map Strategy

The generated JSON uses Elementor's native `google_maps` widget because existing generated templates in this project use that Elementor-compatible pattern. If the target install cannot render it, replace it manually with Elementor Google Maps or another approved map widget.

### Responsive Behavior

- Full-width map.
- Height reduces on tablet/mobile.
- No footer content is included below the map.

## Known Import Risks

- The requested screenshot path `elementor-outputs/screenshots/student-resources-page-reference.png` was not present locally; the attached screenshot in the prompt was used as the visual reference.
- Resource rows are editable Button widgets styled as link rows, not static text.
- Final real URLs are unknown, so each resource link uses `#` as a placeholder.
- Elementor Button hover style keys can vary by version; manually confirm hover text color after import.
- Background image URLs are replaceable placeholders and should be swapped with approved media-library images.
- Google Maps may require manual configuration depending on the target Elementor/WordPress setup.
- Stable Elementor Kit global token IDs are unavailable, so project style values are represented directly in JSON.

## Manual Replacement Steps In Elementor

1. Import `student-resources-page-body-template.json`.
2. Confirm it is placed between the existing site header and footer.
3. Replace the hero background image with the approved student resources/caregiving image.
4. Edit each resource Button widget and replace `#` with the final URL.
5. Confirm each resource row text, color, and hover color.
6. Replace the CTA background image if needed.
7. Update the Contact Us button link.
8. Confirm the Google Maps widget address and zoom.
9. Test mobile wrapping for the longer resource link labels.
10. Regenerate Elementor CSS if imported styles look stale.
