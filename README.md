# PSAT Path

Small steps. Stronger skills.

An interactive PSAT/SAT study path with 120 sessions, five original practice exams, automatic grading, targeted practice plans, worked equations, optional 1.5x timers, and a study calendar.

## Features

- 8 learning cycles and 24 sessions: math, reading, and a 10-word vocabulary set with a review test in each cycle.
- 48 workbook math/reading questions with four options, checking, elimination tools, and worked explanations; 80 vocabulary review questions across the eight cycle sets.
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

The multiple-choice options and answer keys are newly authored adaptations of the supplied workbook. The eight former Mixed sessions are replaced by vocabulary sessions. Earlier written responses and their existing completion/review data are preserved; choosing a new option reopens that session for review. The tips tab links to College Board sources.

## Reading length update

The eight reading samples have been expanded into original practice passages, used in the eight reading sessions. Word counts are displayed in the workbook. Every passage falls within the current digital SAT range of 25–150 ordinary words, and also within the framework’s technical six-character word range. These are adaptations, not copied official passages. The workbook retains three questions per shared text; the digital SAT uses one question per passage or passage pair. Length alignment does not establish equivalent exam difficulty. Questions, options, and evidence references were reviewed for consistency; previously saved progress remains available.

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

Choose **SAT vocabulary** in the navigation menu, or open `#vocabulary`. The bank contains 200 selected words in 20 sets of 10, drawn from single-word answer choices and target words in Words in Context questions in College Board’s released SAT Practice Tests 4–11. Every card includes its source test, PDF page number, printed form when different, and a direct source link. Correct and incorrect options are both included as vocabulary study material. Sources: [official practice library](https://satsuite.collegeboard.org/practice/practice-tests/paper), and the individual `sat-practice-test-N-digital.pdf` files linked on each card. Reviewed November 15, 2026.

The words appearing in more of these eight files come first; inflected forms are grouped where appropriate. Counts are limited to this corpus and do not measure live SAT frequency. This is a selected study list, not every commonly used SAT word or an official College Board vocabulary bank. Each card gives one original definition, part of speech, and original example sentence. The source verifies the word’s appearance, not the card’s wording or whether that option was correct. College Board emphasizes meaning in context; see its [assessment framework](https://satsuite.collegeboard.org/media/pdf/assessment-framework-for-digital-sat-suite.pdf#page=142).

Click or keyboard-activate the card to flip between the word and its meaning/example. Mark it known or needing practice if useful. Search opens any word directly. Flip all ten cards in a set to unlock its ten-question multiple-choice meaning-in-context quiz. Each word appears once. Submission shows exact correct totals and explanations; missed words have a dedicated card-review path. Retakes shuffle questions and choices while keeping best scores. Related meanings are excluded from one another’s distractors within a set. Ratings and quiz completion record practice, not lasting mastery or an official SAT score.

Required files are `vocabulary-data.js`, `vocabulary.js`, and `vocabulary.css`. The revised deck uses localStorage `psat-path-vocabulary-sat-words-v2`, with a separate demo suffix. On first use it carries over reviewed status and ratings for exact matching words from the previous 400-word deck. Previous quiz scores remain in a separate history because the quiz groups changed; new quiz groups start fresh. The earlier store remains untouched. Version 1 vocabulary backups can also be imported with this migration. Version 2 backups retain the deck identifier and history. Backups without vocabulary preserve the existing store. Published word order is a stable identifier within this deck.

Checks cover 200 unique cards and matching example words, all card sources against the extracted question choices/targets and PDF page text, corpus recurrence ordering, 100 deterministic quiz variants, correct/incorrect grading, ten-card gating, missed-word review, retakes, next sets, exact-word legacy migration, separate prior score history, and backup round trips. Browser verification covers card flipping, source links, quizzes, saved results, search, and a phone layout.

## Vocabulary cycles and pronunciation update

Session C in each of the eight original cycles is now vocabulary. Each session uses one of the first eight stable sets in the SAT vocabulary library: ten flashcards followed by a ten-question multiple-choice review test. The dedicated Vocabulary tab and SAT vocabulary page share the same answers, scores, and reviewed status. The remaining twelve sets are extra practice. There are still 24 sessions before Exam 1.

Grading a cycle vocabulary test automatically completes its C session. Its saved date contributes to the study calendar, completion count, and first-exam unlock. Best vocabulary scores contribute to practice accuracy; starting a retake does not erase session completion. Exact word order and the 200-word deck identifier are unchanged. A `completedAt` date is now included in vocabulary records and their backups. Existing submitted vocabulary tests supply their actual completion date.

The workbook store includes `vocabularyRevision: 1` and `legacyMixed` archives. Earlier C-session responses, choices, notes, grades, dates, and flags are moved into that archive rather than applied to the new vocabulary work. Math and reading records, plans, and completed SAT exams are retained. Older workbook backups are migrated on import; normal JSON export includes archived work and vocabulary results. Earlier mixed completion does not count as completion of a new vocabulary test.

Every word has Hear word, Slower, and Hear example buttons, with word audio also in quizzes and all three in explanations. Recommended voice selection favors available neural/natural/enhanced English voices, then established English voices such as Samantha; novelty voices are penalized. A Reading voice picker lets the student choose among available English voices, with the preference saved on that device. Voice availability and quality depend on the browser and installed voices. Playback is still synthesized speech, not a human recording.

Normal speech requests rate 1; Slower requests 0.45. Playback cancels the earlier request, resumes a paused engine, and allows a 100 ms cancellation interval before starting a new utterance. This avoids the immediate cancel/speak restart that can lose a slower-playback request. Stop, navigation, hidden tabs, imports, and submission cancel playback. Unsupported or failing speech has a dictionary fallback. Listening does not mark definitions reviewed. No microphone, API key, or audio backend is needed.

Verified in the browser on November 15, 2026: Recommended selects Samantha, and the same word (commercialization) measured 1,286 ms at normal speed versus 1,657 ms with Slower. Browser timings vary and the synthesis rate is not a promise of a linear speed ratio. Tests cover all 200 words, voice ranking, queued restart cancellation, progress migration, shared cycle tests, completion dates, retakes, backups, and the 24-session exam gate.
