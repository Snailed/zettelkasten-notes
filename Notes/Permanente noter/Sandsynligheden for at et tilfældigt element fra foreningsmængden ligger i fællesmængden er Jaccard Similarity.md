Reference: [[Vassilvitskii, Sergey - Dealing with Massive Data]]

Hvis du har to mængder $V$ og $W$ og trækker et tilfældigt element $x \in V\cup W$, så er sandsynligheden for at $x \in V\cap W$
$$Pr[x\in V\cap W] = \frac{|V\cap W|}{|V\cup W|} = J(V,W)$$
hvor $J(V,W)$ er [[Jaccard Similarity]].
Dette bruges i [[MinHash]].