# Redegørelse
## Datalogiens matematiske rødder
Datalogi og matematik hænger tæt sammen
Matematik er abstrakt og i formelle systemer. Vi antager at computere også er formelle systemer, men det er også virkelige maskiner der skal køre rigtige programmer

## Turingmaskiner og Hilberts program
I starten af 1900-tallet mente filosoffer at man kunne opnå klar sikkerhed ved hjælp af matematik indenfor formelle systemer
Atomare beregninger i den endelige aritmetik er perfekte (ifølge Hilbert)
Ifølge hilbert:
1. Matematikken skulle sikres igennem syntaktiske aksiomssystemer hvori al mening var givet implicit af aksiomerne
2. Man skal opstille formelle systemer og vise deres uafhængighed, konsistens og fuldstændighed ved hjælp af endelige metoder. Dermed bevise at der ikke er modstrid i aksiomerne
3. Derefter kan man tilføje ideale elementer igennem konservative udvidelser således at de ikke danner modstrid med andre aksiomer. Dermed har man sikret hele matematikken, særligt den uendelige del fra mængdelæren og differentialregning
Gödel, den mad man, beviser dog at alle konsistente aksiomssystemer vil være ufuldstændige.

Turingmaskinen: En model for beregning af tal (og propositioner).
Man har en maskine med nogle konfigurationer og et uendeligt langt bånd bestående af en masse kvadranter. Ved at læse og skrive i kvadranterne og ændre sine konfigurationer kan den beregne alt.

Church-Turing-tesen: Church-Turing-tesen: Alt hvad der kan siges at være beregneligt, kan beregnes af en maskine, som den Turing beskrev i 1936, hvilket Turing gjorde eksplicit i en artikel fra 1948.

Turing hævdede at en beregnelig sekvæns af tal er alene afgjort af det program der beregner den.

Ved at lave en maskine der kan simulere en turingmaskine, kan den beregne det samme som en turingmaskine. Dermed er den turing-komplet.
Halting-problemet er bevis på at der findes problemer der ligger udenfor Turing-maskiners udtrykskraft.
Entscheidungsproblemet: Man kan ikke finde en generel, effektiv algoritme der afgør om en sætning er en del af et givet formel system.
Det hele leder til P = NP problemet.

Hartmanis' paradigme: Turingmaskiner kan bruges til at finde et problems kompleksitetsklasse. En Turing's man.

## Algoritme begreb(er)
Algoritmer kan både betyde formelle teoretiske algoritmer, men også større systemer som Facebooks algoritmer. Det kan også betyder et større etnografisk system (se [[Seaver, 2017 - Algorithms as culture. Some tactics for the ethnography of algorithmic systems]]).
En algoritme kan være en formalistisk model, men også et "objekt" som man kan "eje". Den kan også have en social karakter hvis man kan kommunikere med den.
Den datalogiske teoretiske algoritme består af en række handlinger som skal udføres. De er klare og har et veldefineret resultat. Opskriften kan dermed også ses give et rigtigt resultat.
Relation mellem algoritme og kørsel.


## Computere og matematiske beviser
Beviskulturer
Formelle beviser af kode og computerchips
Eksperimentel matematik
Firefarvesætningen
To problemer med formelle beviser i praksis: De kan aldrig bevise reelvidenskabelige forhold og de er meget tidskrævende.

Beviser er kun for specifikation-implementation forholdet.

Af teoretiske algoritmer er vi typisk interesseret i at bevise korrekthed, terminering, køretid og pladsforbrug.

Bell-LaPadula-modellen for sikkerhed (no write-down, no read-up). Covert Channels.


## Videnskabelige revolutioner
Kuhn i forhold til datalogien. Normalvidenskab udforsker paradigmet.
Når man får anomalier så forkaster man ikke bare hele paradigmet med det samme, men nærmer lader dem ophobe sig.
Mono-paradigmatisk videnskab.
Hvordan fungerer interdisciplinære videnskaber med Kuhns teori? 
Hvis datalogi skal hjælpe verden skal vi være tværvidenskabelige!
