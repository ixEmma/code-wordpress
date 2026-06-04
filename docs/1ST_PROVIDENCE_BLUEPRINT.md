# 1st Providence Elementor Rebuild Blueprint

## Scope

This repository documents the 1st Providence WordPress and Elementor rebuild. It is a public blueprint only. It intentionally excludes Elementor exports, screenshots, WordPress backups, database files, media assets, and finished client page output.

## Header Structure And Navigation Plan

The global header should remain separate from page body templates. It uses the 1st Providence logo on the left and a desktop navigation row on the right.

Navigation plan:

- Home
- About Us
- Programs
- Tuition
- Student Resources
- Class Schedule
- More
- Payment
- Contact Us

Header implementation notes:

- Use Elementor Containers, not legacy Sections or Columns.
- Keep the logo editable through an Image widget or the site logo widget.
- Keep menu items managed through WordPress menus where possible.
- Use the dark red button treatment for Payment and Contact Us.
- Do not rebuild the header inside individual page bodies.

## Footer Structure

The footer is global and should not be recreated inside page content.

Footer content plan:

- Social links: Facebook and Instagram.
- Utility links: Home, Privacy Policy, Contact, Blog.
- Contact row: phone, email, and address.
- Address: 1549 Old Bridge Rd Suite 208, Woodbridge, VA 22192.
- Copyright should use a dynamic current year where supported by Elementor or WordPress.
- Credit line can remain editable as footer text.

Footer design notes:

- Dark navy background.
- White text with small, readable link styling.
- Centered layout matching the current 1st Providence footer rhythm.

## Page Blueprints Completed

### Testimonials Page

Blueprint covers a testimonial-focused page using editable review cards, consistent spacing, and a map/footer transition. Testimonials should remain text-editable and should not be embedded as screenshots.

### Meet Our Trainers Page

Blueprint covers a trainer/profile page with editable profile content, healthcare education tone, and reusable page-body structure. Trainer images should be selected from approved media only.

### Nurse Aide Page

Blueprint covers a Nurse Aide program page with a body-only Elementor layout, program details, requirements, schedule content, career CTA, and editable image widgets.

### Medication Aide 68 Hour Page

Blueprint covers the Medication Aide 68 Hour program page with:

- Light gray split hero intro.
- Red career-value feature section.
- Benefits icon grid.
- How To Register section.
- Final healthcare CTA.
- Map section.

### Medication Management Page

Blueprint covers the Medication Management program page with:

- Image hero banner.
- Blue intro section.
- Two-column course details section.
- Final healthcare CTA.
- Map section.

### Electrocardiogram Technician Page

Blueprint covers the Electrocardiogram Technician (EKG) program page with:

- EKG monitor hero and two buttons.
- Blue intro.
- Alternating two-column education sections.
- Blue benefits icon grid.
- Centered certification pathway section.
- Registration and semester date sections.
- Final EKG CTA.

## Global Typography Rules

Use the established 1st Providence Elementor Site Settings typography system.

- Hero H1: 45px desktop, 38px tablet, 32px mobile, weight 900, line height 1.1-1.15.
- H2 section heading: 34px desktop, 30px tablet, 26px mobile, weight 800, line height 1.2.
- H3/card heading: 22px desktop, 20px tablet, 19px mobile, weight 800, line height 1.25.
- Body text: 16px desktop/tablet, 15px mobile, weight 400/500, line height 1.6-1.7.
- Hero subtitle: 24px desktop, 21px tablet, 18px mobile, weight 600/700.
- Button text: 14px desktop/tablet, 13px mobile, weight 800, uppercase.

## Global Color Rules

- Providence blue: `#004990`
- Dark red: `#A72D34`
- Button hover red: `#8F252B`
- Dark navy overlay/background: `#001932`
- Light gray: `#F1F1F1`
- Off white: `#F7F9FB`
- White: `#FFFFFF`
- Main text: `#1F2933`

## Button Rules

Use the established 1st Providence button system:

- Font family: Nunito Sans.
- Font weight: 800.
- Text transform: uppercase.
- Letter spacing: 1.5px.
- Text color: white.
- Background: `#A72D34`.
- Hover background: `#8F252B`.
- Border radius: 4-6px.
- Desktop padding: 14px top/bottom, 30px left/right.
- Mobile padding: 12px top/bottom, 24px left/right.

## Elementor Class Naming Conventions Used

Class prefixes documented during the rebuild:

- Testimonials page: `provx-*`.
- Nurse Aide page: `provcna-*`.
- Medication Aide 68 Hour page: `provmed68-*`.
- Medication Management page: `provmanage-*`.
- Electrocardiogram Technician page: `provekg-*`.

Rules:

- Use page-specific prefixes to avoid style leakage.
- Keep scoped CSS minimal and only for layout behavior Elementor cannot reliably express in import JSON.
- Do not add classes to global header/footer from page body builds.
- Keep all content editable through Elementor widgets.

## Privacy And Public Repo Rules

Do not commit:

- Elementor export JSON files.
- WordPress backups or full site copies.
- Database files.
- Screenshots or media assets.
- Client-owned finished layouts.
- Environment files.
- Archives.

Commit documentation and blueprint files only.
