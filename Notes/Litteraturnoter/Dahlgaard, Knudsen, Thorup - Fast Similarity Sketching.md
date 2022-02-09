1: Similarity Sketching problemet: Givet et univers $[u]=\{0,\dots,u-1\}$, ønsker vi en tilfældig funktion $S$ som afbilleder delmængder $A\subseteq [u]$ ind i vektorer $S(A)$ af størrelse $t$ sådan så at similarity er bibeholdt.

De definerer en stokastisk variabel $X$ som følgende:
Givet to mængder $A,B \subseteq [u]$, så vil $X_i=[S(A)[i] = S(B)[i]]$ og $X=\sum_{i\in[t]}X_i$. Vi vil gerne have at den forventede værdi af $X$ er $E[X]=t\cdot J(A,B)$

2: Denne artikel bidrager med en metode der blander sampling med tilbagelægning og uden tilbagelægning. Den har super gode koncentration bounds og kan bruge en mixed-tabulation hashfunktion som kan blive evalueret i $O(1)$ tid.

3: Theorem 1: Lad $[u]=\{0,1,2,\dots, u-1\}$ være en mængde af nøgler. Der eksisterer en algoritme som givet en mængde $A\subseteq [u]$ i forvented tid $O(|A| + t\log t)$ laver en vektor $v(A)$ af størrelse $t$ som kun består af ikke-negative reelle tal.
Disse tal besidder den følgende egenskab. For to mængder $A,B\subseteq [u]$ gælder det at $v(A\cup B)_i =\min\{v(A)_i,v(B)_i\}$ for alle index $i\in[t]$. 
Nu kan vi pakke dens concentration bounds ind i en Chernoff-agtig pakke.
For $i\in [t]$ lad $X_i=1$ hvis $v(A)_i=v(B)_i$ og lad $X_i=0$ ellers og lad $X=\frac{1}{t}\sum_{i\in[t]}X_i$. Så vil $E[X]=J$ hvor $J(A,B)$ og for alle $\delta > 0$ holder det at:
$$Pr[X\geq J(1+\delta)]\leq \left(\frac{e^\delta}{(1+\delta)^{1+\delta}}\right)^t$$
$$Pr[X\geq J(1-\delta)]\leq \left(\frac{e^\delta}{(1-\delta)^{1-\delta}}\right)^t$$
4: Denne metode filtrerer falske positiver i forventet konstant tid, i forhold til $O(L\cdot |Q|)$ tid som fra MinHash.
Derudover så beregner man færre hashværdier ved at bruge den nye similarity sketch og så sample fra den på en smart måde til at bygge en LSH tabel i $O(L\cdot K + |Q|)$ tid, hvilket forbedrer query tid til $O(L\cdot K + |Q|)=O(n^\rho \log n + |Q|)$