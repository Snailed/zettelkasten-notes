[[Filinsky, 2023, Semantics and Types Lecture Notes]]

![[Pasted image 20230319162821.png]]

In writing, for arithmetic expressions:
Arithmetic expressions $a$ and $a'$ are considered semantically equivalent whenever, in all stores $\sigma$, if $a$ can evaluate to an integer $n$, then so can $a'$ and vice versa.

To show semantic equivalence, we must consider how the left-hand side of the $\iff$ could have been derived by the semantic rules, and check that the right-hand side is then also derivable; and then we establish the same property from right to left (**show both sides of the double-implication!**).
