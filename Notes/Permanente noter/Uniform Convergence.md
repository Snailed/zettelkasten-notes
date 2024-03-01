[[Yehudayoff, 2023 - ATML Lecture Notes]]
A class $H$ satisfies uniform convergence if the probability of the difference between the [[Population loss]] and the [[Empirical Loss]] is less than $\epsilon > 0$ with a probability of at least $1-\delta$
$$P[\forall h \in H \colon \mathbb{E}_{S_{\mu^n}}[|L_\mu(h) - L_S(h)|] < \epsilon] > 1 - \delta$$
If a class $H$ satisfies uniform convergence, then any [[Empirical Loss]] minimizer learns $H$.