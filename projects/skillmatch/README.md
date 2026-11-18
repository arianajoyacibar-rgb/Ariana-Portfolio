# SkillMatch

A browser-only résumé-to-job matcher. Paste a résumé, pick a job, get a weighted match score with matched and missing skills. A small companion to the EmploySmart capstone.

## How it works
1. **Parse**: a keyword dictionary with aliases (`js` → JavaScript) extracts skills; regex pulls years or months of experience; keywords detect education level.
2. **Score**: `total = (skills·w1 + experience·w2 + education·w3) / (w1+w2+w3)`. Required skills count fully, nice-to-haves count half.
3. **Explain**: the UI shows each component and lists the missing skills.

## Run
Open `index.html`. No build step, no dependencies.

## Limitations
Keyword matching only, so it misses synonyms outside the dictionary. Jobs are fictional.

## Ideas to extend
- Load jobs from a JSON file or REST API
- Add PDF résumé parsing
- Add unit tests for `parse()` and `score()`
