# 1st Providence Electrocardiogram Technician (EKG) Page Section Map

## Page Body Section List

1. Hero Banner With Title And Two Buttons
2. Blue Intro Section
3. Why Become An Electrocardiogram Technician Section
4. Comprehensive Program Overview Section
5. Blue Benefits/Icon Grid Section
6. Essential EKG Curriculum And Topics Section
7. Practical Skill Development And Outcomes Section
8. National Certification Pathways Centered Section
9. How To Register Section
10. 2026 Semester Dates Section
11. Final EKG CTA Section

This template is body-only. It excludes the global header, navigation, logo area, global footer, footer social icons, footer links, legal links, copyright, and footer contact details.

## Design Direction

Healthcare certification program page matching the supplied EKG reference: diagnostic monitor hero, Providence-blue intro and benefits band, alternating white/light gray two-column learning sections, centered certification pathway section, registration and semester details, and a final dark EKG CTA.

## Reference Observations

- The page is longer than the prior Medication Management page and relies on alternating section rhythm.
- The first viewport uses a darkened EKG monitor image with a centered title and two red buttons.
- Most content sections are clean two-column layouts with one clear image and one concise content block.
- The benefits section is the visual anchor: blue background, white text, red circular editable icons, and a thin white divider.
- The final CTA returns to EKG monitor imagery with a dark overlay and centered text.

## Class Names Used

- `provekg-page`
- `provekg-hero`
- `provekg-hero-overlay`
- `provekg-hero-inner`
- `provekg-hero-title`
- `provekg-hero-buttons`
- `provekg-button`
- `provekg-blue-intro`
- `provekg-blue-inner`
- `provekg-blue-title`
- `provekg-blue-text`
- `provekg-section`
- `provekg-section-inner`
- `provekg-two-col`
- `provekg-content`
- `provekg-image`
- `provekg-title`
- `provekg-text`
- `provekg-benefits`
- `provekg-benefits-inner`
- `provekg-benefits-title`
- `provekg-benefits-text`
- `provekg-benefits-rule`
- `provekg-icon-grid`
- `provekg-icon-item`
- `provekg-icon-circle`
- `provekg-icon`
- `provekg-icon-title`
- `provekg-icon-text`
- `provekg-centered-section`
- `provekg-register`
- `provekg-dates`
- `provekg-career-cta`
- `provekg-career-overlay`
- `provekg-career-inner`
- `provekg-career-title`
- `provekg-career-text`
- `provekg-career-button`

## Section 1: Hero Banner

### Section Goal

Introduce the EKG program immediately with diagnostic imagery and primary navigation actions.

### Container Hierarchy

```txt
EKG Hero Banner
  HTML widget: scoped page CSS
  Hero Inner
    Heading widget
    Hero Buttons
      Button widget: HOW TO REGISTER
      Button widget: GET DIRECTIONS
```

### Widget List

- HTML widget for scoped CSS
- Heading widget
- Container widget for button row
- Two Button widgets

### Global Styles Needed

- Dark navy overlay: `#001932` at 0.70 opacity
- White hero title
- Button red: `#A72D34`
- Button hover: `#8F252B`

### Spacing Values

- Desktop height: 300px
- Tablet height: 240px
- Mobile height: 200px
- Section padding: 70px desktop, 55px tablet, 44px mobile

### Typography Specs

- Hero title: 40px desktop, 34px tablet, 27px mobile, weight 900, uppercase, line height 1.15
- Buttons: project button lock

### Responsive Notes

- Buttons wrap if needed on narrow screens.
- Background remains cover-sized and centered.

## Section 2: Blue Intro Section

### Section Goal

Present the program name, location, hybrid learning promise, and first `GET STARTED` action.

### Container Hierarchy

```txt
Blue Intro Section
  Blue Intro Inner
    Heading widget
    Text Editor widget
    Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget

### Spacing Values

- Desktop padding: 60px top, 65px bottom
- Tablet padding: 50px top/bottom
- Mobile padding: 40px top/bottom
- Inner max width: 1120px

## Section 3: Why Become An EKG Technician

### Section Goal

Explain the career value and patient-care role of EKG technicians.

### Container Hierarchy

```txt
Why Become an EKG Technician
  Section Inner Two Column
    Content
      Heading widget
      Text Editor widget
      Button widget
    Image
      Image widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget
- Image widget

### Spacing Values

- Desktop padding: 75px top/bottom
- Tablet padding: 60px top/bottom
- Mobile padding: 45px top/bottom
- Two-column gap: 70px desktop, 40px tablet, 30px mobile

## Section 4: Comprehensive Program Overview

### Section Goal

Describe the sixty-hour structure, cardiac topics, and hybrid training model.

### Container Hierarchy

```txt
Comprehensive Program Overview
  Section Inner Two Column
    Image
      Image widget
    Content
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

- Light gray background: `#F1F1F1`
- Blue heading: `#004990`
- Body text: `#1F2933`

## Section 5: Blue Benefits/Icon Grid Section

### Section Goal

Show six reasons students choose 1st Providence with editable icons and concise supporting copy.

### Container Hierarchy

```txt
Why Students Choose 1st Providence
  Benefits Inner
    Heading widget
    Text Editor widget
    Divider widget
    Icon Grid
      Icon Item x6
        Icon Circle
          Icon widget
        Heading widget
        Text Editor widget
```

### Widget List

- Heading widget
- Text Editor widget
- Divider widget
- Six Icon widgets
- Six icon title Heading widgets
- Six icon Text Editor widgets

### Spacing Values

- Desktop padding: 75px top, 80px bottom
- Tablet padding: 60px top/bottom
- Mobile padding: 45px top/bottom
- Icon grid: 3 columns desktop, 2 columns tablet, 1 column mobile
- Icon circle: 74px by 74px

## Section 6: Essential EKG Curriculum And Topics

### Section Goal

Explain curriculum topics such as HIPAA, pharmacology, rhythms, artifacts, and clinical documentation.

### Container Hierarchy

```txt
Essential EKG Curriculum and Topics
  Section Inner Two Column
    Content
      Heading widget
      Text Editor widget
      Button widget
    Image
      Image widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget
- Image widget

## Section 7: Practical Skill Development And Outcomes

### Section Goal

Describe hands-on skills with EKG machines, leads, tracing, reversals, and ambulatory monitoring.

### Container Hierarchy

```txt
Practical Skill Development and Outcomes
  Section Inner Two Column
    Image
      Image widget
    Content
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

- Light gray background: `#F1F1F1`

## Section 8: National Certification Pathways

### Section Goal

Center the certification exam positioning for NHA and NAHP pathways.

### Container Hierarchy

```txt
National Certification Pathways
  Centered Inner
    Heading widget
    Text Editor widget
    Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget

### Spacing Values

- Desktop padding: 65px top/bottom
- Tablet padding: 55px top/bottom
- Mobile padding: 45px top/bottom
- Inner max width: 980px

## Section 9: How To Register

### Section Goal

Explain the registration process and small-class positioning with a three-step ordered list.

### Container Hierarchy

```txt
How to Register
  Section Inner Two Column
    Image
      Image widget
    Content
      Heading widget
      Text Editor widget with ordered list and link
      Button widget
```

### Widget List

- Image widget
- Heading widget
- Text Editor widget
- Button widget

### Button/Link Notes

- `Contact us` inline link is currently `#`.

## Section 10: 2026 Semester Dates

### Section Goal

Show course schedule structure and the three available 2026 semester date ranges.

### Container Hierarchy

```txt
2026 Semester Dates
  Section Inner Two Column
    Content
      Heading widget
      Text Editor widget with bold note and list
      Button widget
    Image
      Image widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget
- Image widget

## Section 11: Final EKG CTA

### Section Goal

Close the page with a certification-focused contact CTA over EKG imagery.

### Container Hierarchy

```txt
Final EKG CTA
  Career CTA Inner
    Heading widget
    Text Editor widget
    Button widget
```

### Widget List

- Heading widget
- Text Editor widget
- Button widget

### Spacing Values

- Desktop padding: 95px top/bottom
- Tablet padding: 75px top/bottom
- Mobile padding: 60px top/bottom
- Minimum height: 360px desktop, 330px tablet, 300px mobile

## Shared Typography Specs

- Section headings: 28px desktop, 24px mobile, weight 900, line height 1.2
- Body text: 15px, line height 1.7
- Benefits heading: 30px desktop, 26px mobile, weight 900
- Icon titles: 17px, weight 900
- Icon text: 14px, line height 1.55
- Buttons: project button lock, uppercase, 14px desktop, 13px mobile, weight 800, 1.5px letter spacing

## Manual Image Replacement Notes

- Hero background: replace with the exact EKG monitor/heart rhythm monitor image from the approved media library.
- Why Become image: replace with the nurse/patient clinical care image from the reference.
- Program Overview image: replace with the healthcare lab/training/mannequin image.
- Curriculum image: replace with the anatomy book/heart diagram/stethoscope image.
- Practical Skill image: replace with the close-up ECG electrode placement image.
- Register image: replace with the healthcare students studying/registering image.
- Dates image: replace with the online schedule/calendar/laptop image.
- Final CTA background: replace with the approved EKG waveform/monitor CTA image if different.

## Button Link Notes

- Hero `HOW TO REGISTER`: currently `#`
- Hero `GET DIRECTIONS`: currently `#`
- All `GET STARTED` buttons: currently `#`
- Register inline `Contact us`: currently `#`
- Final CTA `CONTACT US`: currently `#`

## Elementor Compatibility Notes

- Template uses Elementor Containers and native Elementor widgets.
- Text, images, buttons, icons, and section background images remain editable.
- One scoped HTML widget handles responsive grids, icon circles, image crops, and hover states.
- No global header, footer, Site Settings, or unrelated templates are modified.

## Quality Check

- Page order is exactly: hero banner, blue intro, why become section, program overview, benefits icon grid, curriculum section, practical skill section, national certification section, how to register, semester dates, final CTA.
- No section is flattened into one text block.
- No legacy Elementor Sections or Columns are used.
- The benefits area uses editable Icon widgets rather than static image icons.
