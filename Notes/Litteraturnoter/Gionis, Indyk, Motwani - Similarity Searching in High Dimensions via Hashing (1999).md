1: I 1999 (og sikkert også nu) var der en del research der pegede på at man skulle bygge index/søgetræs strukturer for at hjælpe med similarity search over højdimensionel data.
1: Disse strukturer led af "curse of dimensionality" - når antallet af features er over en 10-20 stykker, så ender søgning i k-d træer og lign. med at involvere søgning i næsten hele databasen, hvilket ikke er meget bedre end lineær søgning.
1: Det vurderes at eftersom at afstandsfunktionen og valg af features er valgt på baggrund af heuristikker, så må en approximeret nærmeste nabo være godt nok til det meste brug i praksis.
1: I artiklen præsenterer de en "ny" måde at gøre dette på, ved at hashe datapunkter i en database sådan så at punkter der er tæt på hinanden har større sandsynlighed for at kollidere end punkter der er langt væk fra hinanden.
1: De præsenterer eksperimentel empiri for at deres metode er hurtigere end en klassisk træ-struktur, og at deres metode skalerer godt til højdimensionel data (over 50 dimensioner).
1: Similarity search problemet er givet sådan: Givet en mængde af datapunkter og en forespørgsel (som også er et datapunkt af samme dimensionalitet), find det punkt i datamængden som er tættest på forespørgselspunktet.
1: Similarity search problemet er mest velstuderet i et d-dimensionelt Euclidisk rum.
1: Man kan også løse problemet med at lave en indeksing-struktur
2: I stedet for at opdelet rummet bruger forfatterne *locality sensitive hashing* (LSH)
2: Locality Sensitive Hashing hasher datapunkter sådan så at to punkter der er tætte på hinanden har stor sandsynlighed for at hashe til det samme punkt
2: Når man så skal svare på en forespørgsel svarer man bare alle de elementer som har kollideret med forespørgselen.
2: Indyk og Motwani introducerede LSH (P. Indyk and R. Motwani. Approximate Nearest Neighbor Towards Removing the Curse of Dimensionality 1998)
2: Worst case tid er $O(dn^{1/(1+\epsilon)})$. Det betyder at den kører i sublineær tid for alle $\epsilon > 0$
3: skriv noget om Hamming distance
3: Definition 1: Nearest Neighbor Search (NNS): Givet en mængde $P$ af $n$ objekter repræsenteret som punkter i et normeret rum $l_p^d$, forbehandl $P$ sådan så man effektivt kan svare på forespørgsler ved at finde det punkt i $P$ som er tættest på et forespørgselspunkt $q$
3: Definition 2: $\epsilon$-Nearest Neighbor Search ($\epsilon$-NNS): Givet en mængde af punkter $P$ i et normeret rum $l_p^d$, forbehandl $P$ sådan så at man effektivt kan returnere et punkt $p\in P$ for et hvert forespørgselspunkt $q$ sådan at $d(q,p)\leq (1+\epsilon)d(q,P)$ hvor $d(q,P)$ er afstanden fra $q$ til dens tætteste punkt i $P$.
3: Antagelser til algoritmen: Distancen følger $l_1$ normen (manhattan normen, men gør ikke nogen forskel), coordinater af punkter i $P$ er positive heltal
3: Et gennemsnitligt forespørgselspunkt beregnet under $l_1$ normen er også en $\epsilon$-approximativ nabo under $l_2$ normen med en gennemsnitlig $\epsilon$-værdi på under 3%.
3: Forskellen på $l_1$ og $l_2$ normen er meget lille
3: Man kan nemt transformere alle ens datapunkter til at være positive heltal, så længe at man accepterer en lille fejl. 
3: Hvis du definerer $v(p)$ som en *unary* repræsentation af et datapunkt, så vil $d_1(p,q)=d_H(v(p),v(q))$ hvor $d_H$ er Hamming-afstanden, ergo at denne hash-funktion bevarer afstande.
3: Man *behøver* dog ikke at lave denne transformation til unary format. Idéen gør bare nogle ting nemmere.
4: Hashfunktionen er defineret som følgende: Vælg $l$ delmængder $I_1, \dots, I_l$ fra $\{1,\dots, d'\}$. Lad $p_{|I}$ være projektionen af en vektor $p$ på koordinatsættet $I$ (dvs vælg koordinatpositioner $j_i$ fra $I$ og sæt bitsene fra $p_{j_i}$ sammen).   Eksempel: $p=[4,3,3,6,5]^T,\ I=\{1,3,5\} \implies p_{|I}=concat([4,3,5]^T)=10011101_2=157_{10}$
4: Hashfunktionerne er defineret som sådan: Vælg $l$ delmængder $I_1, \dots, I_l$ fra $\{1, \dots, d'\}$. Hver delmængde kan nu betragtes som et koordinatserie (eks: $\{1,6,3\}\rightarrow (1,6,3)$). 
4: Lad $g_j(p)=p_{|I_j}$. Dette udregnes ved blot at vælge værdierne på koordinaterne fra $I$ og sammensætte deres binære repræsentation. Nu opbevares hvert datapunkt i en spand for hvert $j\in [l]$ (som selv er en normal hashtabel)
4: Størrelsen på hashtabellen kan beskrives sådan her: $M=\alpha \frac{n}{B}$ hvor $\alpha$ er en parameter der beskriver forholdet mellem hukommelse allokeret til indeksering vs størrelsen af datasættet.
4: Når vi så skal foretage et opslag, så finder vi $g_1(q), \dots g_l(q)$ og søger igennem alle punkterne indtil vi finder mindst $c\cdot l$ punkter eller bruger alle $l$ index. Ud fra dette gennemsøger vi $p_1, \dots, p_t$ punkter fra hvilket vi returnerer de $K$ tætteste (vi kan risikere at returnere mindre end $K$!).
4: Når vi vælger $I_j$, så vælger vi $k$ elementer fra $\{1, \dots, d'\}$.  Den optimale værdi af $k$ er valgt for at maximere sandsynligheden for at et punkt $p$ "tæt" på $q$ vil falde i samme spand som $q$ og for at minimere at et punkt $p'$ som er "langt" væk fra $q$ lander i sammem spand som $q$.
4: Vi kan lave en ret effektiv hashfunktion hvis vi konverterer $l_1^d$ til et $d'$-dimensionelt Hamming rum: Lad $p$ være et givent punkt fra datasættet og $p'$ være dets afbilledning efter at være blevet konverteret. Lad $I$ være koordinatsættet. For $i=1,\dots, d$, lad $I_{|i}$ være i sorteret rækkefølge koordinater i $I$ som svarer til det $i$nde koordinat af $p$
