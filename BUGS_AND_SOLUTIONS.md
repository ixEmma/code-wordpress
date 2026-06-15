# Bugs And Solutions

## Elementor Outputs In Public Git

Problem: Elementor export files and page output artifacts can contain client-owned layouts or private implementation details.

Solution: Exclude `elementor-outputs/`, `*.json`, screenshots, archives, media files, WordPress folders, database files, and environment files from Git.

## Header/Footer Duplication Risk

Problem: Rebuilding global header or footer inside page bodies can create duplicated navigation and inconsistent maintenance.

Solution: Keep page templates body-only. Header and footer remain global Elementor/WordPress templates.

## Flattened Page Content Risk

Problem: Long program pages can accidentally become one large text block.

Solution: Each section must be represented as its own Elementor Container with editable native widgets.

## Style Leakage Risk

Problem: Shared class names or broad CSS selectors can affect unrelated pages.

Solution: Use page-specific class prefixes such as `provmed68-*`, `provmanage-*`, and `provekg-*`.

## Public repo output folders not visible

Problem: Followers could not understand the Elementor output workflow because generated output folders were not visible in GitHub.

Cause: Git does not track empty folders, and earlier ignore rules blocked important workflow structure such as the output folder, JSON reference examples, and agent instructions.

Solution: Added public placeholder files and README files inside the output structure. Confirmed that AGENTS.md, public documentation, section maps, and safe reference exports can be committed while private/generated Elementor templates remain ignored.
