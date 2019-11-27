# nice-reads

## Variational inference, idea and methods 
1. [Variational Inference: A Review for Statisticians](https://arxiv.org/pdf/1601.00670.pdf) - review paper on variational inference. 

After reading this paper you should know:
* What is variational inference?
* How and why do we even need variational inference?
* What is the evidence lower bound? The intution behind its components? More to think: what is the relationship between the evidence lower bound and expectation-maximization (EM) algorithm?
* What is mean-field approximation?

2. [Auto-Encoding Variational Bayes](https://arxiv.org/pdf/1312.6114.pdf) - A nice usage of variatonal inference introducing reparametreization trick

This paper introduces the reparameterization trick which enables computing gradient of the parameters of the posterior distribution on a expectation operator of any function of posterior distribution. After reading this paper you should know:

* A sample usage of variational inference to estimate an intractable distribution?
* What is the cost function when the prior distibution of the latent variable is assumed to be Gaussian?
* What does each component of the cost function mean? -very important
* What is reparameterization trick? Why do we even need it? Why does it work?
* Understand the variational auto encoder deeply as it is the foundation of many consecutive papers 

3. Some papers that use variational inference to learn nonlinear dynamics and emmission in sequential data

 - 3.1. [Structured Inference Networks for Nonlinear State Space Models](https://arxiv.org/pdf/1609.09869.pdf)

 - 3.2. [A Disentangled Recognition and Nonlinear Dynamics Model for Unsupervised Learning](https://arxiv.org/pdf/1710.05741.pdf)

After reading this papers you should know:

* How papers 1 and 2 were used in building structure of the model algorithm?
* What are the ways to improve on these papers and many other similar papers?
