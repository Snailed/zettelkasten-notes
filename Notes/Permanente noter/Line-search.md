[[Nocedal, Wright - Numerical Optimization]] page 19

The _Line-search_ strategy for optimization, the algorithm chooses a direction $p_k$ and searches along this direction from the current iterate $x_k$ for a new iterate with a lower function value.
Finding the step length $\alpha$ is in itself a minimization problem, that tries to solve
$$\min_{\alpha > 0}f(x_k + \alpha p_k)$$

This strategy is opposed to the [[Trust-region]] strategy