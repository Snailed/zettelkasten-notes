[[Bishop - Pattern Recognition and Machine Learning]] page 85

If two sets of variables are jointly following a [[Gaussian Distribution]], then the conditional distribution of one set conditioned on the other must also be Gaussian. The marginal distribution of either set is also Gaussian.

For $p(x_a|x_b)$:
$$\mu_{a|b}=\mu_a+\Sigma_{ab}\Sigma_{bb}^{-1}(x_b-\mu_b)$$
$$\Sigma_{a|b}=\Sigma_{aa}-\Sigma_{ab}\Sigma_{bb}^{-1}\Sigma_{ba}$$