# Copilot Instructions for cube-drop-privacy

## Repository Overview

This repository hosts the **public-facing static website** for [Cube Drop: Brain Block Game](https://play.google.com/store), an Android puzzle game. The site is deployed via GitHub Pages and contains:

- `index.html` — Landing page with links to the privacy policy and account-removal instructions.
- `privacy_policy.html` — Full privacy policy for the app.
- `remove-account.md` — Instructions for users who want to erase their game data.

## Tech Stack

- **Pure HTML/CSS** — no JavaScript frameworks, no build tools, no package managers.
- **No dependencies** — all styling is inline `<style>` blocks; no external stylesheets or CDN links.
- **GitHub Pages** — the site is served directly from the repository root.

## Design Conventions

- Background colour: `#0f0f1a` (dark navy).
- Primary accent: `#00e5ff` (cyan).
- Secondary accent: `#e040fb` (purple).
- Body text: `#d0d0e8`; muted text: `#b0b0cc`.
- Border / card background: `#1a1a35` with `1px solid #2a2a55`.
- Headings use `h2` with a left cyan border (`border-left: 3px solid #00e5ff`).
- Keep all styles in `<style>` blocks inside `<head>` — do **not** add external CSS files.

## Content Guidelines

- The app collects **no personal data**; all storage is local-only via Android SharedPreferences.
- Keep legal language plain and jargon-free.
- All pages must include the `CUBEDROP` logo header and a `© 2026` footer.
- Do **not** add third-party analytics, tracking pixels, or external scripts.

## Editing Guidelines

- Maintain consistent indentation (2 spaces).
- Preserve the existing comment blocks (e.g., `<!-- ───── SECTION ───── -->`) when editing `privacy_policy.html`.
- When updating effective/last-updated dates, change both the visible text and any `<strong>` wrappers in `privacy_policy.html`.
- `remove-account.md` should remain a single concise paragraph — no headers needed.

## No Build / Test Pipeline

There is no linter, bundler, or test suite. Validate changes by opening the HTML files in a browser.
