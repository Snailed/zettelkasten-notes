[[Gionis, Indyk, Motwani Similarity Searching]]

Hashfunktionen som bliver beskrevet i [[Gionis, Indyk, Motwani - Similarity Searching in High Dimensions via Hashing (1999)]] virker som følgende:

Hvis hvert datapunkt $p\in P$ har en dimensionalitet af $d$, så vælg et tal $l \leq d'$. Jo større tal, jo højere plads/tidsforbrug og bedre præcision. Hvis du så har en tilfældig delmængde $I$ fra $\{1, \dots, d'\}$ er hashfunktionen $g(p)=p_{|I}$ (projektionen af $p$ på koordinatsettet $I$). Dette foretages i praksis ved at vælge koordinaterne som defineret i $I$ og sammensætte deres bineære repræsentationer.

Eksempel:
$p=[4,3,3,6,5]^T,\ I=\{1,3,5\} \implies p_{|I}=concat([4,3,5]^T)=10011101_2=157_{10}$

