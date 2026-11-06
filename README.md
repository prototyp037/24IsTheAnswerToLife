# 24IsTheAnswerToLife

## Eigenvector embedding of a word

### Question

If $V = [v_1, v_2, \ldots, v_c]$ is the eigenvector matrix of the word co-occurrence matrix $C$, what is the eigenvector embedding of word $e_i$?

### Answer

**Take the $i$-th row of $V$.** Equivalently, when the embedding is written as a column vector,

$$
\boxed{\operatorname{embed}(e_i) = V^\top e_i =
\begin{bmatrix}
(v_1)_i \\
(v_2)_i \\
\vdots \\
(v_c)_i
\end{bmatrix}}
$$

Here:

- $v_1,\ldots,v_c$ are the **columns** of $V$ (the eigenvectors of $C$).
- $e_i$ denotes the **one-hot vector** for word $i$.
- $(v_j)_i$ is the $i$-th entry of eigenvector $v_j$.

### Why?

The eigenvectors form an orthonormal basis for a real symmetric co-occurrence matrix. The embedding records the coordinates of word $i$ along each eigenvector: its entries across the $i$-th row of $V$.

If only $k$ eigenvectors are retained for a $k$-dimensional embedding, use $V_k = [v_1,\ldots,v_k]$:

$$
\operatorname{embed}_k(e_i) = V_k^\top e_i \in \mathbb{R}^k.
$$

**Takeaway:** Columns of $V$ are eigenvectors; **rows of $V$ are word embeddings**. This question asks for the eigenvector-only embedding, without additional eigenvalue weighting.
