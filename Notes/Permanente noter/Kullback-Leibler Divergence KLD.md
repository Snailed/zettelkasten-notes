[[Bishop - Pattern Recognition and Machine Learning]]

Also called _relative entropy_

If we have an unknown distribution $p(x)$ and we approximate it with a distribution $q(x)$, then the average "data loss" for $x$ between using $p$ and $q$ is the KLD:
$$\text{KL}(p||q) = -\int p(\mathbf{x})\ln q(\mathbf{x}) d \mathbf{x} - \left( - \int p(\mathbf{x})\ln p(\mathbf{x}) d\mathbf{x} \right)$$
or 
$$\text{KL}(p||q) = -\int p(\mathbf{x})\ln \frac{q(\mathbf{x})}{p(\mathbf{x})} d \mathbf{x}$$
It is also a fact that $KL(p||q) \geq 0$ with equality if and only if $p(\mathbf{x}) = q(\mathbf{x})$
KLD is often hard to compute, so it can be better to use [[Expectation Lower Bound (ELBO)]].
KLD is related to the [[Mutual Information]]