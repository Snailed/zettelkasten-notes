# Kunsten at få en computer til at adlyde (I): Programmering
## Modularisering, abstraktion og grænseflader
Computerprogrammer er en streng af instruktionskoder
Pålidelighed vs hastighed, omkostninger ved vedligeholdelse osv.
Softwarekrise
Software som ingeniørvidenskab
Struktureret Programmering fremført af Dijkstra.
Resultat af softwarekrisen:
- Strukturelle sprog (subroutiner, blokke, kontrolstrukturer)
- Modularisering (store systemer i forskellige delproblemer, og gøre delene så robuste og fejlfri som muligt)
- Linking
Generelt set abstraktionsprocesser
Grænseflader

## Programmeringssprog
Wirth:
> A language represents an abstract computer whose objects and constructs lie closer to, and reflect more directly, the problem to be represented than the concrete machine.

Et sprog er ifølge ham en abstrakt computer.
IBM udviklede FORTRAN, akademikere ALGOL.
ALGOL var maskinagnostisk.
LISP med dens lambdafunktioner
Simula med dens agenter der interagerer med hinanden (forløber til OOP)
BASIC
PASCAL  
PROLOG
C
C++
## Programmeringsparadigmer
Imperative (proceduerelle sprog vs objekt-orienterede) vs deklarative sprog
Programmeringsparadigmer kan være et filter som man anskuer verden med
De er sameksisterende

## Fra algoritme til afvikling
Den moderne måde at notere algoritmer er en model der har mange implicitte antagelser og forsimplinger
![[Pasted image 20220613203903.png]]
Afviklingen af en computer er et åbent system desværre.

## Fuld fart frem
Eksemplet med Toyota og bilulykkerne. Man kan ikke bevise at kode er fejlfrit med man kan godt påvise en fejl.
Bevis af kritiske systemer igennem formel verifikation.
Omfattende systematisk og teoridreven afprøvning.

