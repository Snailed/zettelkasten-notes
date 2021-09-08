Reference: [[Gionis, Indyk, Motwani - Similarity Searching in High Dimensions via Hashing (1999)]]

 >Givet en mængde af punkter $P$ i et normeret rum $l_p^d$, forbehandl $P$ sådan så at man effektivt kan returnere et punkt $p\in P$ for et hvert forespørgselspunkt $q$ sådan at $d(q,p)\leq (1+\epsilon)d(q,P)$ hvor $d(q,P)$ er afstanden fra $q$ til dens tætteste punkt i $P$.

Bruges til [[Similarity Search Problemet]]. Relateret til [[Nearest Neighbor Search (NNS)]]. Den kan bruges i stedet for NNS da [[Approksimeret Nearest Neighbor er godt nok til de fleste tilfælde]].