[[Nocedal, Wright - Numerical Optimization]] page 599

A square matrix $A$ is _positive definite_ if there exists a positive scalar $\alpha$ such that
$$x^TAx \geq \alpha x^Tx\quad \text{for all}\ x\in \mathbb{R}^n$$

It is _positive semi-definite_ if
$$x^TAx\geq 0\quad \text{for all}\ x\in \mathbb{R}^n$$


If $x$ is a vector that points in a direction, and is transformed by a PD matrix $A$, then it will still point in its general direction (the angle change won't be larger than 90 degrees ($\pi /2$)).
If it is transformed by a PSD matrix, then the angle change will be 90 degrees or lower (non-strict bound).

If a matrix is positive definite and symmetric, then its [[Eigenvalue]]s will be positive real numbers.