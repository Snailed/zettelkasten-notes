Reference [[Gionis, Indyk, Motwani - Similarity Searching in High Dimensions via Hashing (1999)]].

Vælg $l$ delmængder af størrelse $k$ kaldet $I_1, \dots, I_l$ fra $\{1, \dots, d'\}$. Hver delmængde kan nu betragtes som et koordinatserie (eks: $\{1,6,3\}\rightarrow (1,6,3)$). [[I LSH vælger man delmængder ud fra en parameter k der bestemmer præcision]].
Herefter hasher man hvert eneste datapunkt $l$ gange ved hjælp af [[Gionis, Indyk, Motwani Locality Sensitive Hash-funktion]] og opbevarer det i en spand $j \in [l]$.
Når vi så skal foretage et opslag ud fra et opslagspunkt $q$, så finder beregner vi $g_1(q), \dots g_l(q)$ og søger igennem punkterne i hver tilsvarende spand. Når vi har fundet mindst $c \cdot l$ eller har brugt alle $l$ indices stopper vi og returnerer de $K$ tætteste punkter (eller mindre!) ud fra dem vi har fundet.
[[I LSH afhænger størrelsen af hashtabellen på en parameter alpha der beskriver forholdet mellem hukommelse og datamængden]]
