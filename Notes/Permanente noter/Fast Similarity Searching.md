Reference: [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]]

Defineret af Jakob Tejs Knudsen.
Baseret på [[Fast Similarity Sketching]] af Dahlgaard et al. Første reelle pladsforbedring siden [[Gionis, Indyk, Motwani Similarity Searching]].

Tidsforbrug:
$$O((\frac{n\log w}{w})^\rho\log(1/\epsilon) + |Q|)$$

Pladsforbrug:
$$O((\frac{n\log w}{w})^\rho\log(1/\epsilon) + \sum_{A\in\mathcal{F}}|A|))$$

Denne algoritme har to forbedringer: Først og fremmest producerer den kun ét stort sketch i stedet for $M$ sketches, og det bliver delt op i $M$ delsketches. Disse sketches er ikke længere uafhængige, men Jakob Tejs viser at det ikke er et problem.

Dernæst benytter den også word-parallelisme for at reducere $n^\rho$ faktoren til $(\frac{n\log w}{w})^\rho$