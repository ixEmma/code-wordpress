# Elementor System Architecture Skill

## Purpose

Use this skill when working with Elementor page structure, Elementor JSON, WordPress page templates, Elementor Containers, programmatic saves, or debugging why Elementor content does not appear correctly.

This skill exists to prevent blind editing. Elementor pages are not plain HTML. Elementor stores layouts as structured JSON in WordPress post meta, then renders that data through Elementor, PHP, WordPress templates, generated CSS files, and browser output.

## Core Rule

Before making any Elementor-related edit, first identify what controls the page and how Elementor is storing the content.

Do not edit blindly.

## Mandatory Pre-Edit Analysis

Before editing an Elementor page, check or reason through these items:

1. What controls the page layout?
   - Default theme template
   - Elementor Canvas
   - Elementor Full Width
   - Theme Builder template
   - Custom WordPress page template

2. What is inside `_elementor_data`?
   - Is it present?
   - Is it valid JSON?
   - Is it empty?
   - Is it corrupted by escaping or slashes?

3. Is the page actually set to Elementor mode?
   - `_elementor_edit_mode` should be `builder`.

4. Are global or reusable Elementor templates involved?
   - Header template
   - Footer template
   - Global widgets
   - Saved sections
   - Theme Builder templates

5. What does the active Elementor Kit define?
   - Global colors
   - Global typography
   - Buttons
   - Spacing
   - Page layout defaults

6. Are Elementor Containers active and being used?
   - Use Containers for modern builds.
   - Do not use legacy Sections and Columns for new builds unless specifically required.

7. Is Elementor CSS cache stale?
   - Elementor generates page CSS files.
   - Stale generated CSS can make correct content appear broken.

## Elementor Rendering Flow

Elementor content follows this flow:

```txt
HTTP request
  → WordPress bootstrap
  → WordPress selects theme/page template
  → Elementor hooks into the page render
  → Elementor reads _elementor_data from wp_postmeta
  → Elementor parses layout JSON
  → Elementor renders each container and widget through PHP classes
  → Elementor generates or loads CSS files
  → Browser receives final HTML and CSS