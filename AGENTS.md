# Repository guidance for Codex

## Project
- This repository is a static Russian-language product-design portfolio; there is no package manager or build step.
- The homepage is `index.html`. Portfolio case pages are `core/index.html` (CORE, a private messenger case study) and `echo/index.html` (ECHO, an influencer/business platform case study).
- Shared site styles are in `styles.css`. Media and local font files are in `assets/`.
- The `core/` page in this repository is a **portfolio case study**, not the separate client web application sometimes called "Core" in design discussions. Do not change the client application unless its own repository is explicitly selected.

## Rules for changes
- Implement only the explicitly agreed scope. Do not redesign unrelated sections, rewrite content, or refactor working code without a clear request.
- Preserve existing layout, typography, component patterns, responsive behavior, and Russian copy except where the task explicitly requests changes.
- Check for CSS side effects on all three pages whenever modifying `styles.css`. Prefer focused, reusable selectors rather than broad overrides.
- Keep references to local assets and locally hosted fonts working; do not delete, replace, or rename media files without explicit authorization.
- Avoid introducing a build system, frameworks, external dependencies, or remote font loading unless explicitly requested.
- Protect accessibility basics: meaningful alt text, keyboard operability, focus states, semantic markup, and reduced-motion behavior where relevant.
- Do not include credentials, keys, personal data, or secrets in source control.

## Verification
- Serve the site locally over HTTP, rather than relying only on `file://` URLs.
- Check the affected pages on representative mobile and desktop viewports; inspect for horizontal overflow, unintended layout changes, and missing media.
- Verify that edited HTML, CSS, and JavaScript are syntactically valid using available tools, and that referenced local resources exist.
- Report what was tested and what could not be checked. Do not claim visual verification if no browser or screenshot inspection was performed.

## Git and review
- Work on a dedicated branch for each change. Never push straight to `main`.
- Create clear, focused commits and provide a pull request for review. Do not merge without the user's approval.
- In the pull request, summarize changed files, behavior, verification, and any open questions or risks.
- If the request is ambiguous or conflicts with existing design constraints, identify the conflict before making a potentially destructive change.
