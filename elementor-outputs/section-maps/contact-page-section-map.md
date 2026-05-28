# 1st Providence Contact Page Section Map

## Page Body Section List

1. Page Title Banner
2. Contact Information + Form
3. Accreditation Badge Row

This template is body-only. It excludes the header, navigation, logo area, footer, footer social links, legal links, copyright, and footer contact details.

## Section 1: Page Title Banner

### Section Goal

Provide a strong page introduction immediately below the existing site header, matching the screenshot's deep blue banner with centered white `CONTACT US` title.

### Container Hierarchy

```txt
Page Title Banner Container
  Title Inner Container
    Heading widget: CONTACT US
```

### Widget List

- Heading widget

### Global Styles Used

- Deep Providence Navy / Deep Blue: `#003F7F`
- White text: `#FFFFFF`
- Hero-style page title typography from the project lock

### Spacing Values

- Desktop padding: 62px top, 62px bottom, 20px left/right
- Tablet padding: 54px top/bottom
- Mobile padding: 44px top/bottom
- Inner width: 1180px

### Typography Specs

- Heading: 45px desktop, 38px tablet, 32px mobile
- Weight: 900
- Line height: 1.1
- Uppercase text

### Responsive Behavior

- Remains centered on all breakpoints.
- Banner height compresses slightly on mobile while keeping the title readable.

## Section 2: Contact Information + Form

### Section Goal

Recreate the main white contact area from the screenshot with contact details on the left and a clean editable form on the right.

### Container Hierarchy

```txt
Contact Main Container
  Contact Inner Container
    Contact Info Column
      Heading widget: Get In Touch
      Text Editor widget: intro paragraph
      Text Editor widget: phone/email/hours/address
    Form Column
      Elementor Pro Form widget
```

### Widget List

- Heading widget
- Text Editor widget
- Elementor Pro Form widget

### Global Styles Used

- White background: `#FFFFFF`
- Providence Navy heading: `#003F7F`
- Main text: `#333333`
- Link/CTA Red: `#A72D34`
- Field border: `#D7DEE5`
- Button background: `#A72D34`
- Button hover: `#8F252B`
- Nunito Sans typography from the project lock

### Spacing Values

- Outer padding desktop: 92px top, 28px bottom, 20px left/right
- Outer padding tablet: 72px top, 24px bottom, 24px left/right
- Outer padding mobile: 52px top, 20px bottom, 20px left/right
- Inner max width: 1120px
- Desktop column gap: 120px
- Tablet column gap: 60px
- Contact info internal gap: 16px
- Form row gap: 16px

### Typography Specs

- Section heading: 34px desktop, 30px tablet, 26px mobile, line height 1.2, weight 800
- Body text: 16px desktop/tablet, 15px mobile, line height 1.65, weight 400
- Form labels: 16px desktop/tablet, 15px mobile, line height 1.4, weight 500
- Submit button: 14px desktop/tablet, 13px mobile, line height 1.0, weight 800, uppercase, 1.5px letter spacing

### Form Widget Strategy

The generated JSON uses the Elementor Pro `form` widget so form fields remain editable in Elementor.

Fields:

- Name, required text field
- Email, required email field
- Phone, tel field
- Which program are you interested in?, select field with `Please select value` placeholder
- How can we help?, textarea
- May we add you to our mailing list?, required select field with `-Select-` placeholder

Program options are included in the select field to make the form useful after import. They can be edited in Elementor.

### Responsive Behavior

- Desktop: two-column layout, contact info left and form right.
- Tablet: still two columns if space allows, with reduced gap.
- Mobile: columns stack, contact info first, form second.
- Form fields stay full width.

## Section 3: Accreditation Badge Row

### Section Goal

Place the three replaceable badge images centered below the contact section, matching the screenshot's row of accreditation/provider badges.

### Container Hierarchy

```txt
Badge Row Section
  Badge Row Inner Container
    Image widget: badge 1
    Image widget: badge 2
    Image widget: badge 3
```

### Widget List

- Three Image widgets

### Global Styles Used

- White background: `#FFFFFF`
- Image widgets remain replaceable through Elementor media controls

### Spacing Values

- Section padding desktop: 36px top, 104px bottom, 20px left/right
- Section padding tablet: 32px top, 80px bottom
- Section padding mobile: 28px top, 64px bottom
- Badge row max width: 560px
- Badge gap: 36px desktop, 24px mobile
- Badge image width target: 148px desktop, 132px mobile

### Typography Specs

No typography required in this section.

### Responsive Behavior

- Desktop: three centered badges in a row.
- Tablet: three centered badges with reduced width/gap.
- Mobile: badges wrap or stack cleanly with centered alignment.

## Known Import Risks

- Elementor Pro is required for the Form widget.
- If Elementor Pro is not active, the form widget may fail to render and should be replaced manually with an available form widget.
- The requested file `elementor-outputs/screenshots/contact-page-reference.png` was not present locally; the attached screenshot in the prompt was used as the visual reference.
- Badge images are replaceable placeholders with empty media URLs and must be replaced after import.
- Form email actions, recipients, reCAPTCHA, anti-spam, and confirmation behavior must be configured inside Elementor after import.
- Generated JSON references explicit style values because stable active-kit global IDs are not available from the reference files.

## Manual Replacement Steps In Elementor

1. Import `contact-page-body-template.json`.
2. Confirm the page uses the existing site header and footer outside this body template.
3. Replace the three badge Image widgets with the correct 1st Providence badge assets.
4. Open the Form widget and configure form Actions After Submit.
5. Set recipient email, subject, reply-to, and success/error messages.
6. Add reCAPTCHA or other anti-spam settings if required.
7. Confirm all field labels, dropdown options, and required flags.
8. Test desktop, tablet, and mobile spacing.
9. Regenerate Elementor CSS if the imported styling appears stale.
