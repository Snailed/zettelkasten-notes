[[Nocedal, Wright - Numerical Optimization]] page 22

A way of finding $p_k$ in a [[Line-search]] algorithm.
It is derived from the second-order [[Taylor's Theorem]] series approximation to $f(x_k + p)$ defined as $m_k(p)$

By simply setting the derivative of $m_k(p)$ to zero, we obtain the following explicit formula:
$$p_k^N = -(\nabla^2f_k)^{-1}\nabla f_k$$