Reference: [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]], [[Indyk, Motwani - Approximate Nearest Neighbors Towards Removing the Curse of Dimensionality]]

Det klassiske LSH-framework kan løse [[Approximeret Jaccard Similarity Searching]] (og almindelig approximeret similarity searching) hvis blot den er givet en familie af [[(s_1, s_2, p_1, p_2)-sensitive hashfunktioner]] for et similarity-rum $(X,S)$ samt to parametre $0 < s_2 < s_1 < 1$. 

Først defineres et rum $B(q, r)$ for et punkt $q$ og et tal $r$ som en kugle omkring punktet $q$ af radius $r$. Et punkt $x$ opfylder $x \in B(q, r)$ hvis afstanden mellem $a$ og $q$ er $< r$.

Nu definerer vi en funktionsfamilie $\mathcal{G}=\{g : S \rightarrow U^k\}$ for et tal $k$ sådan at $g(p)=\langle h_1(p), \dots, h_k(p)\rangle$ for $h_i\in \mathcal{H}$ - altså at $g(p)$ blot kører $k$ forskellige hashfunktioner på $p$.
Nu vælger vi $l$ funktioner fra $\mathcal{G}$ $g_1,\dots, g_l$. 
Når vi så forbehandler hvert $p\in P$, så opbevarer vi punktet i spanden $g_j(p)$ for $j=1,\dots , l$.
Når man så vil querie, så søger man alle spande $g_1(q),\dots , g_l(q)$, hvilket giver en masse punkter $p_1, \dots, p_t$. For hver $p_j$, hvis $p_j \in B(q, r_2)$, så returnerer vi True og $p_j$, ellers returnerer vi False.