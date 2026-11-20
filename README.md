# Math Notes — Single-Worksheet Website

**Website:** https://prototyp037.github.io/24IsTheAnswerToLife/

This is a single-page, dark-themed GitHub Pages site. It always displays solutions to **only the most recently uploaded worksheet**.

## Current state

The website is intentionally **empty** and displays "Ready for the next worksheet". Previous questions and solutions have been removed from the current site (though older versions may still exist in public Git history).

## Rules for the next update

1. Completely **replace** the current page contents for each new photo. Do **not** retain or append earlier worksheets.
2. Write the full questions, answers, and step-by-step solutions from the new sheet only.
3. Place **every problem in a single vertical flow**, with successive HTML section elements using the class "question" in [index.html](index.html). Do not use tabs or carousels.
4. Keep the current **dark theme** and mobile-friendly layout for narrow rectangular screens.
5. Avoid horizontal scrolling. Use MathJax v4's **automatic equation line breaking** (with output.displayOverflow set to linebreak), and manually split exceptionally wide matrices, tables, or aligned expressions into smaller steps if necessary. The goal is vertical scrolling only.
6. Push changes to the existing main branch so the **same link** always displays the newest worksheet.
7. Do not publish names, student IDs, or other personal data visible in uploaded photos.

## Technology

- Static HTML + CSS with no build process, in [index.html](index.html)
- Dark, responsive stylesheet
- MathJax 4 (tex-chtml.js) for LaTeX, with automatic line breaking configured
- GitHub Pages via main / (root), using [.nojekyll](.nojekyll)
- HTTPS website: https://prototyp037.github.io/24IsTheAnswerToLife/

### Hosting

If the site is not yet published, enable GitHub Pages in [Settings → Pages](https://github.com/prototyp037/24IsTheAnswerToLife/settings/pages), select **Deploy from a branch**, main, and /(root).

Because the repository is public, previous versions can remain visible in commit history even after the current page has been overwritten.
