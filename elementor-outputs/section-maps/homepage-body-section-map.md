# Homepage Body Section Map

Build: `homepage-body-template.json`

Scope: homepage body only. Header, navigation, logo area, footer, footer social links, legal links, copyright, and footer contact details are excluded.

## Full Body Section List

1. Hero Section
2. Welcome Accreditation Section
3. Three Image Link Cards Section
4. Mission Section
5. Testimonials Section
6. CTA Banner Section
7. Map Section

## Global Styles Used

Visual source of truth:

- Providence Navy: `#2B254F`
- Healthcare Blue: `#1F5F8F`
- Body Dark Gray: `#333333`
- CTA Red: `#A72D34`
- CTA Red Hover: `#8F252B`
- Deep Blue: `#142C3F`
- Soft Light Background: `#F7F9FB`
- Muted Gray: `#666666`
- White: `#FFFFFF`
- Font family: `Nunito Sans`

Repeated style patterns documented for Elementor Site Settings:

- Body font: Nunito Sans, 13px to 16px, weight 400, line-height 1.55em.
- Section headings: Nunito Sans, 30px to 48px, weight 800, line-height 1.15em.
- Card headings: Nunito Sans, 20px, weight 800.
- Button typography: Nunito Sans, 12px, weight 800, uppercase.
- Primary button: CTA Red background, White text, CTA Red Hover hover background.
- Image overlay: Deep Blue or Healthcare Blue at 0.68 to 0.82 opacity.
- Section padding desktop: 66px to 92px vertical for standard sections.
- Section padding mobile: 46px to 70px vertical, 20px to 24px horizontal.
- Container max widths: 1180px hero, 1040px mission, 980px testimonials, 960px CTA.
- Card shadow: `0 12px 28px rgba(0, 0, 0, 0.12)`.

## Section Details

### 1. Hero Section

Section goal: introduce the healthcare training offer immediately after the site header with a strong image-backed hero and a red contact CTA.

Container hierarchy:

- Hero Section container
- Hero Content Inner container
- Heading widget
- Text Editor widget
- Button widget

Widget list:

- Heading: `Start Your Healthcare Career With Us`
- Text Editor: `Learn the fundamentals with experts in the field.`
- Button: `CONTACT US`

Spacing values:

- Desktop padding: `92px 0`
- Mobile padding: `70px 0`
- Content max width: `1180px`
- Content gap: `14px`

Typography specs:

- H1: Nunito Sans, 48px desktop, 34px mobile, weight 800, White.
- Supporting text: Nunito Sans, 18px, White.
- Button: 12px uppercase, weight 800.

Responsive behavior:

- Content remains left aligned.
- Hero min-height reduces from 510px desktop to 470px mobile.
- Horizontal padding increases to 24px on mobile.

### 2. Welcome Accreditation Section

Section goal: establish trust through badges, a centered welcome statement, and replaceable accreditation/logo images.

Container hierarchy:

- Welcome Accreditation Section container
- Accreditation Badge Row container
- Three Image widgets
- Heading widget
- Text Editor widget
- Accreditation Logo Row container
- Four Image widgets

Widget list:

- 7 Image widgets for badges and accreditation logos.
- Heading: `Welcome to 1ST Providence Healthcare Training LLC`
- Text Editor: centered school/training overview paragraph.

Spacing values:

- Desktop padding: `66px 20px 70px`
- Mobile padding: `46px 20px 50px`
- Badge row gap: `18px`
- Logo row gap: `28px`

Typography specs:

- Heading: Nunito Sans, 32px desktop, 25px mobile, weight 800, Healthcare Blue.
- Body: Nunito Sans, 13px, Body Dark Gray.

Responsive behavior:

- Badge and logo rows stack on mobile.
- Text remains centered.

### 3. Three Image Link Cards Section

Section goal: recreate the screenshot's three equal blue-overlay navigation tiles for major user paths.

Container hierarchy:

- Three Image Link Cards Section container
- Three Image Link Card containers
- One Heading widget inside each card

Widget list:

- Heading: `OUR PROGRAMS`
- Heading: `TUITION`
- Heading: `STUDENT RESOURCES`

Spacing values:

- Outer padding: `0`
- Card min-height: `250px`
- Card padding: `30px 20px`
- Card gap: `0`

Typography specs:

- Tile text: Nunito Sans, 20px, uppercase content, weight 800, White.

Responsive behavior:

- Desktop: three equal row cards at 33.333% width.
- Mobile: cards stack vertically at 100% width.

### 4. Mission Section

Section goal: explain the school's mission using the screenshot's image-left, text-right layout with a contact CTA.

Container hierarchy:

- Mission Section container
- Mission Inner container
- Mission Image Column container
- Image widget
- Mission Text Column container
- Heading widget
- Subheading widget
- Text Editor widget
- Button widget

Widget list:

- Image: replaceable healthcare training/lab image.
- Heading: `Our Mission`
- Heading: `Our Pledge of Quality`
- Text Editor: mission paragraph.
- Button: `CONTACT US`

Spacing values:

- Section padding: `72px 0`
- Mobile section padding: `52px 0`
- Inner max width: `1040px`
- Column gap: `42px`

Typography specs:

- Main heading: 31px desktop, 27px mobile, Healthcare Blue.
- Subheading: 15px, Body Dark Gray, weight 800.
- Body: 14px, Body Dark Gray.

Responsive behavior:

- Desktop: two columns, image 52%, text 48%.
- Mobile: columns stack with image first and text below.

### 5. Testimonials Section

Section goal: show three student quotes in a soft light gray band.

Container hierarchy:

- Testimonials Section container
- Heading widget
- Testimonials Cards Row container
- Three Testimonial Card containers
- Heading widget and Text Editor widget inside each card

Widget list:

- Heading: `What our past students are saying`
- Three red testimonial heading widgets.
- Three editable testimonial body Text Editor widgets.

Spacing values:

- Section padding: `76px 0 84px`
- Mobile padding: `54px 0 58px`
- Cards row max width: `980px`
- Card gap: `44px`
- Card padding: `28px 24px 26px`

Typography specs:

- Section heading: 30px desktop, 25px mobile, Healthcare Blue.
- Testimonial headings: 20px, CTA Red.
- Testimonial body: 13px, Body Dark Gray.

Responsive behavior:

- Desktop: three cards in a row.
- Mobile: cards stack.

### 6. CTA Banner Section

Section goal: provide a strong final enrollment prompt above the map, using the screenshot's dark blue image overlay and centered text.

Container hierarchy:

- CTA Banner Section container
- CTA Banner Inner container
- Heading widget
- Text Editor widget
- Button widget

Widget list:

- Heading: `Are You Ready to Start Your Career in Healthcare?`
- Text Editor: enrollment prompt.
- Button: `CONTACT US`

Spacing values:

- Section padding: `86px 0`
- Mobile padding: `66px 0`
- Min-height: `360px`
- Inner max width: `960px`
- Inner gap: `16px`

Typography specs:

- Heading: 30px desktop, 25px mobile, White.
- Body: 16px, White.
- Button: red primary button pattern.

Responsive behavior:

- Content remains centered.
- Background image uses cover sizing and center positioning.

### 7. Map Section

Section goal: match the screenshot's full-width map strip without adding footer content.

Container hierarchy:

- Map Section container
- Google Maps widget

Widget list:

- Google Maps widget with address: `1549 Old Bridge Rd Suite 208, Woodbridge, VA 22192, USA`

Spacing values:

- Section padding: `0`
- Map height: `430px`

Typography specs:

- No typography used in this section.

Responsive behavior:

- Full-width map remains below CTA.
- If the Google Maps widget does not render after import, replace it with Elementor's native Google Maps widget or a map image placeholder.

## Known Import Risks

- The requested file `elementor-outputs/references/global-styles-site-settings.md` was not present. The template uses the explicit global color/font values supplied in the task.
- Screenshot path had a doubled extension: `homepage-full-reference.png.png`; that file was inspected.
- Remote Unsplash image URLs are placeholders for import/editing and should be replaced with approved brand/media-library images.
- Badge and accreditation image widgets are intentionally empty so real badge/logo assets can be added from the WordPress media library.
- The map uses Elementor's native `google_maps` widget settings. Confirm widget availability after import.
- Generated `global_variables` are included for documentation/import context, but the active Elementor Kit may need manual global color/font setup.

## Manual Replacement Needed in Elementor

- Replace hero background image with the exact healthcare team image from the live/reference site.
- Replace all badge and accreditation logo image widgets.
- Replace the three tile background images with final `Our Programs`, `Tuition`, and `Student Resources` images.
- Replace mission image with the exact lab/student training image.
- Replace CTA banner background image with the exact medical/surgical background image.
- Confirm all button URLs point to the correct contact page or anchor.
- Confirm Google Maps address, zoom, and display height after import.
- Set or confirm Elementor Site Settings for Nunito Sans and the listed global colors.

