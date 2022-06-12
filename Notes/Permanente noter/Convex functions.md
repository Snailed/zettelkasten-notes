[[Nocedal, Wright - Numerical Optimization]] page 8

A set $S\in \mathbb{R}^n$ is _convex_ if for any two points $x, y \in S$, the line segment between the two lies entirely in $S$ e.g.
$$\alpha x + (1-\alpha)y \in S, \quad \text{ for all }\alpha \in [0,1]$$

A function $f\colon S \rightarrow \mathcal{R}$ is a _convex function_ if its domain $S$ is a convex set and if for any $x, y \in S$, the following property is satisfied:
$$f(\alpha x + (1-\alpha)y) \leq \alpha f(x) + (1-\alpha)f(y),\quad \text{ for all }\alpha \in [0,1]$$