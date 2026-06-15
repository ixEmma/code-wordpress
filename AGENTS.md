# AGENTS.md

## Project Purpose

This repository documents the 1st Providence WordPress and Elementor rebuild workflow.

The public repository is a **learning blueprint**, not a full WordPress backup. It teaches followers how to:
- Plan WordPress page structures
- Build Elementor page templates with consistent styling
- Organize reusable components
- Document page blueprints and design systems
- Maintain workflow separation between public documentation and private outputs

## Public Repository Rules

1. **Public content** must never expose private client work, generated templates, databases, credentials, or production media.
2. **Documentation is public**: blueprints, style guides, section maps, and design notes.
3. **Placeholder files are public**: `.gitkeep` files and README files inside output folders.
4. **Reference exports are optional**: Approved public reference exports may be placed in `elementor-outputs/references/exports/` if the owner explicitly approves.
5. **Never commit generated Elementor templates** unless intentionally reviewed and approved for public use.

## Private Data Rules

**Never commit these file types:**

- `.env`, `.env.*`, `wp-config.php` (credentials)
- `elementor-outputs/elementor-templates/*.json` (generated templates, ignored by default)
- `elementor-outputs/private-templates/**` (private templates, always ignored)
- `*.sql`, `*.sql.gz`, `*.wpress`, database files (backups)
- `wp-content/`, `wordpress/`, `uploads/`, `backup/`, `database/` folders
- `*.jpg`, `*.png`, `*.webp` (client media, ignored by default)
- `AGENTS.local.md`, `AGENT_PRIVATE_NOTES.md`, `LOCAL_DAILY_WORK.md` (local notes, ignored)

## Required Folder Structure

```
codex-skills/                              # Public skills and instructions
docs/
  1ST_PROVIDENCE_BLUEPRINT.md              # Main blueprint
  ELEMENTOR_BUILD_NOTES.md                 # Build guidance
  STYLE_GUIDE.md                           # Design system
  PERSONAL_CARE_AIDE_PCA_BLUEPRINT.md      # Program blueprint
  BASIC_LIFE_SUPPORT_PROVIDER_BLUEPRINT.md # Program blueprint
  REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md    # Output workflow (public)
elementor-outputs/
  README.md                                # Output folder guide (public)
  elementor-templates/                     # Generated templates folder
    .gitkeep                               # Placeholder (public)
    README.md                              # Naming guide (public)
  private-templates/                       # Private templates folder
    .gitkeep                               # Placeholder (public)
    README.md                              # Rules (public)
  references/
    README.md                              # Reference guide (public)
    exports/
      .gitkeep                             # Placeholder (public)
    screenshots/
      .gitkeep                             # Placeholder (public)
  section-maps/                            # Section maps folder
    .gitkeep                               # Placeholder (public)
README.md                                  # Main project README
PROJECT_PROGRESS.md                        # Public milestones only
IMPLEMENTATION_PHASES.md                   # Workflow phases
BUGS_AND_SOLUTIONS.md                      # Known issues and solutions
AGENTS.md                                  # This file (public)
.gitignore                                 # Scoped ignore rules
```

## Elementor Output Rules

### Generated Elementor Templates

**Location:** `elementor-outputs/elementor-templates/`

**Format:** Elementor JSON `.json` files

**Git behavior:** Ignored by default. Never commit without owner approval.

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
medication-management-page-body-template.json
ekg-why-students-choose-section-template.json
header-mega-menu-template.json
```

**Important:** When a task asks you to "build a page," "build a section," or "build a template," you must produce a real Elementor `.json` file. Markdown-only output is not sufficient.

### Private Templates

**Location:** `elementor-outputs/private-templates/`

**Git behavior:** Completely ignored. Never commit from this folder.

**Use cases:**
- Client-sensitive page layouts
- Production-only templates
- Early draft versions
- Day-to-day working exports

## Reference Export Rules

**Location:** `elementor-outputs/references/exports/`

**Git behavior:** Allowed in Git. Must be explicitly approved before committing.

**When to use:**
- Public-safe Elementor references
- Approved sample exports
- Learning materials

**When NOT to use:**
- Private client layouts
- Production-sensitive exports
- Unreleased designs

## Daily Work Privacy Rules

1. **Day-to-day work notes stay local.** Never commit daily worklog files.
2. **Use local ignored files for private notes:**
   - `AGENTS.local.md` for local agent instructions
   - `AGENT_PRIVATE_NOTES.md` for private development notes
   - `LOCAL_DAILY_WORK.md` for daily work tracking
3. **Commit only public milestones** to `PROJECT_PROGRESS.md`.
4. **Generate Elementor outputs locally,** then decide what to publish.

## How To Build A New Elementor Page

**Workflow:**

1. **Read AGENTS.md** (this file). Understand the rules.
2. **Review the relevant blueprint** in `docs/`. Example: `docs/1ST_PROVIDENCE_BLUEPRINT.md` for general structure, `docs/NURSE_AIDE_PCA_BLUEPRINT.md` for program pages.
3. **Review `docs/STYLE_GUIDE.md`** to understand:
   - Global color palette
   - Typography rules
   - Button styles
   - Responsive breakpoints
   - Class naming conventions
4. **Review public reference exports** in `elementor-outputs/references/exports/` to see approved patterns.
5. **Build the Elementor template locally:**
   - Use page-specific class prefixes (e.g., `nurse-*`, `provmanage-*`) to scope styles
   - Follow the section structure from the blueprint
   - Use only approved colors and typography
   - Use real Elementor widgets (containers, text, buttons, images)
6. **Export the template as JSON** from Elementor
7. **Save the JSON file** to `elementor-outputs/elementor-templates/` using the naming format
8. **Update section maps** in `elementor-outputs/section-maps/` if the page structure changed
9. **Update public documentation** in `docs/` if needed
10. **Stage only public files** for commit (README updates, section maps, approved reference exports)

## How To Build A New Elementor Section

**Workflow:**

1. **Read AGENTS.md** and the relevant blueprint.
2. **Review STYLE_GUIDE.md** for section patterns.
3. **Review public reference exports** to see approved patterns.
4. **Build the section in Elementor:**
   - Use consistent naming for nested containers
   - Scope all class names with section/page prefix
   - Use approved colors, fonts, and spacing
5. **Export as JSON** from Elementor
6. **Save to `elementor-outputs/elementor-templates/`** using the naming format: `page-name-section-name-template.json`
7. **Update the section map** in `elementor-outputs/section-maps/page-name-section-map.md`
8. **Commit only the updated section map** (not the template)

## Template Naming Rules

**Page body templates:**
```
page-name-page-body-template.json
```
Examples:
- `homepage-body-template.json`
- `nurse-aide-page-body-template.json`
- `medication-management-page-body-template.json`

**Section templates:**
```
page-name-section-name-template.json
```
Examples:
- `ekg-why-students-choose-section-template.json`
- `nurse-aide-schedule-section-template.json`

**Component templates:**
```
page-name-component-name-template.json
```
Examples:
- `homepage-cta-button-template.json`
- `nurse-aide-faq-template.json`

**Global/header/footer templates:**
```
header-mega-menu-template.json
footer-contact-section-template.json
```

## Documentation Rules

1. **Blueprints** must include:
   - Page purpose
   - Section structure
   - Content requirements
   - Styling rules (colors, fonts)
   - Class naming conventions

2. **Section maps** must include:
   - Visual breakdown of page sections
   - Section names and classes
   - Widget structure
   - Responsive considerations

3. **README files** in output folders explain:
   - Folder purpose
   - File types and naming
   - Git behavior
   - When/how to use the folder

## What To Commit

**Safe to commit:**
- `README.md` updates
- Root documentation files (`AGENTS.md`, `PROJECT_PROGRESS.md`, `IMPLEMENTATION_PHASES.md`, `BUGS_AND_SOLUTIONS.md`)
- `docs/` folder updates (blueprints, build notes, style guides)
- `codex-skills/` folder updates
- `elementor-outputs/` subfolders' README files and `.gitkeep` files
- `elementor-outputs/section-maps/*.md` files
- `elementor-outputs/references/exports/` files (only when approved)
- `.gitignore` updates (only for policy changes)

**Never commit:**
- `elementor-outputs/elementor-templates/*.json` (generated templates)
- `elementor-outputs/private-templates/**` (private templates)
- `.env`, `wp-config.php`, credentials
- `*.sql`, database files, backups
- Media files (`*.jpg`, `*.png`, `*.webp`)
- Local ignored work files

## What Never To Commit

**Hard block files (ignored by Git):**

- All `.env*` files and `wp-config.php`
- All `*.json` inside `elementor-outputs/elementor-templates/`
- All files inside `elementor-outputs/private-templates/`
- All `*.sql`, `*.sql.gz`, `*.wpress` database/backup files
- All media inside `wp-content/`, `uploads/`, `backup/`, `media-library/` folders
- All `*.jpg`, `*.jpeg`, `*.png`, `*.webp`, `*.gif`, `*.svg`, `*.pdf`, `*.psd`, `*.ai`, `*.indd` (client media, ignored by default)
- Local work files: `AGENTS.local.md`, `AGENT_PRIVATE_NOTES.md`, `LOCAL_DAILY_WORK.md`, `DAILY_WORKLOG.md`

**Manual block files (require review before commit):**

- Any Elementor JSON file
- Any production screenshot
- Any day-to-day work note

## Verification Checklist Before Commit

**Before running `git add` or `git commit`:**

1. ✅ **Am I updating public documentation only?** (README, blueprints, section maps, build notes, style guide)
2. ✅ **Did I review `.gitignore` rules?** Run: `git check-ignore -v <filename>` on uncertain files
3. ✅ **No generated Elementor templates?** Check that no `*.json` from `elementor-outputs/elementor-templates/` is staged
4. ✅ **No private templates?** Check that no files from `elementor-outputs/private-templates/` is staged
5. ✅ **No credentials?** Check for `.env`, `wp-config.php`, API keys
6. ✅ **No media files?** Check for `*.jpg`, `*.png`, `*.webp` outside approved reference folders
7. ✅ **No databases?** Check for `*.sql`, `*.sql.gz`, backups
8. ✅ **No day-to-day work?** Check that `AGENTS.local.md`, `LOCAL_DAILY_WORK.md` are NOT staged
9. ✅ **Reference exports approved?** If committing from `elementor-outputs/references/exports/`, confirm owner approval
10. ✅ **Run `git status --short`** to see the exact list of staged and unstaged changes
11. ✅ **Run `git diff --cached`** to review the diff of staged files
12. ✅ **Confirm commit message** is clear and public-safe

**Example safe commits:**

```bash
git add docs/STYLE_GUIDE.md AGENTS.md README.md
git commit -m "Add AGENTS.md and update public documentation"
```

```bash
git add elementor-outputs/section-maps/
git commit -m "Add section maps for program pages"
```

**Example unsafe commits (do not do this):**

```bash
git add elementor-outputs/elementor-templates/  # Contains generated JSON files!
git add elementor-outputs/private-templates/    # Contains private templates!
git add .env                                     # Contains credentials!
```

## How Future Agents Should Use This Repository

1. **Start by reading AGENTS.md** (this file) to understand public rules.
2. **Understand the folder structure** from `docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md`.
3. **Review relevant blueprints** in `docs/` based on the task.
4. **Review `docs/STYLE_GUIDE.md`** before building any new templates.
5. **Generate Elementor outputs locally** in `elementor-outputs/elementor-templates/`.
6. **Commit only public documentation and approved reference exports.**
7. **Never commit generated templates unless explicitly instructed by the owner.**

---

**Last updated:** 2026-06-15

This is the public agent guidance for the 1st Providence rebuild project. Future agents and contributors must follow these rules to maintain the public/private separation and keep the repository useful for followers.
