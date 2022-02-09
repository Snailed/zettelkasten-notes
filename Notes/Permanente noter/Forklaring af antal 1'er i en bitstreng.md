Reference: [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]]

Versionen i [[Antallet af 1'er i en bitstreng kan udregnes i O(log d) tid]] er lidt for kompleks, her er en intuitiv version til den "naive" version af algoritmen.

Betragt følgende bitstreng:
$$1011100110101101$$
Vi vil gerne tælle antallet af 1'taller. Vi kan betragte den som en samlet bitstreng af mange små blokke af størrelse 1. For en blok af størrelse 1 gælder at dens værdi svarer til antallet af 1-taller i dens bitstreng (0 = 0 1'er, 1= 1 1'er).
Når vi har to blokke der hver repræsenterer antallet af 1'er i bitstrengen kan vi plusse dem for at finde antallet af 1'er i deres samlede bitstreng (altså en blok af dobbelt størrelse).

Derfor tager vi hver anden blok af størrelse 1 og plusser med blokken til venstre for den.
$$0110010101011001$$
Nu har vi en masse blokke af størrelse 2. Nu kan vi tage hver anden blok af størrelse 2 og plusse den med blokken til venstre for den.
$$0011001000100011$$
Nu har vi en masse blokke af størrelse 4. Nu kan vi tage hver anden blok osv.
$$0000010100000101$$
Osv:
$$0000000000001010$$

