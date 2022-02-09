[[Nocedal, Wright - Numerical Optimization]] page 624

A function $f$ is said to be _Lipschitz Continuous_ on some set $\mathcal{N} \subset \mathcal{D}$ if there exists a constant $L>0$ such that 
$$||f(x_1)-f(x_0)||\leq L||x_1-x_0||, \quad \text{for all }x_0, x_1 \in \mathcal{N}$$
$L$ is called the _Lipschitz constant_.
If two functions $f$ and $g$ are Lipschitz continuous with $L_f$ and $L_g$, then $f+g$ will be Lipschitz continuous with $L_{f+g} =L_f + L_g$..
If two functions $f$ and $g$ are Lipschitz continuous, then $fg$ will be Lipschitz continuous *if* both $f$ and $g$ are bounded on $\mathcal{N}$ (that is, there exists a constant $M>0$ such that $|f(x)|\leq M$ and $|g(x)|\leq M$ for all $x\in \mathcal{N}$)
