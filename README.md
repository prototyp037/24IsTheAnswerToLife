# Math Quick Notes

A mobile-first [GitHub Pages](https://pages.github.com/) website of worked calculus and AI questions, with LaTeX rendered by [MathJax](https://www.mathjax.org/). Designed for narrow rectangular screens.

**Website:** https://prototyp037.github.io/24IsTheAnswerToLife/

## Latest sheet — three new questions

Select the **New 1**, **New 2**, or **New 3** tabs to see full derivations:

| Question | Answer |
|---|---|
| **New 1 — Average value** | $\displaystyle \frac{46}{3\left(2\sqrt5+9\arcsin(2/3)\right)}\approx1.389$ |
| **New 2 — Vector field** | **Circulation negative; flux positive** for the counterclockwise rectangular path and field shown |
| **New 3(a) — Exact 1-form** | $B=C=0$ |
| **New 3(b) — Potential** | $\displaystyle f(x,y)=\frac{x^2}{2}+\frac{y^3}{3}+K$ |

The question text is transcribed from the supplied sheet, and a compact, schematic vector-field illustration helps explain the circulation and flux. No personal identifiers from the sheet are published.

## Earlier questions (still available)

- **Old 1 — Hessian test:** The minimum could occur at $b$, since $D^2 f(b)=2I$ is positive definite, while $a$ and $c$ are saddles.
- **Old 2 — Changing integration order:** $\displaystyle \int_0^1\int_{x^2}^1\frac{\sqrt y}{1+y^2}\,dy\,dx=\frac{\ln2}{2}$.
- **Old 3 — Closest point:** $\displaystyle \left(\pm\frac{\sqrt{26}}6,0,\frac13\right)$, each at distance $\sqrt{5/6}$.
- **Eigenvectors:** $\operatorname{embed}(e_i)=e_i^\top V$, the $i$-th row of $V$.

## Using the site

- Tap a tab to show one problem; **swipe the horizontal tab row** to access other problems.
- The new sheet opens by default. Direct links: [New 1](https://prototyp037.github.io/24IsTheAnswerToLife/#s2q1), [New 2](https://prototyp037.github.io/24IsTheAnswerToLife/#s2q2), [New 3](https://prototyp037.github.io/24IsTheAnswerToLife/#s2q3).
- Equations are scrollable within their own boxes, so large formulas won't widen the entire page.
- The website is static HTML, CSS, and JavaScript in [index.html](index.html). No build system required.
- MathJax is loaded from jsDelivr and requires an internet connection.

## GitHub Pages (HTTPS)

If Pages isn't enabled: open [Settings → Pages](https://github.com/prototyp037/24IsTheAnswerToLife/settings/pages), select **Deploy from a branch**, choose **main** and **/(root)**, then save. The [.nojekyll](.nojekyll) file disables Jekyll preprocessing.
