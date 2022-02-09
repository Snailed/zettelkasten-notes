Reference: [[Vassilvitskii, Sergey - Dealing with Massive Data]]

For en mængde $V$ kan vi definere en vektor $S(V)$ som er dens "summary vector" defineret som sådan:
$$S(V)=\langle H_1(V),H_2(V),\dots H_k(V)\rangle$$
hvor $H$ er som defineret i [[MinHash]].
Vi kan approximere to dokumenters similarity ved at sammenligne deres summary vectors.