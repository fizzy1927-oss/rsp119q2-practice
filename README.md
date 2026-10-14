# RC Pharm Exam Prep

A single-page study site for Respiratory Care Pharmacology:

- **Mucus-Controlling Drug Therapy** — bland aerosols, mucolytics (NAC, dornase alfa), CFTR modulators / Trikafta dosing
- **Corticosteroids & Anti-asthmatics** — HPA axis, ICS vs OCS, side effects, leukotriene modifiers
- **Calculating Drug Doses** — % ↔ mg/ml, proportions, weight-based dosing

## Features
- **Quiz** — filter by topic or learning objective; Practice mode (instant feedback) or Exam mode (score at the end, per-objective breakdown, review of misses). Missed questions are remembered for a "missed only" retake.
- **Cases** — 9 multi-step patient scenarios.
- **Calc drill** — unlimited randomized calculation problems with worked solutions.
- **Terms** — searchable key-term flashcards.

Progress is stored in the browser's localStorage. No build step, no dependencies.

## Publish on GitHub Pages
1. Create a new repository and upload `index.html` (and this README) to the root.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, then **Save**.
4. After a minute, your site is live at `https://<your-username>.github.io/<repo-name>/`.

## Editing questions
All content lives in the `Q`, `CASES`, and `TERMS` arrays near the top of the `<script>` in `index.html`. In each question, the **first** choice is the correct answer — choices are shuffled on screen.

*Study aid based on course lecture slides; not clinical guidance.*
