# Design Atlas v3 | Nine-week Interaction Design preparation

A responsive, dark-mode **static self-study application** designed to be hosted on GitHub Pages or opened directly from `index.html`.

## Contents

- Nine weeks, **36 expanded lessons**, definitions, worked UX examples, contrasts and common errors.
- **18 essay/research assignments** with word counts, autosaving and a manual 100-point rubric.
- **101 topic questions across nine randomised weekly question banks**, with shuffled answer order, scores and explanations.
- Short, attributed source quotations; reading links and four PDFs (see `papers/`).
- Embedded, verified educational videos (subject to YouTube allowing embedding); open-on-YouTube alternatives.
- Personal notes, practice answers, completed lessons, reading checks, quiz history and assignment scoring.
- **Export / import a full `content.json` file**, containing the course and the saved learner state.

## Local usage

Open `index.html` from this folder in a browser. Everything needed for lessons is embedded inside the HTML, so it **does not depend on fetching `content.json` locally**. If your browser allows localStorage for files, notes persist locally. Export `content.json` regularly to protect your work.

## Deploy to GitHub Pages

1. Create a repository for the site.
2. Upload the *contents* of this directory to repository root: `index.html`, `content.json`, `.nojekyll`, `papers/`, and optionally `README.md`.
3. Go to repository **Settings → Pages**; choose **Deploy from a branch**, `main`, `/ (root)`.
4. Open your published Pages URL. The site fetches repository `content.json` (and has an embedded curriculum fallback if it fails).

## Save progress in content.json via GitHub

1. Study using Design Atlas. Entries are automatically saved in your **current browser's localStorage**.
2. Go to **Your data → Download content.json**.
3. In GitHub, replace the site's `content.json` with the exported one and commit the changes.
4. Open/refresh the Pages website on your other device. On launch, the app compares the timestamps in localStorage and the repository file and takes the newer snapshot. Import exported files manually from **Your data** whenever needed.
5. If two devices edit independently, **changes are not merged**. Export before switching devices, and refresh after committing.

**Critical privacy warning:** If your GitHub Pages source repository is **public**, `content.json` is publicly downloadable. That includes your notes, essays, marks and practice answers. Never publish sensitive information this way. To keep user data private, use a separate private repository with an authenticated integration (not implemented in this static-only workflow), or use the offline JSON export/import approach without committing private notes.

GitHub Pages cannot accept direct writes from a static page. Exporting `content.json` does not itself update the GitHub repo: you must manually commit it, or add a separately authenticated backend. No GitHub token is required by this version.

## Source accuracy and copyrights

This is an independent preparation guide, **not official IIT Bombay lecture content**. Teaching text is original explanation informed by the listed resources. Short quotations are attributed to provided research papers or independently checked, freely accessible book chapters. Paid book chapters are not bundled. Embedded videos require internet access, and their owners may disable embedding.

## Updating the course

`content.json` contains the curriculum and progress. `index.html` includes an embedded *fallback copy* of the course to work with `file://`. For permanent curriculum edits, update both the JSON and the fallback HTML. Progress updates need only `content.json` because the hosted page reads it on startup.

## v3.2 update
- Revised all main action and week-card layouts for phone, tablet and desktop sizing.
- Added **Essay guide** tab with original annotated academic UX writing samples, paragraphs, revision checklist, outline editor and verified reading references.
- All existing `content.json` study content and progress fields remain compatible.

## Version 3.3 updates
- Fixed the Weekly assessment button using an explicit metrics/actions column layout.
- Expanded all 36 lessons’ glossary definitions with UX examples, application guidance and limitations.
- Export your progress with the built-in content.json export.
