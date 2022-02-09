[[Nocedal, Wright - Numerical Optimization]] page 619

A [[Series]] that fulfills [[Convergence]] can have different _convergence rates_. Examples include [[Q-linear convergence]], [[Q-superlinear convergence]] and [[Q-quadratic convergence]] convergence rates (in order of strength, quadratic being best for algorithms) as well as the slightly weaker [[R-linear convergence]].
The convergence rate typically describes how fast a solution approaches some number if the parameter moves a constant amount.

In general we can talk about an _order of convergence_ for a series $\{x_n\}$ as
$$\frac{||x_{k+1}-x^*||}{||x_k-x^*||^p}\leq M$$
for some positive constant $M$ and some order of convergence $p>1$.