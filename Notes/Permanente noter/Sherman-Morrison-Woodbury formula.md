[[Nocedal, Wright - Numerical Optimization]] page 612

If a square, [[Nonsingular matrix]] $A$ undergoes a [[Rank-one update]] update to become
$$\bar{A}= A + ab^T$$
then if $\bar{A}$ is non-singular, we have
$$\bar{A}^{-1}=A^{-1}-\frac{A^{-1}ab^TA^{-1}}{1+b^TA^{-1}a}$$

If a higher-rank update happens, then let $U,V$ be matrices in $\mathbb{R}^{n\times p}$ for $1 \leq p \leq n$. If we define
$$\hat{A}=A+UV^T$$
then $\hat{A}$ is only a [[Nonsingular matrix]] if and only if $(I+V^TA^{-1}U)$ is non-singular, and in this case, we have
$$\hat{A}^{-1}=A^{-1}-A^{-1}U(I+V^TA^{-1}U)^{-1}V^TA^{-1}$$