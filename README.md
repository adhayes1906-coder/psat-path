# PSAT Path

Small steps. Stronger skills.

An interactive PSAT/SAT study path with 120 sessions, five original practice exams, automatic grading, targeted practice plans, worked equations, optional 1.5x timers, and a study calendar.

## Features

- 8 learning cycles and 24 sessions from the supplied Third Edition workbook.
- 64 multiple-choice practice questions with four options each, automatic checking, and an option eliminator, 8 unscored memory checks, and worked explanations for all 72 prompts.
- Step-by-step equations with formatted fractions, powers, square roots, and final answers in every math solution.
- Longer original reading texts within the digital SAT passage-length range, with visible word counts.
- Separate Questions, Answers & solutions, Learn more, and Multiple-choice tips tabs.
- Four independent, optional module timer presets: Reading & Writing 1/2 at 48:00; Math 1/2 at 52:30.
- Saved answers, checked-answer accuracy, session completion, K/F/U/T/G tags, reflections, and a revisit list.
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

These are original PSAT-style skills exercises, not official College Board questions. Accuracy combines automatically checked multiple-choice selections with preserved reviews of earlier written responses and is not a scaled PSAT score or score prediction. Short workbook sets are not full PSAT test modules. Module 1/2 labels identify timer presets, not an adaptive test simulation.

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

The multiple-choice options and answer keys are newly authored adaptations of the supplied workbook. The eight memory checks remain open-ended. Earlier written responses and their existing completion/review data are preserved; choosing a new option reopens that session for review. The tips tab links to College Board sources.

## Reading length update

The eight reading samples have been expanded into original practice passages, also used in the matching mixed reviews. Word counts are displayed in the workbook. Every passage falls within the current digital SAT range of 25–150 ordinary words, and also within the framework’s technical six-character word range. These are adaptations, not copied official passages. The workbook retains three questions per shared text; the digital SAT uses one question per passage or passage pair. Length alignment does not establish equivalent exam difficulty. Questions, options, and evidence references were reviewed for consistency; previously saved progress remains available.

Source: [College Board SAT Reading and Writing](https://satsuite.collegeboard.org/sat/whats-on-the-test/reading-writing).


## Five-round SAT path

The existing 24 sessions form round 1. Finishing all 24 unlocks the first original full-length practice exam. Each exam has 54 Reading & Writing questions and 44 Math questions in four modules (27/27/22/22). Optional module timers are 48/48/52.5/52.5 minutes, with a 10-minute between-section break. Answers save locally, previous modules lock, and solutions are available after submitting the whole exam.

Grading reports exact raw correct totals and percentages overall and for both sections, plus 29 skill-level results. Blanks count as incorrect. There is no fabricated scaled SAT score. Optional official Bluebook section scores are user-entered, validated 200–800 in increments of 10, and summed separately.

After each of exams 1–4, the next 24 sessions are generated deterministically from the missed and unanswered skill profile. Priority combines error rate and missed count with diminishing allocation, while reserving practice in both subjects. Each session has two focus items, one secondary item, and one maintenance item; four questions total. A perfect result produces rotating review. Rounds 2–5 include worked MathML equations, explanations, resource links, multiple-choice tips, completion tracking, and calendar scheduling. Exam 5 ends the sequence.

These original forms are fixed, nonadaptive, and uncalibrated. Repeated question families use different parameters and fictional scenarios. Matching counts, broad domains, and 25–150-word passage lengths does not establish official SAT difficulty, blueprint equivalence, or a valid scaled score. All Math items use multiple choice, whereas the official SAT also includes student-produced responses. Official practice: https://satsuite.collegeboard.org/practice/practice-tests/bluebook

New source files: `sat-bank.js` (content, grading, targeting), `sat-path.js` (journey and exam UI), `sat-path.css` (responsive layouts). Journey data uses a separate localStorage key, `psat-path-journey-v1`; the original workbook remains compatible. Demo storage is isolated and clearly labeled hypothetical. JSON export/import includes both stores. Import pauses timers; ordinary reloads preserve running exam countdowns. No server, API key, account, or backend generation is required.

Primary references: [SAT structure](https://satsuite.collegeboard.org/sat/whats-on-the-test/structure), [Reading & Writing format](https://satsuite.collegeboard.org/sat/whats-on-the-test/reading-writing), [Official scoring](https://satsuite.collegeboard.org/scores/what-scores-mean/how-scores-calculated).


## Reading review and quick tips (November 15, 2026)

A dedicated Reading quick tips page and session tab provide a question-first routine, seven skill-specific guides, flexible 1.5x pacing, an unscored example with a revealable explanation, a checklist, and official practice links. The same content is available in the original workbook and targeted follow-up sessions.

The comparison with College Board’s current format and official digital SAT samples confirms similar skills and some format features, not equivalent exam difficulty. Workbook passages remain 106–115 words with three questions per reading text; practice-form texts remain 60–103 words with one question per text or pair. The existing exam generator uses a narrower range of fictional scenarios and repeated templates; it does not reproduce the full literary/subject variety, skill grouping, difficulty order, or adaptive routing of the SAT. These limits are disclosed in the new tab. No existing question, answer key, item order, or stored-progress format was changed.

`reading-tips.js` is required alongside the existing website files. Sources: [Reading & Writing format](https://satsuite.collegeboard.org/sat/whats-on-the-test/reading-writing), [official sample questions](https://satsuite.collegeboard.org/media/pdf/digital-sat-sample-questions.pdf), and [College Board pacing and test-taking tips](https://blog.collegeboard.org/top-10-test-taking-tips-digital-sat).


## Vocabulary studio

Choose **SAT vocabulary** in the navigation menu, or open `#vocabulary`. The curated bank contains 400 academic words in 40 sets of 10, with an original definition, part of speech, and example sentence for each. Click or keyboard-activate the card to flip between the word and its meaning/example; optionally mark it known or needing practice. Search opens any word directly.

Flip all ten cards in a set to unlock its ten-question multiple-choice meaning-in-context quiz. Each word appears once. Submission shows exact correct totals and explanations; missed words have a dedicated card-review path. Retakes shuffle questions and choices, while best scores remain saved. Other sets can be studied in any order. Ratings and quiz completion are practice records, not a claim of lasting mastery or an official SAT score.

There is no claim that this bank includes every commonly used word or every word a student might see on the SAT. It is not an official or frequency-ranked SAT list. College Board’s vocabulary framework emphasizes contextual meanings and notes that word tiers are not universal static banks. Definitions and examples here are originally written instructional material; one academic sense is shown per word, with familiar words’ less familiar meanings included. Source for the scope explanation: https://satsuite.collegeboard.org/media/pdf/assessment-framework-for-digital-sat-suite.pdf (PDF page 142).

Required new files are `vocabulary-data.js`, `vocabulary.js`, and `vocabulary.css`. Vocabulary progress uses localStorage `psat-path-vocabulary-v1` with a separate demo suffix. Core JSON backup export/import includes the vocabulary store, alongside the original workbook and SAT path. Older backups without vocabulary fields preserve the existing vocabulary store. Sets and word order are stable identifiers; append new sets rather than reordering published content.

Checks cover all 400 unique entries and their example-word matches, 200 deterministic quiz variants, correct/incorrect grading, ten-card gating, missed-word review, retakes, next sets, storage validation, and backup round trips. Browser verification covers card flipping, quizzes, saved results, and search.
