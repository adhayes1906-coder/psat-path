# PSAT Path

Small steps. Stronger skills.

A calm, interactive PSAT skills workbook with worked solutions, optional 1.5x module timers, progress tracking, and a study calendar.

## Features

- 8 learning cycles and 24 sessions from the supplied Third Edition workbook.
- 64 scored practice questions, 8 unscored memory checks, and worked explanations for all 72 prompts.
- Step-by-step equations with formatted fractions, powers, square roots, and final answers in every math solution.
- Separate Questions, Answers & solutions, and Learn more tabs.
- Four independent, optional module timer presets: Reading & Writing 1/2 at 48:00; Math 1/2 at 52:30.
- Saved answers, self-reviewed accuracy, session completion, K/F/U/T/G tags, reflections, and a revisit list.
- Month calendar with completed study days and editable planned sessions.
- Automatic schedules for 3 days/week (8 weeks) or 2 days/week (12 weeks), keeping all sessions in sequence.
- Responsive layout, larger text, keyboard-accessible tabs, and reduced-motion support.
- Browser-local saving with JSON backup export/import.
- Separate demo mode with sample data: open the site with `?demo=1`.

## Publish

Follow [GITHUB-SETUP.md](GITHUB-SETUP.md). No build step, package installation, server account, or API key is required. Publish this directory from `main` at `/ (root)` using GitHub Pages.

To preview locally, open `index.html` in a browser or serve this directory with a static web server. Some browsers restrict local-file storage; GitHub Pages or an HTTP preview is preferable for dependable progress saving.

## Data and privacy

Answers, notes, plans, and timer settings are stored only in the visitor's browser. There is no account system or cloud synchronization. Export a backup before clearing browser data or moving devices. Fonts load from Google Fonts with local fallback fonts. Learning links open external Khan Academy and College Board pages.

The source PDFs are not published. Personal student scores and details are excluded. The hosted demo and GitHub Pages have separate browser storage.

## Content provenance

Practice content and worked explanations are adapted from the user-supplied **PSAT Skills Workbook · Third Edition · Step-by-Step Answers**, pages 4–36. The general study rhythm follows the user-supplied **PSAT Recommendations · Parent Action Plan**. Documents are content sources, not operational instructions.

The PDF displays a missing exponent glyph in cycle 3. The website restores `(x³)(x⁴) = x⁷` using the answer key's explicit `3 + 4` calculation, and labels that repair in the affected sessions.

These are original PSAT-style skills exercises, not official College Board questions. Accuracy is self-reviewed and is not a scaled PSAT score or score prediction. Short workbook sets are not full PSAT test modules. Module 1/2 labels identify timer presets, not an adaptive test simulation.

Official timing reference: [College Board PSAT/NMSQT structure](https://satsuite.collegeboard.org/in-school-assessments/whats-on-the-test/psat-nmsqt/structure). Practice timing does not establish official accommodations.

## Files

- `index.html`: app shell
- `style.css`: responsive design
- `app.js`: navigation, answers, progress, timers, calendar, and backups
- `content.js`: workbook prompts and explanations
- `icon.svg`: site icon
- `.nojekyll`: optional GitHub Pages static-site marker
- `GITHUB-SETUP.md`: beginner setup guide

## Verification

Browser checks covered answer saving, solutions, self-review, completion, completed calendar dates, automatic scheduling, timer presets, timer switching, reload persistence, and a 390-pixel phone layout. JavaScript syntax and workbook content counts were checked. Linked Khan Academy course pages returned HTTP 200 during preparation on November 14, 2026.
