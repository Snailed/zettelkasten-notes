Reference: [[Gionis, Indyk, Motwani - Similarity Searching in High Dimensions via Hashing (1999)]] side 1

Similarity Search problemet er givet sådan: Givet en mængde af datapunkter og en forespørgsel (som også er et datapunkt af samme dimensionalitet), find det punkt i datamængden som er tættest på forespørgselspunktet.

Når man skal søge i store datamængder kan man blive påvirket af [[Curse of Dimensionality]]. Dette kan [[Locality Sensitive Hashing]] være med til at løse hvis du bruger Approksimeret Nearest Neighbor.
[[Approksimeret Nearest Neighbor er godt nok til de fleste tilfælde]] til at løse Similarity Search problemet. Når man skal svare på en forespørgsel, så svarer man bare alle de elementer som har kollideret med forespørgselen. Locality Sensitive Hashing kan løse Similarity Search Problemet i sublineær tid.

Jeg ved at det er defineret lidt anderledes i Jakob Tejs' artikel (noget med Jacobian similarity).

Mulig reference: P. Indyk and R. Motwani. Approximate Nearest Neighbor Towards Removing the Curse of Dimensionality 1998

