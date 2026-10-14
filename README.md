# RSP 119 Practice Test

A study quiz for RSP 119 (patient assessment): vital signs, breathing patterns, chest inspection, chest deformities, breath sounds, labs, charting, and meds/emergencies.

- **95 questions** — the 20 from the graded quiz plus 75 bonus questions for extra exposure
- **Practice mode** shows the answer and an explanation after each question
- **Exam mode** scores you at the end, with a per-topic breakdown and a review of everything you missed
- Filter by topic, shuffle questions and answers, and retry only the ones you missed
- Works on phone and desktop, light and dark mode. One file, no installs.

## Put it on GitHub Pages

1. Create a new repository on GitHub (e.g. `rsp119-practice-test`).
2. Click **Add file → Upload files** and upload `index.html` and `README.md`. Commit.
3. Go to **Settings → Pages**. Under *Build and deployment*, set **Source** to *Deploy from a branch*, pick the **main** branch and the **/ (root)** folder, then **Save**.
4. After a minute or two your test is live at `https://<your-username>.github.io/<repo-name>/`.

You can also just double-click `index.html` to open it in a browser — no internet needed.

## Add or edit questions

All questions live near the top of the `<script>` section in `index.html`, inside `const QUESTIONS = [ ... ]`. Each one looks like this:

```js
{ cat: "Vital signs", src: "bonus",
  q: "What is the normal adult respiratory rate?",
  o: ["12–20 breaths/min", "6–10 breaths/min", "20–30 breaths/min", "60–100 breaths/min"], a: 0,
  e: "12–20 breaths/min. Above 20 is tachypnea; below 12 is bradypnea." },
```

| Field   | Meaning |
|---------|---------|
| `cat`   | Topic. A new name automatically becomes a new filter chip. |
| `src`   | `"quiz"` for questions from the graded quiz, `"bonus"` for extra practice. |
| `q`     | The question. Use `\n` for line breaks. |
| `o`     | 2–4 answer choices. |
| `a`     | Which choice is correct, **counting from 0** (0 = first, 1 = second…). |
| `e`     | Explanation shown after answering. |
| `fixed` | Optional. `true` keeps the choices in order (for "1, 3 and 4" style answers). |

Don't forget the comma after each `}`.

## Notes

- Original quiz Q13 displayed the potassium range as "5-5.0 m/eq" — the leading "3." was cut off. The correct normal range is **3.5–5.0 mEq/L**, and that's what this test uses.
- Lab reference ranges vary slightly between labs and textbooks; go with your course materials if they differ.
- Study aid only — not a substitute for your textbook or instructor.
