[[Nocedal, Wright - Numerical Optimization]] page 626

Consider a function $f\colon \mathbb{R}^n \rightarrow \mathbb{R}$, which is a real-valued function of $n$ independent variables. These values can be described as $x=(x_0, x_1, \dots x_{n-1})^T$.
We say that $f$ is differentiable at $x$ if there exists a vector $g\in \mathbb{R}^n$ such that
$$\lim_{y\rightarrow 0}\frac{f(x+y) - f(x_0) + g^Ty}{||y||} = 0$$
where $||y||$ is any vector norm of $y$.