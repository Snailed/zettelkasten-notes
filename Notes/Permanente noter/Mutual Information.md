[[Ryan, 2015 - A Review of Modern Computational Algorithms for Bayesian Optimal Design]]
[[Bishop - Pattern Recognition and Machine Learning]]

A [[Design Criterion]] for [[Experimental Design]] based on the expected [[Kullback-Leibler Divergence KLD]].

Consider a joint distribution between two sets of variables $\mathbf{x}$ and $\mathbf{y}$, $p(\mathbf{x},\mathbf{y})$. If they're independent, then $p(\mathbf{x},\mathbf{y})=p(\mathbf{x})p(\mathbf{y})$. Otherwise, we can measure how "close" to independent they are by taking the KLD of the LHS and the RHS:
$$\text{I}[\mathbf{x,y}]=KL(p(\mathbf{x,y})||p(\mathbf{x})p(\mathbf{y})) $$
$$= -\iint p(\mathbf{x,y})\ln (\frac{p(\mathbf{x})p(\mathbf{y})}{p(\mathbf{x,y})}) \ d\mathbf{x}\ d\mathbf{y}$$