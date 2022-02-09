2: Hvis du har to mængder $V$ og $W$ og trækker et tilfældigt element $x \in V\cup W$, så er sandsynligheden for at $x \in V\cap W$
$$Pr[x\in V\cap W] = \frac{|V\cap W|}{|V\cup W|} = J(V,W)$$
2: Lad $g$ være en hashfunktion fra $V\cap W \rightarrow  [M]$ for et $M\in \mathbb{Z^+}$. Lad så $H(W)=\min_{w\in W}g(w)$ altså den mindste hashværdi af alle elementerne i $W$. Nu gælder følgende:
$$Pr[H(W)=H(V)]=\frac{|V\cap W|}{|V\cup W|} = J(V,W)$$
Fedt manner! Det kan vi gøre endnu bedre. For en mængde $V$ kan vi definere en vektor $S(V)$ som er dens "summary vector" defineret som sådan:
$$S(V)=\langle H_1(V),H_2(V),\dots H_k(V)\rangle$$
Vi kan approximere to dokumenters similarity ved at sammenligne deres summary vectors.

3: Hvis man lader $d(S(V), S(W))$ være antallet af dimensioner hvor at disse er ens, så vil den forventede værdi være Jaccard similarity:
$$E[d(S(V), S(W))]=J(V,W)$$