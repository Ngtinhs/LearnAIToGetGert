# T-Study — Claude Certification Practice

A static HTML/CSS/JavaScript study site containing the four Claude courses extracted from the supplied T-Study archive.

## Courses and source question counts

- CCAR-P — Claude Certified Architect – Professional: 166 questions
- CCAF — Claude Certified Architect – Foundations: 175 questions
- CCDV-F — Claude Certified Developer – Foundations: 110 questions
- CCAO-F — Claude Certified Associate – Foundations: 169 questions

Total: 620 questions.

## Features

- Four-course dashboard and course search
- Practice mode with single-choice, multiple-choice, true/false, and matching questions
- Check answer and reveal answer with the source explanation and per-option explanations
- Review answers mode
- Quiz mode with randomized questions and score review
- Question navigation and filters for all, to learn, learned, incorrect, and saved
- Local progress persistence via browser LocalStorage
- JSON question banks in `data/`

## Run locally

Because the app fetches JSON files, open it through a local static server rather than `file://`.

```bash
python -m http.server 8000
```

Then open http://localhost:8000.

## Deploy to Vercel

Import this folder/repository into Vercel as a static site. No build command is required; set the output directory to `.` (the project root).

## Data

The JSON files preserve the course objects and question content, answer keys, explanations, option explanations, and review/source metadata from the supplied archive. Progress is stored in the current browser only; it is not synced across devices.
