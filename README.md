# Eigenvector Word Embeddings

A small, responsive website explaining eigenvector-based word embeddings with rendered LaTeX, a derivation, and a worked example.

**Website (GitHub Pages):** https://prototyp037.github.io/24IsTheAnswerToLife/

> The website address becomes active after GitHub Pages is enabled in the repository settings.

## Answer

If \(V=[v_1,v_2,\ldots,v_c]\) contains the chosen eigenvectors of a co-occurrence matrix as its **columns**, then the embedding for word \(e_i\) is the **\(i\)-th row** of \(V\):

$$
\operatorname{embedding}(e_i)
=e_i^\top V
=\begin{bmatrix}(v_1)_i & (v_2)_i & \cdots & (v_c)_i\end{bmatrix}.
$$

If word embeddings are represented as column vectors, this is equivalently \(V^\top e_i\).

## Publish the website

This is a no-build static site. To enable HTTPS hosting:

1. Open [Settings → Pages](https://github.com/prototyp037/24IsTheAnswerToLife/settings/pages).
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select **main**, choose **/(root)**, and click **Save**.
4. Open the [live website](https://prototyp037.github.io/24IsTheAnswerToLife/) after GitHub deploys it.

The site uses [MathJax](https://www.mathjax.org/) from a CDN to render LaTeX in the browser. Edit [index.html](index.html) to change website content. No npm dependencies or local build commands are needed.

## Files

- [index.html](index.html) — complete responsive website and math content
- [.nojekyll](.nojekyll) — instructs GitHub Pages to serve the site without Jekyll processing
- [README.md](README.md) — overview and hosting instructions
