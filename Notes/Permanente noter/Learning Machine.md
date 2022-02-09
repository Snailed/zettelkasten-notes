[[EML 7-2-2022]]

A learning machine works by picking a hypothesis $h\colon \mathcal{X} \rightarrow \mathcal{Y}$ from a hypothesis class $\mathcal{H}$ 
Applying a learning algorithm means coming up with a hypthesis from the hypothesis class given sample data.
This can be seen as a mapping from the sample to the hypothesis class:
$$\{((x_1, y_1, \dots , (x_n, y_n))| 1 \leq i \leq n < \infty, x_i\in \mathcal{X}, y_i\in \mathcal{Y}\}\ \text{to }\mathcal{H}$$

The quality of the prediction is quantified by a [[Loss function]] (that is picked specifically for the task)

The goal of learning is to minimize expected loss