[[NO 7-2-2022]]

Every vector norm (e.g. [[Manhattan norm]], [[Euclidian norm]], [[Infinity norm]]) induces a matrix norm. Let $A\in \mathbb{R}^{n\times m}$ be a matrix and $x\in \mathbb{R}^m$. We define for any vector-norm $||\cdot ||$:
$$||A|| = \max_{||x|| \leq 1}\frac{||Ax||}{||x||}$$

For $||\cdot ||_2$ holds:
$$||A||_2 = \sqrt{\sigma_1(AA^T)}$$

If $A$ is a symmetric PSD:
$$||A||_2=\sigma_1(A)$$