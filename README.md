# 1st Providence WordPress and Elementor Rebuild

Public documentation for the 1st Providence WordPress and Elementor rebuild workflow.

**This is a public learning blueprint, not a complete WordPress backup.** It teaches the rebuild process while keeping private client work, generated templates, databases, credentials, and media files out of the public repository.

## What This Repo Contains

✅ **Public content that followers can use:**
- Detailed page structure blueprints (`docs/`)
- Elementor design system and style guide
- Build notes and technical guidance
- Section breakdown maps (`elementor-outputs/section-maps/`)
- Approved public reference exports
- Workflow documentation for agents (`AGENTS.md`)

## What This Repo Does NOT Contain

❌ **Private content intentionally excluded:**
- Generated Elementor templates (`.json` files)
- Private client page layouts
- WordPress backups or database files
- Database credentials or `.env` files
- Media libraries and client assets
- Production-sensitive exports
- Day-to-day work notes

These items are protected by `.gitignore` to maintain client privacy and repository focus.

## Repository Structure

```
1st providence rebuild/
│
├── README.md                                  # This file
├── AGENTS.md                                  # Agent guidelines for future work
├── PROJECT_PROGRESS.md                        # Public milestone tracking
├── IMPLEMENTATION_PHASES.md                   # Workflow phases
├── BUGS_AND_SOLUTIONS.md                      # Known issues and solutions
├── .gitignore                                 # Scoped ignore rules
│
├── docs/                                      # Public documentation
│   ├── 1ST_PROVIDENCE_BLUEPRINT.md            # Main page structure blueprint
│   ├── ELEMENTOR_BUILD_NOTES.md               # Build guidance and notes
│   ├── STYLE_GUIDE.md                         # Global design system
│   ├── PERSONAL_CARE_AIDE_PCA_BLUEPRINT.md    # Program-specific blueprint
│   ├── BASIC_LIFE_SUPPORT_PROVIDER_BLUEPRINT.md
│   └── REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md  # Output workflow guide
│
├── codex-skills/                              # Agent instructions (public)
│   ├── codex-instruction-authoring.md
│   ├── distinctive-frontend-design.md
│   └── ...
│
└── elementor-outputs/                         # Local Elementor workspace
    ├── README.md                              # Output folder guide
    ├── elementor-templates/                   # Generated templates (ignored)
    │   ├── .gitkeep
    │   ├── README.md
    │   └── *.json                             # Local output (ignored by Git)
    ├── private-templates/                     # Private templates (ignored)
    │   ├── .gitkeep
    │   └── README.md
    ├── references/                            # Public reference materials
    │   ├── README.md
    │   ├── exports/                           # Approved public exports
    │   │   └── .gitkeep
    │   └── screenshots/                       # Public-safe visual references
    │       └── .gitkeep
    └── section-maps/                          # Page structure documentation
        ├── .gitkeep
        ├── nurse-aide-page-section-map.md
        ├── medication-management-page-section-map.md
        └── ...
```

## How The Elementor Workflow Works

**For agents building or modifying pages:**

1. **Read [AGENTS.md](AGENTS.md)** to understand public repository rules and commit policies
2. **Review the relevant blueprint** in [docs/](docs/) based on the page you're building
   - Start with [1ST_PROVIDENCE_BLUEPRINT.md](docs/1ST_PROVIDENCE_BLUEPRINT.md) for general structure
   - Program-specific pages: [PERSONAL_CARE_AIDE_PCA_BLUEPRINT.md](docs/PERSONAL_CARE_AIDE_PCA_BLUEPRINT.md), etc.
3. **Review [docs/STYLE_GUIDE.md](docs/STYLE_GUIDE.md)** to understand:
   - Global color palette and typography
   - Button styles and spacing rules
   - Class naming conventions
   - Responsive breakpoints
4. **Study approved reference exports** in `elementor-outputs/references/exports/` to see approved patterns
5. **Build the Elementor page/section/component** locally in WordPress
6. **Export the template as JSON** from Elementor
7. **Save the generated output** to `elementor-outputs/elementor-templates/` using the naming format
8. **Update section maps** in `elementor-outputs/section-maps/` if page structure changed
9. **Update documentation** (README, build notes, blueprints) if needed
10. **Commit only public files:**
    - Documentation updates
    - Section maps
    - Approved reference exports (with owner approval)
    - `.gitkeep` and README files

**Never commit:**
- Generated Elementor templates (`.json` files) unless explicitly approved
- Private templates
- Credentials or `.env` files
- Media or database files

## Public Documentation

### Getting Started

- **[AGENTS.md](AGENTS.md)** — Agent guidelines, commit rules, template naming, and verification checklist
- **[REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md](docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md)** — Detailed explanation of the output workflow

### Blueprints and Design

- **[1ST_PROVIDENCE_BLUEPRINT.md](docs/1ST_PROVIDENCE_BLUEPRINT.md)** — Main page structure and navigation
- **[PERSONAL_CARE_AIDE_PCA_BLUEPRINT.md](docs/PERSONAL_CARE_AIDE_PCA_BLUEPRINT.md)** — PCA program page structure
- **[BASIC_LIFE_SUPPORT_PROVIDER_BLUEPRINT.md](docs/BASIC_LIFE_SUPPORT_PROVIDER_BLUEPRINT.md)** — BLS program page structure
- **[STYLE_GUIDE.md](docs/STYLE_GUIDE.md)** — Global design system, colors, typography, and class conventions
- **[ELEMENTOR_BUILD_NOTES.md](docs/ELEMENTOR_BUILD_NOTES.md)** — Technical build guidance

### Progress and Issues

- **[PROJECT_PROGRESS.md](PROJECT_PROGRESS.md)** — Public milestones and completed work
- **[IMPLEMENTATION_PHASES.md](IMPLEMENTATION_PHASES.md)** — Workflow phases
- **[BUGS_AND_SOLUTIONS.md](BUGS_AND_SOLUTIONS.md)** — Known issues and solutions

## For Future Agents

**Before making any changes, read these in order:**

1. [AGENTS.md](AGENTS.md) — Understand the rules
2. [REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md](docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md) — Understand the folder organization
3. Relevant blueprint in [docs/](docs/) — Understand what you're building
4. [STYLE_GUIDE.md](docs/STYLE_GUIDE.md) — Know the design system
5. Reference exports in [elementor-outputs/references/exports/](elementor-outputs/references/exports/) — See approved patterns

**When you complete work:**

1. Export Elementor templates as JSON to `elementor-outputs/elementor-templates/`
2. Update section maps in `elementor-outputs/section-maps/`
3. Update documentation in `docs/` if needed
4. Run `git status --short` to verify your changes
5. Commit only public documentation, section maps, and approved reference exports
6. Never commit generated Elementor templates unless explicitly approved

See [AGENTS.md](AGENTS.md) for complete guidelines and the commit verification checklist.

## Privacy And Output Rules

### Why Generated Templates Are Ignored

Generated Elementor `.json` templates are excluded from the public repository because:

1. **Client privacy** — Exports can contain proprietary layouts or client-approved designs
2. **Production safety** — Full Elementor outputs tied to production should not be public
3. **Learning focus** — This repo teaches the *process*, not distributing production templates
4. **Flexibility** — The rebuild team can iterate privately without exposing incomplete work

### Folder Rules

| Folder | Git behavior | Contents |
|--------|---|---|
| `docs/` | ✅ Committed | Public blueprints and style guide |
| `codex-skills/` | ✅ Committed | Agent instructions and skills |
| `elementor-outputs/elementor-templates/` | ❌ Ignored | Generated Elementor templates (local only) |
| `elementor-outputs/private-templates/` | ❌ Ignored | Private/confidential templates (local only) |
| `elementor-outputs/references/exports/` | ✅ Committed | Approved public reference exports |
| `elementor-outputs/section-maps/` | ✅ Committed | Markdown section documentation |

### Before Every Commit

**Verification checklist:**

- ✅ No generated templates in `elementor-outputs/elementor-templates/`
- ✅ No files from `elementor-outputs/private-templates/`
- ✅ No `.env`, `wp-config.php`, or credentials
- ✅ No database files or WordPress backups
- ✅ No media files (`.jpg`, `.png`, `.webp`) outside approved folders
- ✅ No day-to-day work files
- ✅ All staged files are public documentation or approved exports

**Run these commands:**

```bash
git status --short          # See what will be committed
git check-ignore -v <file>  # Verify a file should be ignored
git diff --cached           # Review the exact diff
```

---

**Last updated:** 2026-06-15

For detailed information about the workflow, see [AGENTS.md](AGENTS.md) and [docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md](docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md).
