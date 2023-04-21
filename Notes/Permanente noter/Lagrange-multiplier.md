[[Khan Academy, Multivariable Calculus]]

A useful strategy for dealing with equality-contraint optimization problems of the form

> "Optimize $f$ with regards to $x$ such that $g(x, y, z, \dots) = c$"

By restricting our search space to points where the tangent lines of $f$ and $g$ are tangent to eachother, we are guaranteed that any minumum found will satisfy the constrait.

This is done by introducing a **Lagrange multiplier** $\lambda$ in the following formula:
$$\mathcal{L}(x, y, z, \dots, \lambda) = f(x,y,z,\dots) - \lambda g(x, y, z, \dots )$$
Where $\mathcal{L}$ is called the _Lagrangian_.
Consider the [[Gradient]] of the Lagrangian and optimize to find the critical points. The critical point that evaluates to the smallest number is then the minimum.