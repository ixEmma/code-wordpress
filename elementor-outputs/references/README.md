# Reference Outputs

This folder contains **public-safe reference material** used to guide Elementor rebuilds and for followers to learn from.

## folders

### `exports/`

Approved public Elementor JSON reference exports can be placed here.

**Examples:**
- Hero section reference patterns
- Approved layout examples
- Public component templates
- Learning materials

**Rules:**
- Files here are visible in the public repository
- Only add files with explicit owner approval
- Must be safe for public distribution
- No private client layouts
- No production-sensitive exports

### `screenshots/`

Only **public-safe visual references** should be placed here.

**Examples:**
- Approved design mockups
- Public visual references
- Learning materials
- Approved wireframes

**Never include:**
- Private client screenshots
- Production-sensitive visuals
- Unreleased designs
- Credentials or sensitive information
- Internal notes or comments

## Important

- All files in this folder are visible in the public repository
- Do not add files without explicit owner approval
- Review files for any private or sensitive data before adding
- Do not commit private client layouts, production exports, or unreleased designs
- This folder is for **public learning materials only**

## Workflow

**To add a public reference:**

1. Owner reviews and approves the file for public use
2. File is saved to `exports/` or `screenshots/`
3. File is staged and committed with public documentation
4. Documentation is updated if needed

**To move a generated template here:**

1. Owner reviews the template
2. Confirms it contains no private data
3. Gets explicit approval to publish
4. Moves the file from `../elementor-templates/` to `exports/`
5. Stages and commits

See [AGENTS.md](../../AGENTS.md) for detailed rules on what to commit and what to keep private.

See [REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md](../../docs/REPO_STRUCTURE_AND_OUTPUT_WORKFLOW.md) for complete guidance.
