# nice-reads

## Variational inference, idea and methods 
Here, I provide some papers that talk about variational inference; why do we need it and how do we use it? 

### 1. [Variational Inference: A Review for Statisticians](https://arxiv.org/pdf/1601.00670.pdf) - a review paper on variational inference. 

After reading this paper you should know:
* What is variational inference?
* Why do we even need variational inference and how do we use it?
* What is the evidence lower bound? The intution behind its components? More to think: what is the relationship between the evidence lower bound and expectation-maximization (EM) algorithm? Also see Matthew Beal's great [PhD thesis](https://cse.buffalo.edu/faculty/mbeal/papers/beal03.pdf) 
* What is mean-field approximation?

### 2. [Auto-Encoding Variational Bayes](https://arxiv.org/pdf/1312.6114.pdf) - A nice usage of variatonal inference introducing reparametrization trick.

This paper introduces the reparameterization trick which enables computing gradient of the parameters of the posterior distribution on a expectation operator of any function of posterior distribution. After reading this paper you should know:

* A sample usage of variational inference to estimate an intractable distribution? Also see Diederik Kingma's great [PhD Thesis](https://www.dropbox.com/s/v6ua3d9yt44vgb3/cover_and_thesis.pdf?dl=0)
* What is the cost function when the prior distibution of the latent variable is assumed to be Gaussian?
* What does each component of the cost function mean? -very important
* What is reparameterization trick? Why do we even need it? Why does it work?
* Understand the variational auto encoder deeply as it is the foundation of many consecutive papers. 

### 3. Some papers which use variational inference to learn nonlinear dynamics and emission models in sequential data.

 - 3.1. [Structured Inference Networks for Nonlinear State Space Models](https://arxiv.org/pdf/1609.09869.pdf)

 - 3.2. [A Disentangled Recognition and Nonlinear Dynamics Model for Unsupervised Learning](https://arxiv.org/pdf/1710.05741.pdf)

After reading this papers you should know:

* How papers 1 and 2 were used in building the model structure and algorithm?
* What are the ways to improve on these papers and many other similar papers?

### 4. Some papers which use variational inference to disentangle the latent factor representation. These are examples on how we manipulate the latent factors and inject our knowledge to the cost function within variational methods to enforce the latent representation to have specific characteristics. 

 - 4.1. [β-VAE: LEARNING BASIC VISUAL CONCEPTS WITH A CONSTRAINED VARIATIONAL FRAMEWORK](https://openreview.net/pdf?id=Sy2fzU9gl)

 - 4.2. [Understanding disentangling in β-VAE](https://arxiv.org/pdf/1804.03599.pdf)

 - 4.3. [Isolating Sources of Disentanglement in Variational Autoencoders](https://arxiv.org/pdf/1802.04942.pdf)

After reading this papers you should know:

* How paper 2 were modified in building the model structure and algorithm? Where do we inject our knowledge to make the network learn better (or of interest) representations?
* What are the ways to improve on these papers and many other similar papers?
