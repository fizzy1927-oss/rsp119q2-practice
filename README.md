# RT Assessment Quiz Bank

A practice quiz for Intro to Respiratory Therapy, covering bedside assessment of the patient and interpretation of clinical laboratory data.

- 187 multiple-choice questions with explanations
- 8 topics: ABGs, lab values, breath sounds, chest exam & inspection, vitals & pulse ox, breathing patterns & level of consciousness, history & charting, and patient care & emergencies
- Choose topics and round length (10, 20, 50 or all questions)
- Answer choices are shuffled each round
- Missed questions are remembered in your browser so you can retry just those
- Keyboard shortcuts: A–D or 1–4 to answer, Enter for the next question

The whole site is one file, `index.html`, with nothing to install or build.

## Use it

Open `index.html` in any web browser.

## Publish it with GitHub Pages

1. Create a new public repository on GitHub.
2. Upload `index.html` and `README.md` (Add file → Upload files → Commit changes).
3. Go to **Settings → Pages**. Under "Build and deployment," set Source to **Deploy from a branch**, choose the `main` branch and the `/ (root)` folder, then click **Save**.
4. After a minute or two, the site will be live at `https://<your-username>.github.io/<repository-name>/`.

## Editing questions

Questions are in the `RAW` list inside the `<script>` in `index.html`. Each entry looks like this:

```js
["sounds", "Question text?", ["Correct answer", "Wrong", "Wrong", "Wrong"], "Explanation shown after answering."],
```

List the correct answer first; the page shuffles the choices. For combination questions ("1, 2 and 3"), the choices keep their order and the correct one is set with `{a: index, items: [...]}`, where `index` counts from 0.

Topic keys: `abg`, `labs`, `sounds`, `exam`, `vitals`, `patterns`, `history`, `care`.

## Note

These questions are a study aid built from course lecture slides and standard textbook material. They are not a substitute for your course materials. Where they differ, go with your instructor.
