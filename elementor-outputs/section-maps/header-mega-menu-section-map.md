# 1st Providence Header Mega Menu Section Map

## Header Goal

Create a separate Elementor Pro Theme Builder Header template that matches the updated screenshot reference. The header is a tall white desktop bar with a large 1st Providence logo on the left, horizontal Providence Navy navigation on the right, Programs as a hover dropdown, and Payment plus Contact Us red CTA buttons at the far right.

This remains a header-only task. Do not merge this into the homepage body template. Do not modify footer templates.

## Updated Reference Analysis

- Header background is clean white.
- Header is tall on desktop, approximately 180px to 188px in the screenshot.
- Logo is the dominant header object, left aligned, approximately 270px to 300px wide.
- Navigation sits horizontally to the right of the logo and vertically around the header centerline.
- Main menu labels are uppercase or uppercase-styled in Providence Navy.
- Home appears visually muted/gray compared with the blue links.
- About Us, Programs, and More show dropdown indicators.
- Programs dropdown is open in the screenshot and appears as a tall light-gray panel under Programs.
- Dropdown text is Providence Navy, uppercase, left aligned, and generously spaced.
- Payment and Contact Us are compact CTA Red buttons with white uppercase text.
- The hero begins directly below the white header; this template must not include hero content.

## Header Container Hierarchy

```txt
Header Outer Container
  Header Inner Container
    Logo Container
      Site Logo widget
    Right Header Container
      Navigation Container
        Elementor Pro Nav Menu widget
      CTA Container
        Button widget: Payment
        Button widget: Contact Us
```

Container notes:

- Use Elementor Containers only.
- Outer container is full width with white background.
- Inner container uses wide boxed width around 1700px to match the screenshot spacing.
- Right Header Container groups nav and CTA buttons so they align as one right-side cluster.
- Keep the hierarchy shallow and editable.

## Widget List

- Site Logo widget for replaceable site logo.
- Elementor Pro Nav Menu widget connected to a WordPress menu.
- Button widget for Payment.
- Button widget for Contact Us.

## Recommended Menu Widget Approach

Preferred option when confirmed available:

- Use Elementor Pro Menu widget with native mega menu capability.
- Build the Programs panel as an editable Elementor mega menu panel.
- This gives the closest long-term editing experience for a true mega menu.

Fallback option used in the generated JSON:

- Use Elementor Pro Nav Menu widget connected to a WordPress menu.
- Configure Programs as a parent item with child menu items in Appearance > Menus.
- This preserves menu editability and import compatibility.
- The dropdown becomes a styled vertical list, matching the screenshot's simple panel more closely than a complex multi-column mega menu.

## Mega Menu Editability Strategy

The menu must remain editable. Do not convert the nav into static Heading or Text widgets.

For the Nav Menu fallback, create or update the assigned WordPress menu with Programs as a parent item and these child items:

- Nurse Aide
- Medication Aide 68 Hour
- Medication Management
- Electrocardiogram Technician (EKG)
- Personal Care Aide (PCA)
- Clinical Medical Assistant (CMA)
- Phlebotomy Technician Certificate
- Basic Life Support Provider
- Heart Saver FA CPR/AED
- AHA HeartCode

The screenshot shows these as one vertical dropdown panel, so the fallback list is acceptable and safer than a hardcoded pseudo-mega-menu.

## Desktop Layout

- Header height target: 184px.
- Outer background: #FFFFFF.
- Inner max width: 1700px.
- Desktop side padding: 60px.
- Logo width target: 290px.
- Logo container width: about 28%.
- Right header cluster width: about 72%.
- Right cluster direction: row.
- Navigation takes the remaining space and aligns right.
- CTA container stays fixed at the far right with a 20px gap.
- Main menu text:
  - Font family: Nunito Sans.
  - Weight: 700.
  - Size: 16px.
  - Transform: uppercase.
  - Color: Providence Navy, represented as #003F7F in this header reference.
- Dropdown panel:
  - Background: #F2F2F2.
  - Width target: about 315px.
  - Text color: Providence Navy.
  - Item padding: about 12px top/bottom and 22px left/right.
  - No decorative shadow needed; the screenshot reads flat and clean.
- CTA buttons follow the locked project button system:
  - Nunito Sans.
  - 14px desktop.
  - 800 weight.
  - Uppercase.
  - 1.5px letter spacing.
  - White text.
  - #A72D34 background.
  - #8F252B hover background.
  - 4px radius.
  - 14px vertical and 30px horizontal padding.

The menu size is a header-specific visual match to the screenshot and should be re-linked to the site's menu/body global typography where possible after import.

## Tablet Layout

- Header height target: 96px.
- Logo width target: 210px.
- Navigation collapses at tablet breakpoint using the Elementor Nav Menu toggle.
- Payment and Contact Us remain visible on tablet only if they fit cleanly.
- If crowded, add Payment and Contact Us as WordPress menu items for tablet/mobile and hide the CTA container at tablet.
- Tablet side padding: 28px.

## Mobile Layout

- Header height target: 78px.
- Logo left, burger toggle right.
- Logo width target: 165px.
- Hide separate CTA button container on mobile.
- Put Payment and Contact Us in the mobile WordPress menu if they need to remain visible.
- Mobile dropdown opens below the white header.
- Mobile button text, if separate buttons are later enabled, must use the locked 13px project button value.

## Global Styles Used

Use only project-specific 1st Providence values:

- White: #FFFFFF.
- Providence Navy: #003F7F for header/menu text to match the screenshot.
- Muted Home text: #7E858D.
- Dropdown background: #F2F2F2.
- CTA Red: #A72D34.
- CTA Red Hover: #8F252B.
- Button font: Nunito Sans, 800, uppercase, 1.5px letter spacing.
- Button radius: 4px.

After import, link colors and typography back to Elementor Site Settings if the target kit exposes matching global tokens.

## Manual Steps Required Inside WordPress/Elementor

1. Go to WordPress Dashboard > Appearance > Menus and create or update the main menu if using Nav Menu.
2. Add or confirm menu items: Home, About Us, Programs, Tuition, Student Resources, Class Schedule, More.
3. Add Programs child items from the program list above.
4. Add dropdown children for About Us and More if those dropdowns are required.
5. Or, if the newer Elementor Pro Menu/Mega Menu widget is available, replace the Nav Menu widget and edit the menu directly in Elementor.
6. Import `header-mega-menu-template.json`.
7. Assign it in Elementor Theme Builder as the Header.
8. Set display conditions, usually Entire Site.
9. Replace or confirm the Site Logo.
10. Update Payment and Contact Us button links.
11. Test desktop hover dropdown for Programs.
12. Test tablet and mobile menu behavior.

## Known Import Risks

- Elementor Pro is required for Theme Builder Header and Nav Menu widgets.
- The exact WordPress menu slug or ID may differ from `main-menu`; select the correct menu after import.
- Elementor import may not preserve every Nav Menu style control because Nav Menu setting keys vary across Elementor Pro versions.
- The newer Elementor Pro Menu/Mega Menu widget is not used directly in the JSON because its import structure depends on the installed Elementor version.
- Theme Builder display conditions must be assigned manually.
- Header dropdown position may need small visual adjustment after import depending on theme CSS and Elementor breakpoint settings.

## Quality Check

- Separate header template only.
- No homepage body content included.
- No footer content included.
- Uses Elementor Containers, not legacy sections or columns.
- Logo remains replaceable through Site Logo widget.
- Buttons remain editable Button widgets.
- Menu remains editable through WordPress/Elementor.
- Programs dropdown strategy is documented.
