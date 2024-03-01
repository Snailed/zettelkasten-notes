[[Shalev-Shwartz & Ben-David, 2014 - Understanding Machine Learning From Theory to Algorithms]]
[[Yehudayoff, 2023 - ATML Lecture Notes]]

A hypothesis class $H \colon X \rightarrow \{0, 1\}$ _shatters_ a set $C \subset X$ if the hypothesis class contains all functions from C to 0,1, i.e.
$$H|_C = h \in H \colon C \rightarrow \{0, 1\}$$
$H$ shatters $C$ if $H|_C = C$

## Example
Imagine the hypothesis class of all intervals on a real line.
If $C=\{c_1, c_2\}$, then all functions from $C$ to $0,1$ can be described by a vector representation of its results like so:
$$\{(0,0), (0,1), (1,0), (1,1)\}$$
Since one can find a $h\in H$ for each of these results, we say that $H$ shatters $C$.
If $C=\{c_1, c_2, c_3\}$, then we cannot find a $h$ for $(1, 0, 1)$ and thus $H$ does not shatter $C$