Reference: [[Indyk, Motwani - Approximate Nearest Neighbors Towards Removing the Curse of Dimensionality]] [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]]

En familie af hashfunktioner $\mathcal{H}=\{h:X\rightarrow U\}$ bliver kaldt for $(r_1, r_2, p_1, p_2)$-sensitive for $D$ hvis for enhver $x,y\in X$ og en uniformt tilfældigt valgt $h \in \mathcal{H}$:
- hvis $S(x,y) \geq s_1$, så må $Pr_\mathcal{H}[h(x)=h(y)]\geq p_1$
- hvis $S(x,y) \leq s_2$, så må $Pr_\mathcal{H}[h(x)=h(y)]\leq p_2$

Her bruger vi en afstandsfunktion $S:Y\rightarrow [0;1]$
Når $D$ er en *similarity measure*, så er det kun nyttigt når $p_1 > p_2$ og $r_1 > r_2$.

Et eksempel på en $(r_1, r_2, p_1, p_2)$-sensitiv familie af hashfunktioner er [[MinHash]].

