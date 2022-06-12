[[Nocedal, Wright - Numerical Optimization]] page 19

The _trust-region_ strategy, the information gathered about $f$ is used to construct a _model function_ $m_k$, whose behavior near the current point $x_k$ is similar to that of $f$.
This model function is made so it is easier to minimize, and then we assume that the minimum of the model function is close to the minimum of the actual function (think [[Taylor's Theorem]] for example).
We want to solve the following sub-problem:
$$\min_{p}m_k(x_k + p)$$
We only check $p$'s within a _trust region_ $||p||_2 \leq \Delta$ (where $\Delta$ is called the _trust region radius_), since we cannot expect our model function to be accurate as $||p||_2 > \Delta$

This strategy is opposed to the [[Line-search]] strategy