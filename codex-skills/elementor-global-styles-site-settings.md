# Elementor Global Styles and Site Settings Skill

## Purpose

Use this skill before planning or generating Elementor templates.

The goal is to make Codex define and reuse global styles instead of repeatedly hardcoding colors, fonts, button styles, spacing, radius, shadows, and section patterns inside individual widgets.

## Core Rule

Repeated design values must be treated as global styles.

Do not manually repeat the same color, font size, button style, border radius, shadow, or spacing pattern across many widgets.

## When to Use

Use this skill when:

1. Rebuilding a WordPress or Elementor page.
2. Cloning a homepage section by section.
3. Creating Elementor JSON templates.
4. Auditing an Elementor design.
5. Setting up a new Elementor site style system.
6. Matching a reference website.

## Global Styles to Define

Before building sections, identify:

1. Primary brand color.
2. Secondary brand color.
3. Accent color.
4. Main background color.
5. Alternate background color.
6. Main text color.
7. Muted text color.
8. Heading typography.
9. Body typography.
10. Button typography.
11. Button background colors.
12. Button hover colors.
13. Link colors.
14. Section padding.
15. Container max width.
16. Card border radius.
17. Image border radius.
18. Repeated border styles.
19. Repeated shadow styles.
20. Form/input styles if needed.

## Elementor Site Settings Areas

Use Elementor Site Settings for:

1. Global Colors.
2. Global Fonts.
3. Typography.
4. Buttons.
5. Form fields where applicable.
6. Layout width.
7. Background defaults where applicable.

## Global Color Rules

Do not create random one-off colors without checking if they already exist.

Use clear names such as:

```txt
Primary
Secondary
Accent
Dark Background
Light Background
Main Text
Muted Text
Border
White
Black