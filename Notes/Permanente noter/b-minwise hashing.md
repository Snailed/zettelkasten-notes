Reference: [[Li, Shrivastava, Moore, König - Hashing Algorithms for Large Scale Learning]]

Man kan reducere størrelsen af en [[MinHash]]-sketch ved blot at opbevarer de $b$ laveste bits af hashværdien. Dette gør så man kan opbevare mange flere sketches på én gang, og som kan kombineres med [[Antallet af 1'er i en bitstreng kan udregnes i O(log d) tid]] så man kan køre searching i sublineær tid.