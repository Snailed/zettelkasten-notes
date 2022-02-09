[[Nocedal, Wright - Numerical Optimization]]

A _Hessian Matrix_ is a [[Gradient]]-of-a-gradient (a matrix of second order partial derivatives)
$$
\nabla^2f(x)=
\begin{bmatrix}
\frac{\delta^2f}{\delta^2x_0^2} & 
\frac{\delta^2f}{\delta^2x_0x_1} &
\frac{\delta^2f}{\delta^2x_0x_2} &
\frac{\delta^2f}{\delta^2x_0x_3} \\
\frac{\delta^2f}{\delta^2x_1x_0^2} & 
\frac{\delta^2f}{\delta^2x_1^2} &
\frac{\delta^2f}{\delta^2x_1x_2} &
\frac{\delta^2f}{\delta^2x_1x_3} \\
\frac{\delta^2f}{\delta^2x_2x_0} & 
\frac{\delta^2f}{\delta^2x_2x_1} &
\frac{\delta^2f}{\delta^2x_2^2} &
\frac{\delta^2f}{\delta^2x_2x_3} \\
\frac{\delta^2f}{\delta^2x_3^2} & 
\frac{\delta^2f}{\delta^2x_3x_1} &
\frac{\delta^2f}{\delta^2x_3x_2} &
\frac{\delta^2f}{\delta^2x_3^2} \\
\end{bmatrix}
$$
We say that $f$ is twice differentiable on a domain $\mathcal{D}$ if $\nabla^2f(x)$ exists for all $x\in \mathcal{D}$.