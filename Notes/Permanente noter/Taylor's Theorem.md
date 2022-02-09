[[NO 7-2-2022]]

1D: $f\colon \mathbb{R} \rightarrow \mathbb{R}$, ($k$ + 1)-times continously differentiable: Then there is a $c\in (x, x+h)$
$$f(x+h) = f(x) + hf'(x) + \frac{h^2}{2}f''(x) + \dots + \frac{h^k}{k!}f^{(k)}(x)+\frac{h^{k+1}}{(k+1)!}f^{k+1}(c)$$
Here, the last part is a variable that changes with $x$ (should be written $c(x)$).

In several variables $f \colon U \in \mathbb{R}^n \rightarrow \mathbb{R}$, usually second order is enough
$$f(x+h)=f(x) + \nabla f(x)^Th + \frac{1}{2}h^T\nabla^2 f(x)h + o(||h||^2)$$