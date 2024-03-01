[[Yehudayoff, 2023 - ATML Lecture Notes]]
Also known as the [[Expected loss]].
The population loss over a distribution $\mu$ for some hypothesis $h\in H$ is defined by
$$L_\mu(h)=\mathbb{E}_{(x,y)\sim \mu}(L(h, (x,y)))$$
The population loss of an entire hypothesis class $H$ is defined by
$$L_\mu(h) = \inf\{ L_\mu(h)\ \colon h \in H\}$$
The counter part of [[Empirical Loss]]
An example of loss functions could be the [[The 0-1 loss function]]. 