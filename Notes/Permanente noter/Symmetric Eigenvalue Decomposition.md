[[NO 7-2-2022]]
### Sum form
Symmetric matrix $A\in \mathbb{R}^{n\times n}, A=A^T$. It holds:
$$A=\sum_{i=1}^n\lambda_iq_iq_i^T$$
where $q_i$ are [[Eigenvector]]s that upholds
$q_i\in \mathbb{R}^n, ||q_i||=1, q_i^Tq_j=0 \text{ for }i\not = j$

### Matrix form
It is also possible to decompose a likewise matrix like so:
$$A=\sum_{i=1}^n\lambda_iq_iq_i^T=Q\Lambda Q^T$$
where
$Q\in \mathbb{R}^{n\times n}, q_i$ is $i$th column of $Q$.
$\Lambda\in \mathbb{R}^{n\times n}$ diagonal matrix with $\Lambda_{ii} = \lambda_i$
$Q$ is an orthogonal matrix