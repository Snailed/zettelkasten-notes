Reference: [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]]

I [[Approximeret Jaccard Similarity Searching]] bliver der præsenteret en parameter kaldet $\rho$ som bliver defineret som:
$$\rho=\frac{\log(1/j_1)}{\log(1/j_2)}$$
Eftersom at $0<j_2<j_1<1$, så må dette tal altid være mellem 0 og 1.
Jo større at dette tal, jo større er forskellen på $j_1$ og $j_2$, hvilket betyder at flere svar vil blive accepteret.