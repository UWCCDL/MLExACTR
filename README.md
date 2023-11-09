# A Tutorial on Fitting and Comparing ACT-R Models Using Maximum Likelihood

ACT-R is an integrated framework that is widely used in cognitive psychology and cognitive neuroscience. It is one of the most popular and widely used cognitive architectures (Kotseruba and Tsotsos 2020), the most popular in the psychological sciences, and of the most popular modeling frameworks in the field, with approximately 1,000 scientific publications to its name.

As part of the work, ACT-R researchers often perform operations of model-fitting, attempting to fit the model parameters against some group-level (or, more rarely, individual-level) behavioral index. At the time of writing, the most common measures used to fit these models are Spearman correlations and RMSE. In cases in which two or more models are comparatively evaluated, the same measures are used to decide which model is the best. This approach is potentially misleading.

This repository offers a tutorial on how to fit, evaluate, and compare ACT-R models on the basis of their _likelihood_. The likelihood of a model _m_ with a given set of parameter values _θ_, given the data __x__, is formally defined as 

$$L(m, θ | x_o) = P(x = x_o | m, θ)$$

The meaning of Equation 1 is appealingly intuitive: a model is more “likely” when it has a greater probability of producing the observed data.

![Visual Interpretation of Likelihood](figures_publications/figure1.png)

There are good reasons why ACT-R researchers have not historically relied on likelihood. We argue, however, that this is a limitation, and that likelihood can and should be used more broadly. The accompanying Jupyter Python notebook provides step-by-step instructions and Python code examples; the code contains all of the data and code to generate the examples and figures in the accompanying paper.
