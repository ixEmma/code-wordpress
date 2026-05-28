# Elementor Senior Design System Skill

## Purpose

Use this skill when planning, designing, reviewing, or building Elementor layouts from a screenshot, reference website, brand guide, wireframe, or written brief.

The goal is to produce modern, responsive, conversion-focused Elementor layouts with strong hierarchy, clean spacing, balanced composition, and full editability.

This skill must work for many design styles. Do not force every page into the same static layout. First analyze the reference, then choose the right structure.

## Core Design Principle

Think like a senior UI/UX web designer before thinking like a page builder.

Every section must have:

1. A clear purpose.
2. A logical container structure.
3. Strong visual hierarchy.
4. Clean spacing.
5. Responsive behavior.
6. Consistent styling.
7. Editable Elementor widgets.
8. Premium visual balance.

Do not stack random widgets without structure.

## Dynamic Design Rule

Do not apply one fixed design formula to every project.

Before building, identify the design direction:

1. Corporate
2. Luxury
3. Healthcare
4. SaaS
5. Agency
6. Real estate
7. Restaurant
8. Ecommerce
9. Education
10. Nonprofit
11. Portfolio
12. Local business
13. Minimal editorial
14. Bold campaign landing page

Then adapt layout, spacing, typography, color usage, image treatment, and motion style to match the reference.

The design rules in this file are defaults, not rigid limits. If a reference requires a different structure, follow the reference while keeping the layout clean, responsive, and editable.

## Before Building Any Section

Always analyze first:

1. What is the section trying to achieve?
2. What is the user supposed to notice first?
3. What action should the user take?
4. What content is primary?
5. What content is secondary?
6. What layout pattern fits the content?
7. What should happen on tablet?
8. What should happen on mobile?
9. Which styles should come from global styles?
10. Which Elementor widgets are needed?

Never build before understanding the purpose.

## Elementor Build Rules

Use modern Elementor Containers.

Do not use:

1. Legacy Sections.
2. Legacy Columns.
3. Random nested containers.
4. Hardcoded HTML for normal layout.
5. Gutenberg blocks inside Elementor templates.
6. One-off repeated color values.
7. One-off repeated font settings.

Use:

1. Containers.
2. Nested containers only when needed.
3. Native Elementor widgets.
4. Global colors.
5. Global typography.
6. Global button styles.
7. Global spacing references where possible.
8. Editable image, text, and button widgets.

## Container Strategy

Use the fewest containers necessary to reproduce the design cleanly.

Common structure:

```txt
Outer Section Container
  Inner Width Container
    Content Containers
      Elementor Widgets