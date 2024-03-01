[[Yehudayoff, 2023 - ATML Lecture Notes]]
Like [[PAC Learnability]], but relaxes the restriction that $L_\mu(H) = 0$:
A class $H$ is PAC learnable in the agnostic setting if for every $\epsilon > 0$ there is an algorithm $A$ with a sample size $n$ such that for all $\mu$,
$$L_\mu(A) < \epsilon + L_{\mu}(H)$$