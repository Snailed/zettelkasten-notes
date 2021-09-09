1: Artiklen handler om Approximate Similarity Searching ud fra "Jaccard Similarity" $J(A,B)=\frac{|A\cap B|}{|A\cup B|}$
1: Den er lidt anderledes end LSH ved at den omhandler mængder. Du har en række mængder fra et univers, og du vil finde en mængde der minder om en forespørgselsmængde. I realiteten er dette vel det samme som et punkt - men punkter har vel ordnede koordinater, hvilket mængder ikke nødvendigvis har.
1: Den virker ved at man har to tal $j_1$ og $j_2$ mellem 0 og 1 ($j_2$ er mindre eller lig $j_1$), og at man så vil finde en mængde $B$ der er tættere på forespørgselsmængden $Q$ end $j_2$ betinget af at sådan en mængde eksisterer indenfor en afstand af $j_1$.
I artiklen kalder de den mængde der returneres for $A$ og den mængde som skal eksistere for at algoritmen vil returnere for $B$. Det er muligt at $A=B$. 
1: Der er en konstant fejlsandsynlighed dvs. at algoritmen ikke returnerer $A$ hvis $B$ eksisterer. Det betyder at man kan bruge mediantricket til at opnå en variabel sandsynlighed og præcision.
1: Denne artikel reducerer pladsforbruget og query tid til sublineær tid.
2: Læs mere om MinHash algoritmen af Broder et al.
2: Den originale LSH framework får et pladsforbrug på $O(n^{1+\rho} + \sum_{A\in\mathcal{F}}|A|)$ og en query tid på $O(|Q|\cdot n^{\rho}\log{n})$ hvor $\rho=\frac{\log(1/j_1)}{\log(1/j_2)}$. Den har en konstant 1-sided fejlsandsynlighed.
2: At have en konstant fejlsandsynlig gør så vi kan vælge hvilken fejlsandsynlighed vi gerne vil have. For at få en ønsket fejlsandsynlighed $\epsilon = o(1)$, så skal vi have $O(\log(1/\epsilon))$ uafhængige datastrukturer og så bare returnere den bedste løsning hvis der findes sådan en.
Hvis vi gør dette får vi ud fra de nuværende state-of-art datastrukturer får vi en query time på $O((n^\rho+|Q|)\log(1/\epsilon))$
2: Behøver vi have uafhængige datastrukturer? Ifølge Jakob Tejs, så nej! Man kan faktisk spare log-faktoren sådan så man ikke længere skal udregne mange forskellige hashværdier for query-mængden. Så får man en query time på $O(n^\rho\log(1/\epsilon)+|Q|)$
2: Ved hjælp af bit parallelisme kan man yderligere forberedre query tiden til $O((\frac{n\log w}{w})^\rho\log(1/\epsilon) + |Q|)$ og endda et forbedret pladsforbrug til $O((\frac{n\log w}{w})^\rho\log(1/\epsilon) + \sum_{A\in\mathcal{F}}|A|))$ hvilket virker generelt for LSH.
2: Et similarity space er en to-tuppel af form $(X,S)$ hvor $X$ er et inputrum og $S$ er en afstandsfunktion.
