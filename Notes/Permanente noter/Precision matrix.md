[[Bishop - Pattern Recognition and Machine Learning]] page 85

If you partition $x$ in a multivariate [[Gaussian Distribution]]:
$$x=\begin{pmatrix}x_a \\ x_b\end{pmatrix}$$
and $\mu$:
$$\mu=\begin{pmatrix}\mu_a \\ \mu_b\end{pmatrix}$$
you can get $\Sigma$:
$$\Sigma=\begin{bmatrix}\Sigma_{aa} & \Sigma_{ab} \\ \Sigma_{ba} & \Sigma_{bb}\end{bmatrix}$$

The inverse of $\Sigma$ is known as the _precision matrix_. It can be partitioned as well:
$$\Lambda=\begin{bmatrix}\Lambda_{aa} & \Lambda_{ab} \\ \Lambda_{ba} & \Lambda_{bb}\end{bmatrix}$$

**Important:** $\Sigma_{aa}$  is not nescessarily the same as $\Lambda_{aa}$