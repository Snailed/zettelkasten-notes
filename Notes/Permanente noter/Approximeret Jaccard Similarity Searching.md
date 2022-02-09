Reference [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]], side 1-2, [[Dahlgaard, Knudsen, Thorup - Fast Similarity Sketching]]

Hvis man har to tal $0 < j_2 < j_1 < 1$ samt to mængder $A$ og $B$ fra en familie $\mathcal{F}$ fra et stort univers $U$ så kan vi søge efter en mængde $Q$ og returnere en mængde $A$ hvor $J(A,Q) \geq j_2$ hvis der findes en mængde $B$ hvor $J(B,Q) \geq j_1$.

(her er $J$ [[Jaccard Similarity]] funktionen)

Den klassiske måde til at løse dette på er ved hjælp af [[MinHash]], men nyere metoder er set i [[Fast Similarity Sketching]] og [[Fast Similarity Searching]].