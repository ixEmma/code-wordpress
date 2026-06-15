# Repository Structure And Output Workflow

## Purpose

This document explains how the 1st Providence rebuild repository is organized and how the Elementor output workflow functions.

**This repository is NOT a complete WordPress backup.** It is a public learning blueprint showing:
- WordPress page structure planning
- Elementor template organization
- Reusable component architecture
- Design system documentation
- Section-by-section build guidance

## Why This Repo Does Not Include Full Private Outputs

**Generated Elementor templates** are excluded from the public repository because:

1. **Client privacy:** Elementor exports can contain proprietary layouts, sensitive page structures, or client-approved designs that should remain private.
2. **Production safety:** Full Elementor outputs tied to a production site should not be public.
3. **Learning focus:** The repository exists to teach the *process*, not to distribute production templates.
4. **Flexibility:** Private templates allow the rebuild team to iterate without exposing incomplete work.

**Files intentionally ignored:**
- Generated Elementor JSON templates
- Private Elementor templates
- WordPress backups and databases
- Environment files and credentials
- Media libraries and client assets
- Day-to-day work notes

## Public Documentation

**Committed to the repository:**

- Root documentation files: `README.md`, `AGENTS.md`, `PROJECT_PROGRESS.md`, `IMPLEMENTATION_PHASES.md`, `BUGS_AND_SOLUTIONS.md`
- `docs/` folder:
  - `1ST_PROVIDENCE_BLUEPRINT.md` — Main page structure blueprint
  - `ELEMENTOR_BUILD_NOTES.md` — Build guidance and technical notes
  - `STYLE_GUIDE.md` — Global design system (colors, typography, buttons, classes)
  - `PERSONAL_CARE_AIDE_PCA_BLUEPRINT.md` — Program-specific page blueprint
  - `BASIC_LIFE_SUPPORT_PROVIDER_BLUEPRINT.md` — Program-specific page blueprint
  - `REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md` — This document
- `codex-skills/` folder:
  - Agent instructions and skill documentation
- `elementor-outputs/` folder structure:
  - `README.md` — Output workspace guide
  - `elementor-templates/README.md` — Generated template naming rules
  - `private-templates/README.md` — Private template rules
  - `references/README.md` — Reference export guide
  - `.gitkeep` placeholder files
- `elementor-outputs/section-maps/` — All Markdown section maps (`*.md`)

## Elementor Output Workspace

**Location:** `elementor-outputs/`

This folder is the **local working directory** for all Elementor output, reference materials, and section documentation.

### Subfolders

#### `elementor-templates/`

**Purpose:** Local output folder for generated Elementor page and section templates.

**Git behavior:** Ignored (all `*.json` files excluded)

**Contents:**
- `*.json` files: Generated Elementor templates (e.g., `homepage-body-template.json`, `nurse-aide-page-body-template.json`)
- `README.md` — Public naming guide (committed)
- `.gitkeep` — Public placeholder file (committed)

**Important:** When you complete an Elementor build task that requires a "page," "section," or "component" template, the output must be a real `.json` Elementor export saved here.

#### `private-templates/`

**Purpose:** Folder for private, local-only, or client-sensitive Elementor templates.

**Git behavior:** Completely ignored (all files excluded)

**Use cases:**
- Early draft versions
- Client-sensitive layouts
- Production-only exports
- Day-to-day working templates

**Important:** Files in this folder are never committed. Use this folder to isolate private work from the public repository.

#### `references/`

**Purpose:** Approved public reference materials.

**Git behavior:** Committed (with owner approval)

**Subfolders:**

- `exports/` — Approved public Elementor JSON reference exports (e.g., example hero sections, approved layout patterns)
- `screenshots/` — Public-safe visual references (no client media, no credentials, no unreleased designs)

**Important:** Files in `references/` are visible in the public repository. Only add files that are explicitly approved for public use.

#### `section-maps/`

**Purpose:** Markdown documentation of page section structures.

**Git behavior:** Committed (all `*.md` files)

**Contents:**
- `*.md` files documenting the section breakdown of each page
- Each section map shows:
  - Visual breakdown of sections
  - Container and widget structure
  - Class names and CSS hierarchy
  - Responsive behavior
  - Nesting relationships

**Examples:**
```
nurse-aide-page-section-map.md
medication-management-page-section-map.md
electrocardiogram-technician-ekg-page-section-map.md
```

## Generated Templates

**Files:** All `.json` inside `elementor-outputs/elementor-templates/`

**Status:** Generated locally, ignored by Git

**Naming format:**
```
page-name-page-body-template.json
page-name-section-name-template.json
page-name-component-name-template.json
```

**Examples:**
```
homepage-body-template.json
nurse-aide-page-body-template.json
medication-aide-68-hour-page-body-template.json
ekg-why-students-choose-section-template.json
medication-management-page-body-template.json
meet-our-trainers-page-body-template.json
```

**Important rules:**

1. Generated templates are **never** part of the public commit unless explicitly reviewed and approved.
2. If a build task says "build a page," "build a section," or "build a component," the output must be a real Elementor `.json` file, not Markdown documentation alone.
3. Every Elementor export goes here first. The owner then decides whether to move it to `references/exports/` for public use.

## Private Templates

**Files:** All files inside `elementor-outputs/private-templates/`

**Status:** Private, never committed

**Use for:**
- Client-sensitive or unreleased page layouts
- Production-only templates
- Early draft versions
- Day-to-day working copies

**Important:** Do not move private templates into `references/exports/` without explicit owner approval.

## Reference Exports

**Location:** `elementor-outputs/references/exports/`

**Status:** Public, committed (with approval)

**What can go here:**
- Approved public Elementor JSON exports (e.g., example hero section, approved layout pattern, reference component)
- Learning materials that help followers understand the rebuild approach

**What cannot go here:**
- Private client layouts
- Production-sensitive exports
- Unreleased designs
- Incomplete or in-progress templates

## Section Maps

**Location:** `elementor-outputs/section-maps/`

**Files:** All Markdown files (`*.md`)

**Status:** Public, committed

**Purpose:** Document the structure and organization of each page, including:
- Visual layout breakdown
- Container hierarchy
- Widget types and content
- Class names and CSS scope
- Responsive breakpoints
- Nesting relationships

**Example content:**

```markdown
# Nurse Aide Page Section Map

## Hero Section
- Container: `.nurse-hero`
- Content: Title, subtitle, featured image
- Classes: `.nurse-hero`, `.nurse-hero__text`, `.nurse-hero__image`

## Why Choose Section
- Container: `.nurse-why`
- Content: 3-column feature grid
- Classes: `.nurse-why`, `.nurse-why__item`, `.nurse-why__icon`

## Testimonials Section
- Container: `.nurse-testimonials`
- Content: Testimonial carousel
- Classes: `.nurse-testimonials`, `.nurse-testimonials__item`
```

## Daily Work Privacy

**Ignored local work files:**

- `AGENTS.local.md` — Local agent instructions and notes
- `AGENT_PRIVATE_NOTES.md` — Private development notes
- `LOCAL_DAILY_WORK.md` — Daily work tracking
- `DAILY_WORKLOG.md` — Daily activity log

These files are in `.gitignore` and will never be committed. Use them to track day-to-day work without affecting the public repository.

## What Followers Can Use

**Followers downloading this repository can access and learn from:**

1. **Blueprints and planning documents** — Understand how each page is structured
2. **Style guide** — Learn the design system, colors, typography, and naming conventions
3. **Build notes** — Understand technical decisions and Elementor best practices
4. **Section maps** — See how each page is broken down into components
5. **Approved reference exports** — Study approved Elementor patterns
6. **Agent guidelines** — Understand how future work should be organized

**Followers cannot and should not:**

- Access generated production templates (not public)
- Access private templates (not public)
- Access credentials or environment files (not public)
- Access WordPress backups or databases (not public)
- Access client media or unreleased designs (not public)

## What Future Agents Should Do

**When building or modifying the Elementor site:**

1. **Read AGENTS.md** to understand public repository rules.
2. **Review this document** to understand the folder structure.
3. **Study the relevant blueprint** in `docs/`.
4. **Review the style guide** in `docs/STYLE_GUIDE.md`.
5. **Generate Elementor templates locally** in `elementor-outputs/elementor-templates/`.
6. **Save section maps** and public documentation updates in `elementor-outputs/section-maps/`.
7. **Update public docs** like README files and build notes as needed.
8. **Commit only public documentation and approved reference exports.**
9. **Never commit generated templates** unless explicitly instructed by the owner.
10. **Use private-templates/ and local ignored files** for any private work.

## Safe Commit Checklist

**Before committing, verify:**

- ✅ No generated templates in `elementor-outputs/elementor-templates/*.json` are staged
- ✅ No files from `elementor-outputs/private-templates/` are staged
- ✅ No `.env`, `wp-config.php`, or credentials are staged
- ✅ No database files or WordPress backups are staged
- ✅ No media files outside approved reference folders are staged
- ✅ No local ignored work files are staged
- ✅ All staged files are public documentation, section maps, or approved reference exports
- ✅ Commit message is clear and public-safe

**Run these commands to verify:**

```bash
git status --short                          # See staged and unstaged files
git check-ignore -v <filename>              # Check if a file should be ignored
git diff --cached                           # Review exact diff of staged changes
```

---

**Last updated:** 2026-06-15

This document is the public explanation of the repository structure and output workflow. Future agents and followers should read this to understand how the Elementor rebuild process is organized.
