# Math Quick Notes

A compact, mobile-first **GitHub Pages** website for short mathematical explanations with rendered LaTeX. Designed for narrow rectangular screens, including small phones and landscape orientation.

**Website:** https://prototyp037.github.io/24IsTheAnswerToLife/

## Questions

The website has four selectable tabs:

1. **Q1 — Hessian test:** The minimum **could** occur at \(b\), since its Hessian \(2I\) is positive definite; \(a\) and \(c\) are saddle points.
2. **Q2 — Changing integration order:** \(\displaystyle \int_0^1\int_{x^2}^1\frac{\sqrt y}{1+y^2}\,dy\,dx=\frac{\ln 2}{2}\).
3. **Q3 — Closest point on a surface:** \(\displaystyle \left(\pm\frac{\sqrt{26}}6,0,\frac13\right)\), each at distance \(\sqrt{5/6}\) from the origin.
4. **Eigenvectors (previous question):** \(\operatorname{embed}(e_i)=e_i^\top V\), the \(i\)-th row of \(V\).

The website includes worked solutions and mathematical reasoning. Names and student IDs from the source photo are intentionally excluded.

## Design

- Responsive CSS for narrow phones and short landscape displays
- One question visible at a time; tappable, keyboard-accessible tabs
- Horizontally scrollable equations (no whole-page horizontal overflow)
- MathJax 3 for browser-rendered LaTeX, loaded from jsDelivr
- Plain HTML, CSS, and JavaScript — no build tools needed

## Publish with HTTPS

If GitHub Pages is not already active:

1. Open [Settings → Pages](https://github.com/prototyp037/24IsTheAnswerToLife/settings/pages).
2. Under **Build and deployment**, select **Deploy from a branch**.
3. Set branch to **main** and folder to **/(root)**.
4. Save. GitHub provides HTTPS hosting at the website URL above.

Edit [index.html](index.html) to change questions and layout. The [.nojekyll](.nojekyll) file disables Jekyll processing.
