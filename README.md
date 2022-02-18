# nice-reads

## Machine learning (ML) and Artificial intelligence (AI) blog posts
Here, I provide pointers to keep updated with the progress in ML and AI.
### 1. [OpenAI blog](https://openai.com/blog/?utm_source=towardsai.net&utm_medium=referral&utm_campaign=marketing&utm_term=machine-learning-blog&utm_content=best-machine-learning-blogs-to-follow) - a list of recent projects/publications at OpenAI
### 2. [Distill](https://distill.pub/?utm_source=towardsai.net&utm_medium=referral&utm_campaign=marketing&utm_term=machine-learning-blog&utm_content=best-machine-learning-blogs-to-follow) - includes clean & nice tutorial on various subjects - few posts but super high quality
### 3. [Google AI blog](https://ai.googleblog.com/) - a list of recent projects/publications at Google AI
### 4. [Amazon's science blog](https://www.amazon.science/blog?utm_source=towardsai.net&utm_medium=referral&utm_campaign=marketing&utm_term=machine+learning+blog&utm_content=machine+learning+blog&f0=0000016e-2ff1-d205-a5ef-aff9651e0000&s=0) - a list of recent projects/publications at Amazon
### 5. [Eric Jang's blog](https://blog.evjang.com/) - amazing posts on various topics - few posts but high quality
### 6. [Lilian weng's blog](https://lilianweng.github.io/lil-log/) - amazing posts on various topics - few posts but high quality
### 7. [Chris Olah's blog](https://colah.github.io/about.html) - amazing posts on various topics - few posts but high quality
### 8. [Machine learning is fun](https://www.machinelearningisfun.com/) - various posts, might require Medium membership
### 9. [Machine learning mastery](https://machinelearningmastery.com/blog/) - A lot of posts, mostly coding oriented
### 10. AI research groups in various universities
* [BAIR](https://bair.berkeley.edu/blog/?utm_source=towardsai.net&utm_medium=referral&utm_campaign=marketing&utm_term=machine-learning-blog&utm_content=best-machine-learning-blogs-to-follow)
* [MLCMU](https://blog.ml.cmu.edu/?utm_source=towardsai.net&utm_medium=referral&utm_campaign=marketing&utm_term=machine-learning-blog&utm_content=best-machine-learning-blogs-to-follow)

## Study material
Some of the study materials are quick cheat sheets. The point of these cheat sheets is to brush up your memory on these topics; memorizing the formulas/conclusions are highly discouraged :D. Instead, we'd like to understand the fundamentals. Please only use the cheat sheets for quick review of the material.
### 1. Probability & statistics
* [CME106 cheat sheet](https://stanford.edu/~shervine/teaching/cme-106/)

### 2. Machine learning
* [CS229  cheat sheet](https://stanford.edu/~shervine/teaching/cs-229/cheatsheet-supervised-learning)
### 3. Artificial Intelligence
* [CS221 cheat sheet](https://stanford.edu/~shervine/teaching/cs-221/)
### 4. Deep learning
* [CS230 cheat sheet](https://stanford.edu/~shervine/teaching/cs-230/)
* [CMU DL course](https://deeplearning.cs.cmu.edu/S22/index.html)
* [Stanford DL course](https://cs230.stanford.edu/)
* [fastai book/Jupyter notebooks](https://github.com/fastai/fastbook) -> interactive learning, highly recommended
### 5. Vaious data science materials
* [Data Science Tools](https://www.mit.edu/~amidi/teaching/data-science-tools/)
### 6. Python/coding
I'm personally against cheat sheets to learn coding/programming languages, you only learn them by writing codes for problems/projects :). The point is not memorizing syntaxes, we can always look them up. The cheat sheets are only meant for quick reviews. 
* [matplotlib cheat sheet](https://datacamp-community-prod.s3.amazonaws.com/28b8210c-60cc-4f13-b0b4-5b4f2ad4790b)
* [SQL cheat sheet](https://learnsql.com/blog/sql-basics-cheat-sheet/)
* [pandas cheat sheet](http://datacamp-community-prod.s3.amazonaws.com/dbed353d-2757-4617-8206-8767ab379ab3)

## Variational inference, idea and methods 
Here, I provide some papers about variational inference; why do we need it and how do we use it? 

### 1. [Variational Inference: A Review for Statisticians](https://arxiv.org/pdf/1601.00670.pdf) - a review paper on variational inference. 

After reading this paper you should know:
* What is variational inference?
* Why do we even need variational inference and how do we use it?
* What is the evidence lower bound? The intution behind its components? More to think: what is the relationship between the evidence lower bound and expectation-maximization (EM) algorithm? Also see Matthew Beal's great [PhD thesis](https://cse.buffalo.edu/faculty/mbeal/papers/beal03.pdf) 
* What is mean-field approximation?

### 2. [Auto-Encoding Variational Bayes](https://arxiv.org/pdf/1312.6114.pdf) - A nice usage of variatonal inference, introducing reparametrization trick.

This paper introduces the reparameterization trick which enables computing gradient of the parameters of the posterior distribution on a expectation operator of any function of posterior distribution. After reading this paper you should know:

* A sample usage of variational inference to estimate an intractable distribution? Also see Diederik Kingma's great [PhD Thesis](https://www.dropbox.com/s/v6ua3d9yt44vgb3/cover_and_thesis.pdf?dl=0)
* What is the cost function when the prior distibution of the latent factors is assumed to be Gaussian?
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
