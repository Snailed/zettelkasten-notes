Reference: [[Vassilvitskii, Sergey - Dealing with Massive Data]], [[Dahlgaard, Knudsen, Thorup - Fast Similarity Sketching]]

MinHash er en metode til foretage [[Approximeret Jaccard Similarity Searching]]. 
[[Sandsynligheden for at et tilfældigt element fra foreningsmængden ligger i fællesmængden er Jaccard Similarity]].
Lad $g$ være en hashfunktion fra $V\cap W \rightarrow  [M]$ for et $M\in \mathbb{Z^+}$. Lad så $H(W)=\min_{w\in W}g(w)$ altså den mindste hashværdi af alle elementerne i $W$. Nu gælder følgende:
$$Pr[H(W)=H(V)]=\frac{|V\cap W|}{|V\cup W|} = J(V,W)$$
[[MinHash "sketcher" data ved at lave en summary vektor med værdier fra tilfældige hashfunktioner]]
Hvis man lader $d(S(V), S(W))$ være antallet af dimensioner hvor at disse er ens, så vil den forventede værdi være Jaccard similarity:
$$E[d(S(V), S(W))]=J(V,W)$$

[[MinHash kører i O(t*A) tid]]*, hvilket er langsommere end [[Fast Similarity Sketching]]