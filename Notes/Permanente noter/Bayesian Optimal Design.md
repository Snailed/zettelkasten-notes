[[Ryan, 2015 - A Review of Modern Computational Algorithms for Bayesian Optimal Design]]

A kind of [[Experimental Design]] that utilizes [[Bayes Theorem]] to incorporate [[Prior distribution]]s that can encode information from previous studies, expert elicited data or subjective beliefs from the experimenters.

Prior information is ignored when performing analysis on the data gained from these experiments.

Ryan, 2015, distinguishes between designs that have arisen from "just" encorporating probability distributions and averages on the parameters to "fully" Bayesian designs where the design criterion is a functional of the posterior distribution.

The optimal design, $\mathbf{d}^*$, maximises the expected utility function $U(\mathbf{d})$ (where $U$ is the [[Design Criterion]]) over the design space $\mathbf{D}$ with respect to the future data $\mathbf{y}$ and model parameters $\mathbf{\theta}$.
![[Pasted image 20230421115623.png]]

Thus, the Bayesian optimal design $\mathbf{d}^*$ maximises the posterior expected utility. This equation does not usually have a closed form solution however, so numerical approximations or stochastic solutions are nescessary to solve the maximisation / integration problem.

The predictive prior is $p(\mathbf{y}, \theta | \mathbf{d}) = p(\mathbf{y}|\mathbf{d}, \theta)p(\theta)$ according to Ryan. This can be read as "the possibility of achieving data $\mathbf{y}$ and parameters $\theta$ when using design $\mathbf{d}$"