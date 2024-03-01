[[Seldin, 2023 - Machine Learning The Science of Selection under Uncertaincy]]
Let $X_1, \dots, X_n$ be independent real-valued random variables such that for each $i\in \{1, \dots, n\}$ there exists $a_i \leq b_i$ such that $X_i\in [a_i, b_i]$ . Then for every $\epsilon > 0$:
$$P(\sum_{i=1}^n X_i - \mathbb{E}[\sum_{i=1}^n X_i]\geq \epsilon) \leq e^{-2\epsilon^2/\sum^n_{i=1}(b_i-a_i)^2}$$
and
$$P(\sum_{i=1}^n X_i - \mathbb{E}[\sum_{i=1}^n X_i]\leq -\epsilon) \leq e^{-2\epsilon^2/\sum^n_{i=1}(b_i-a_i)^2}$$
Taking a union bound leads to the "two-side Hoeffding Inequality"

## For $[0,1]$-bounded variables
Let $X_1, \dots, X_n$ be independent random variables, such that $X_i\in [0, 1]$ and $\mathbb{X_i} = \mu$ for all $i$, then for every $\epsilon > 0$:
$$P(\frac{1}{n}\sum_{i=1}^nX_i-\mu \geq \epsilon) \leq e^{-2n\epsilon^2}$$
and
$$P(\mu - \frac{1}{n}\sum_{i=1}^nX_i \geq \epsilon) \leq e^{-2n\epsilon^2}$$
In this case, we can regard the confidence $\delta$ (i.e. the RHS), the precision $\epsilon$ and the amount of samples $n$ as three interconnected terms that are connected. If you have two, you can compute the last one like so:
$$\delta=2e^{-n\epsilon^2}$$
$$\epsilon=\sqrt{\frac{\ln \frac{2}{\delta}}{2n}}$$
$$n=\frac{\ln \frac{2}{\delta}}{2\epsilon^2}$$
![[Pasted image 20230824143517.png]]