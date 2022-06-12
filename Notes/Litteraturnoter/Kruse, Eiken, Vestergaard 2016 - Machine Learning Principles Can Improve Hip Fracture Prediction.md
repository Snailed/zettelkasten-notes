# Redegørelse
Formålet er at anvende machine learning til at forudsige hoftebrud
Undersøger mænd og kvinder som har fået foretaget en DXA scanning indenfor en vis tidsperiode.
Undersøger en masse forskellige parametre, og har en masse forskellige datakilder
De har indsamlet det automatisk for at undgå bias

De har brugt krydsvalidering

Datasættene indeholder 75.000 forskellige predictors bl.a. persondata og sundhedsdata
De har brugt en række metoder til at reducere disse, f.eks. med varians -> 1200 predictors.

De finder en stor uoverensstemmelse mellem kvinder og mænd.

De har brugt en masse forskellige modeller, men endte med to forskellige modeller fra mænd og kvinder.

# Diskussion om objektivitet
Dataindsamling, inklusionskritierier (kun Aarhus og Aalborg), kun folk der er blevet scannet, bias i hvilke biokemiske faktorer der er valgt, bias i valg af kategorier

Dataens begrænsninger
De har ikke indeholdt alkohol og tobaksforbrug f.eks. eller genetik.

Håndtering af dataindsnævring. 

Modellen er ikke objektiv. De har et godt fundament, men de prøver at lave et mere generelt billede på om disse metoder kan bruges generelt.

Spørgsmål: De undersøger om machine learning kan bruges generelt indenfor medicin. Tror I at et emner som disse kan forudsiges med én slags model? Eller et framework? Eller er domænerne så forskellige at det kan være svært?

# Spørgsmål fra plenum
3 epistemiske problemer ved ML
-> De mange dim. forbandelse
	Mange predictors, reducere data
	Få data med til at stole på predictors
	vælge relevante faktorer
-> problemet med sammenfaldende data
	Korrelation -/> kausalitet
	Usynlige confounding factors
-> induktionsproblemet
	Hvorvidt at modellen kommer til at virke i fremtiden.
	
