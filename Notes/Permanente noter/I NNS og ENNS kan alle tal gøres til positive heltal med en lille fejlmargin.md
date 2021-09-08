Reference: [[Gionis, Indyk, Motwani - Similarity Searching in High Dimensions via Hashing (1999)]] side 3

Hvis man transformerer alle datapunkterne til positive heltal får man kun en lille fejl. For at beholde detaljer i decimaler kan man bare gange tallene med en stor nok konstant, da en skalering af rummet stadig bevarer forholdet mellem afstande. Så kan man nemlig løse [[Nearest Neighbor Search (NNS)]] og [[Epsilon-Nearest Neighbor Search (ENNS)]] på samme måde som før.

Det er smart at transformerer datapunkterne til positive heltal, da man så kan lave [[Locality Sensitive Hashing]]