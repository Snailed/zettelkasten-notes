Reference: [[Gionis, Indyk, Motwani - Similarity Searching in High Dimensions via Hashing (1999)]] side 1, [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]], [[Dahlgaard, Knudsen, Thorup - Fast Similarity Sketching]]

Similarity Search problemet er givet sådan: Givet en mængde af datapunkter og en forespørgsel (som også er et datapunkt af samme dimensionalitet), find det punkt i datamængden som er tættest på forespørgselspunktet. 
Datapunkterne kan være regulere punkter eller mængder. 

Når man skal søge i store datamængder kan man blive påvirket af [[Curse of Dimensionality]]. Dette kan [[Locality Sensitive Hashing]] være med til at løse hvis du bruger Approksimeret Nearest Neighbor.
[[Approksimeret Nearest Neighbor er godt nok til de fleste tilfælde]] til at løse Similarity Search problemet. Når man skal svare på en forespørgsel, så svarer man bare alle de elementer som har kollideret med forespørgselen. Locality Sensitive Hashing kan løse Similarity Search Problemet i sublineær tid når først at alle datapunkterne er præprocesseret.

Præprocessering kan ske på mange måder. I almindelig LSH hasher man alle datapunkterne, men man kan også bruge [[Fast Similarity Sketching]] til at oprette "sketches" over dataen som kan bruges til at søge igennem senere. 

For at kunne lave similarity searching skal man bruge en afstandsfunktion. I almene datapunkter kan man bruge Manhattan distance ([[Der er minimal forskel på Manhattan og Euclid-normen]]), og med mængder kan man bruge [[Jaccard Similarity]] (se evt. [[Approximeret Jaccard Similarity Searching]]).

Mulig reference: P. Indyk and R. Motwani. Approximate Nearest Neighbor Towards Removing the Curse of Dimensionality 1998

