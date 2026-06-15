# Basic Life Support Provider Program Page Blueprint

## Scope

Build the `Basic Life Support Provider` page body in Elementor. Do not edit, duplicate, or recreate the global header or footer. Use Elementor Containers and native widgets so all content remains editable.

This repository is documentation-only. The production Elementor page, media selections, and export files must remain in private project storage.

## Design System

- Font: Nunito Sans from Elementor Site Settings.
- Providence blue: `#004990`.
- Dark red: `#A72D34`.
- Button hover red: `#8F252B`.
- Dark navy: `#001932`.
- Light gray: `#F1F1F1`.
- Off white: `#F7F9FB`.
- Main text: `#1F2933`.
- Standard content width: `1120px`.
- Buttons: uppercase, white, 800 weight, 1.5px letter spacing, 4-6px radius.

Do not change global Elementor Site Settings. Use the existing global typography and button styles first.

## Page Order

1. Hero intro
2. Certification badges
3. Why Become a Basic Life Support Provider feature
4. Benefits icon grid
5. Recommended for healthcare professionals
6. BLS Provider Class
7. BLS Provider Renewal
8. How to Register
9. Healthcare career CTA
10. Map

## Class Names

Use only these page-specific classes:

```txt
provbls-page
provbls-hero-intro
provbls-hero-inner
provbls-hero-content
provbls-hero-title
provbls-hero-text
provbls-button-row
provbls-button
provbls-hero-image
provbls-badges
provbls-badges-inner
provbls-badge-item
provbls-red-feature
provbls-red-inner
provbls-red-image
provbls-red-content
provbls-red-title
provbls-red-text
provbls-benefits
provbls-benefits-inner
provbls-section-heading
provbls-heading-rule
provbls-benefit-grid
provbls-benefit-item
provbls-benefit-icon
provbls-benefit-title
provbls-benefit-text
provbls-recommend
provbls-class-section
provbls-class-inner
provbls-class-heading
provbls-class-rule
provbls-class-intro
provbls-class-grid
provbls-class-image
provbls-class-details
provbls-class-schedule
provbls-list
provbls-register-red
provbls-register-inner
provbls-register-image
provbls-register-content
provbls-register-title
provbls-register-text
provbls-career-cta
provbls-career-overlay
provbls-career-inner
provbls-career-title
provbls-career-text
provbls-career-button
provbls-map-section
```

## 1. Hero Intro

### Container Hierarchy

```txt
Page Wrapper: provbls-page
  Hero: provbls-hero-intro
    Inner: provbls-hero-inner
      Content: provbls-hero-content
        Heading widget: provbls-hero-title
        Text Editor widget: provbls-hero-text
        Button Row: provbls-button-row
          Button widget: provbls-button
          Button widget: provbls-button
      Image widget: provbls-hero-image
```

Heading:

```txt
Basic Life Support Provider Certification in Woodbridge, Virginia
```

Body:

```txt
Get high-quality CPR and Basic Life Support training in Woodbridge, Virginia, with 1st Providence Healthcare Training. Our BLS Provider course prepares healthcare professionals and students to respond confidently to cardiac and respiratory emergencies using American Heart Association standards.
```

Buttons: `GET STARTED` and `GET DIRECTIONS`, both linked to `#`.

Use a CPR training or chest-compressions image. Desktop uses two columns, approximately `1.35fr 0.85fr`, with a 70px gap. Use light gray background, 70px vertical desktop padding, and an image near 300px high with cover cropping. Stack content before image on mobile.

## 2. Certification Badges

### Container Hierarchy

```txt
Badges Section: provbls-badges
  Inner: provbls-badges-inner
    Image widget: provbls-badge-item
    Image widget: provbls-badge-item
    Image widget: provbls-badge-item
```

Use three editable image widgets for:

- Instructor-certified badge.
- Active contributor badge.
- American Heart Association/BLS-style badge.

Use a white background, 45px vertical desktop padding, centered wrapping layout, and badge widths near 160px. Label placeholders clearly for replacement if approved artwork is unavailable.

## 3. Red BLS Feature

### Container Hierarchy

```txt
Feature Section: provbls-red-feature
  Inner: provbls-red-inner
    Image widget: provbls-red-image
    Content: provbls-red-content
      Heading widget: provbls-red-title
      Text Editor widget: provbls-red-text
      Button widget: provbls-button
```

Heading:

```txt
Why Become a Basic Life Support Provider?
```

Body:

```txt
Basic Life Support certification is essential for healthcare workers, caregivers, and anyone responsible for emergency response. This training helps you recognize life-threatening emergencies, give high-quality chest compressions, deliver appropriate ventilations, and use an AED quickly and effectively.
```

Button: `GET STARTED`, linked to `#`.

Use dark red background and white text. Place an editable first-aid kit, stethoscope, or emergency supplies image on the left. Use a two-column layout with 70px gap, 75px vertical padding, and an image near 430 by 360px. Stack on mobile.

## 4. Benefits Icon Grid

### Container Hierarchy

```txt
Benefits Section: provbls-benefits
  Inner: provbls-benefits-inner
    Heading widget: provbls-section-heading
    Grid: provbls-benefit-grid
      Benefit Container x6: provbls-benefit-item
        Icon widget: provbls-benefit-icon
        Heading widget: provbls-benefit-title
        Text Editor widget: provbls-benefit-text
```

Section heading: `Why Students Choose 1st Providence`.

| Title | Text |
| --- | --- |
| Expert Instructors | Learn from qualified healthcare professionals with real-world emergency care experience. |
| Flexible Learning | Attend a class schedule designed to support students, workers, and healthcare teams. |
| AHA Certification | Earn certification aligned with American Heart Association standards. |
| Modern Facilities | Practice with quality training equipment in a professional learning environment. |
| Career Support | Build a required healthcare skill that supports employment and clinical readiness. |
| Affordable Excellence | Receive reliable instruction at a practical cost for healthcare training. |

Use editable Elementor Icon widgets in Providence blue. Use three columns desktop, two tablet, and one mobile. Titles are dark red; body text is dark gray. Use light gray background and 75-80px vertical desktop padding.

## 5. Recommended Section

### Container Hierarchy

```txt
Recommended Section: provbls-recommend
  Inner: provbls-benefits-inner
    Heading widget: provbls-section-heading
    Divider widget or container: provbls-heading-rule
    Text Editor widget
```

Heading:

```txt
Recommended For Anyone In The Healthcare Profession
```

Body:

```txt
Basic Life Support training is recommended for healthcare providers, nursing students, nurse aides, caregivers, medical assistants, and anyone who may need to respond during a cardiac or breathing emergency. This training gives students the confidence and practical skills needed to act quickly and safely.
```

Use a white background and 60px vertical desktop padding. Heading and optional thin rule are dark red.

## 6. BLS Provider Class

### Container Hierarchy

```txt
Class Section: provbls-class-section
  Inner: provbls-class-inner
    Heading widget: provbls-class-heading
    Divider: provbls-class-rule
    Text Editor widget: provbls-class-intro
    Grid: provbls-class-grid
      Image widget: provbls-class-image
      Details: provbls-class-details
        Heading widget
        Text Editor widget
      Schedule: provbls-class-schedule
        Heading widget
        Text Editor widget: provbls-list
        Button widget: provbls-button
```

Heading: `BLS Provider Class`.

Intro:

```txt
This course is for healthcare providers who need Basic Life Support training for clinical, workplace, or certification requirements.

Price: $95

American Heart Association
Same day certification available
```

Program Details heading: `Program Details:`

```txt
The BLS Provider course teaches students how to recognize life-threatening emergencies, provide high-quality chest compressions, give appropriate ventilations, and provide early use of an AED. Students will practice CPR for adults, children, and infants while learning team-based emergency response skills.

This course includes hands-on practice, instructor guidance, and skills testing. Students who successfully complete the course receive certification according to American Heart Association standards.
```

Schedule heading: `BLS Provider Class`

```txt
June 1 at 10:30 am
June 8 at 10:30 am
June 15 at 10:30 am
June 22 at 10:30 am
June 29 at 10:30 am
June 30 at 10:30 am
```

Button: `GET STARTED`, linked to `#`.

Use light gray background, 75px top and 85px bottom padding, and three columns for image/details/schedule. Use an editable CPR mannequin training image near 300 by 270px. Stack all columns on mobile.

## 7. BLS Provider Renewal

Use the same container hierarchy and classes as the provider class section. Set the section background to white.

Heading: `BLS Provider (Renewal)`.

Intro:

```txt
This class is designed for students and healthcare professionals who already have a current or recently expired BLS certification and need renewal.

Price: $85

American Heart Association
Same day certification available
```

Program Details heading: `Program Details:`

```txt
The BLS Provider Renewal course reviews key Basic Life Support skills for students who need to renew their certification. Students will review CPR techniques, AED use, rescue breathing, and emergency response steps for adults, children, and infants.

This renewal course includes skills practice and competency review. Students who meet course requirements receive updated certification according to American Heart Association standards.
```

Schedule heading: `BLS Provider Renewal`. Use the same six June dates as the provider class. Button: `GET STARTED`, linked to `#`.

Use an editable healthcare worker or nurse portrait near 300 by 270px.

## 8. How to Register

### Container Hierarchy

```txt
Registration Section: provbls-register-red
  Inner: provbls-register-inner
    Image widget: provbls-register-image
    Content: provbls-register-content
      Heading widget: provbls-register-title
      Text Editor widget: provbls-register-text
      Button widget: provbls-button
```

Heading: `How to Register`.

Body:

```txt
Registering for the Basic Life Support Provider class is simple. Choose the class date that works best for you, complete the enrollment form, and contact the school if you need help confirming your seat.
```

Steps:

```txt
1. Choose your preferred class date.
2. Complete the online enrollment form.
3. Submit your payment or contact the office for payment support.
4. Receive confirmation and attend your scheduled class.
```

Button: `GET STARTED`, linked to `#`.

Use a dark red background, white text, and an editable healthcare student or nurse image on the left near 430 by 360px. Use 75-80px vertical desktop padding and stack on mobile.

## 9. Healthcare Career CTA

### Container Hierarchy

```txt
CTA Section: provbls-career-cta
  Overlay: provbls-career-overlay
    Inner: provbls-career-inner
      Heading widget: provbls-career-title
      Text Editor widget: provbls-career-text
      Button widget: provbls-career-button
```

Heading:

```txt
Are You Ready to Start Your Career in Healthcare?
```

Body:

```txt
We're here to help you take the next step! Contact us today to enroll in our high-quality training programs today.
```

Button: `CONTACT US`, linked to `#`.

Reuse the approved healthcare surgical/medical team background. Apply a dark navy overlay near `rgba(0, 25, 50, 0.75)`. Center all content and use 95px vertical desktop padding.

## 10. Map

### Container Hierarchy

```txt
Map Section: provbls-map-section
  Google Maps widget
```

Address:

```txt
1549 Old Bridge Rd Suite 208
Woodbridge, VA 22192
```

Use the native Elementor Google Maps widget. Set the full-width map to 360-420px desktop, 320px tablet, and 260px mobile. It must sit directly above the global footer.

## Scoped CSS

Prefer Elementor controls. Add only the following page-scoped behavior where controls are insufficient:

```css
.provbls-page { overflow-x: hidden; }

.provbls-hero-inner {
  display: grid;
  grid-template-columns: 1.35fr 0.85fr;
  gap: 70px;
  align-items: center;
}

.provbls-badges-inner {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 45px;
  flex-wrap: wrap;
}

.provbls-red-inner,
.provbls-register-inner {
  display: grid;
  grid-template-columns: 0.95fr 1.05fr;
  gap: 70px;
  align-items: center;
}

.provbls-benefit-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  column-gap: 90px;
  row-gap: 80px;
}

.provbls-class-grid {
  display: grid;
  grid-template-columns: 0.9fr 1fr 0.9fr;
  gap: 55px;
  align-items: start;
}

.provbls-hero-image img,
.provbls-red-image img,
.provbls-register-image img,
.provbls-class-image img {
  width: 100%;
  object-fit: cover;
}

.provbls-button .elementor-button,
.provbls-career-button .elementor-button {
  background: #A72D34;
  color: #FFFFFF;
  text-transform: uppercase;
  font-weight: 800;
  border-radius: 4px;
  transition: background-color 0.25s ease;
}

.provbls-button .elementor-button:hover,
.provbls-career-button .elementor-button:hover {
  background: #8F252B;
}

@media (max-width: 1024px) {
  .provbls-hero-inner,
  .provbls-red-inner,
  .provbls-register-inner,
  .provbls-class-grid { gap: 40px; }

  .provbls-benefit-grid {
    grid-template-columns: repeat(2, 1fr);
    gap: 55px;
  }
}

@media (max-width: 767px) {
  .provbls-hero-inner,
  .provbls-red-inner,
  .provbls-register-inner,
  .provbls-class-grid,
  .provbls-benefit-grid {
    grid-template-columns: 1fr;
  }

  .provbls-red-image img,
  .provbls-register-image img { height: 280px; }
  .provbls-class-image img { height: 240px; }
  .provbls-map-section { min-height: 260px; }
}
```

## Production Build Report

### Sections

Ten page-body sections: hero, badge strip, red BLS feature, benefits, recommendation, provider class, renewal class, registration, career CTA, and map.

### Widgets

- Containers
- Heading
- Text Editor
- Button
- Image
- Icon
- Divider
- Google Maps
- Editable background image and overlay controls

### Images Requiring Approved Media

- Hero CPR/chest-compressions image.
- Three certification badge images.
- First-aid kit or emergency supplies feature image.
- Provider class CPR mannequin image.
- Renewal healthcare worker portrait.
- Registration healthcare student/nurse image.
- Existing healthcare surgical/medical team CTA background.

### Placeholder Links

- Hero `GET STARTED`.
- Hero `GET DIRECTIONS`.
- Feature `GET STARTED`.
- Provider class `GET STARTED`.
- Renewal class `GET STARTED`.
- Registration `GET STARTED`.
- Final `CONTACT US`.

All remain `#` until final production URLs are confirmed.

## Quality Check

- Page sections follow the required ten-section order.
- Every content block uses an editable Elementor widget.
- Desktop, tablet, and mobile layouts are configured separately where needed.
- All page-specific classes use the `provbls-*` prefix.
- Global typography, colors, buttons, header, footer, and Site Settings remain untouched.
- Map is directly above the global footer.
- No screenshot is used as page content.
- Replace and optimize all placeholder media before launch.
- Compare Elementor Preview with the supplied reference at desktop, tablet, and mobile breakpoints before publishing.
