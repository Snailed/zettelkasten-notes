Reference: [[Tejs Knudsen, Fast Similarity Search with Low Error Probability, 2021]]

Antallet af 1'er i en bitstreng kan udregnes i $O(\log d)$ tid. Dette udføres på følgende måde:

Først skal vi bruge en bit-maske. Den er defineret som følgende:
Bitmasken $m_{i,j}$ starter med en sekvæns af $2^j-2^i$ 0'er. Derefter kommer $2^i$ 1'er, hvorefter den gentager sig selv uendeligt.
Shorthand skriver man $m_{i}$ for $m_{i,i+1}$.
Derefter skal vi bruge følgende funktion: 
$$T(t,m,k)=(t>>k) \& m$$

Nu kan vi bruge følgende funktion til at udregne antallet af 1'er i en bitstreng:
$$t^{(0)} = t$$
$$t^{(i+1)}=T(T(t^{(i)}, m_i, 0)+T(t^{(i)}, m_i, 2^i), m_{i+1}, 0)$$
Nu vil antal 1'ere i den j'ne bitstreng i t være $T(t^{(i)}, 2^{2^i+1}-1, j\cdot 2^i)$
Der findes også en intuitiv [[Forklaring af antal 1'er i en bitstreng]].