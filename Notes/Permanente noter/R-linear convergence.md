[[Nocedal, Wright - Numerical Optimization]] page 620

_R-linear_ [[Convergence]] is slightly weaker than [[Q-quadratic convergence]]. This [[Convergence rate]] is concerned with the overall error of the algorithm instead of the error over each step.

We say that convergence is _R-linear_ if there exists a sequence of nonnegative scalars $\{v_k\}$ such that
$$||x_k-x^*||\leq v_k\quad \text{for all }k\text{, and }\{v_k\}\text{ converges Q-linearly to zero.}$$
We can say that $\{||x_k-x^*||\}$ is _dominated_ by $\{v_k\}$