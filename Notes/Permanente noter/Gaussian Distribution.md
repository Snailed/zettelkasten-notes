[[Bishop - Pattern Recognition and Machine Learning]]

In case of a single variable $x$, the Gaussian distribution can be written in the form
$$\mathcal{N}(x|\mu, \sigma^2)=\frac{1}{(2\pi \sigma^2)^{1/2}}\exp{\{-\frac{1}{2\sigma^2}(x-\mu)^2\}}$$
where $\mu$ is the mean and $\sigma^2$ is the variance

For a $D$ dimensional vector $x$, the multivariate gaussian distribution can be written in the form
$$\mathcal{N}(x|\mu, \Sigma)=\frac{1}{(2\pi)^{D/2}}\frac{1}{(\det\Sigma)^{1/2}}\exp{\{\frac{1}{2}(x-\mu)^T\sigma^{-1}(x-\mu)\}}$$
where $\mu$ is the D-dimensional mean vector and $\Sigma$ is the $D\times D$ co-variance matrix.

[[Conditional Gaussian Distributions]]