---
permalink: /
title: "About me"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## Welcome!

I live in beautiful South Florida, where I work as Research Assistant Professor in the [Division of Biostatistics and Bioinformatics](https://www.publichealth.med.miami.edu/divisions/biostatistics/) at the University of Miami. 

My current research revolves around **probability** and **information theory**, with applications to machine learning, physics, statistics, and infectious disesaes, among others. I also have a penchant for the philosophy of science, which motivates a lot of my research. I have worked on the following areas:

1. **Fine-tuning**: Cosmological fine-tuning (FT) states that some constants of nature must pertain to intervals of minuscule probability in
order to permit the existence of carbon-based life. The problem is twofold for each constant of nature: First, finding the constant's life permitting interval (LPI)——the set of possible values of the constant that would permit life (a physics problem); second, finding the probability that the constant of nature pertains to its LPI (a mathematical problem). When this probability is small, there is fine-tuning. However, the second step remained elusive for 50 years, as estimating the probability of the LPI required using a sample of size 1 (the value of the constant in our _uni_-verse), taken from an unknown distribution, supported in an unknown sample space, where the sample is affected by selection bias because it corresponds to a universe that permits life. My colleagues and I developed a sound solution to this problem through a Bayesian approach that relies on maximum entropy and optimization (a nice presentation can be watched [here](https://www.youtube.com/watch?v=3_ZrLrrSTTE). I am now interested in estimating the probabilities of LPIs for more local conditions (as oposed to the universal ones determined by the constants of nature), like gallactic, planetary, and biological ones. 
2. **Stable allocations**: Imagine you have a set of points $Z$ in some Euclidean space (formally, $Z \subset \mathbb R^d$ is a Poisson process of intensity $\lambda$). Assume that every point in $\zeta \in Z$ desires for itself a territory of random volume $V_\zeta \subset \mathbb R^d$, which is as close to it as possible. To acquire their territory, all points grow around them a ball that increases at the same radial speed in such a way that (a) each point claims for itself all territory in the ball around it that any other point has not claimed, and (b) each point stops growing its ball only when it has claimed for itself a territory of volume $V$ . This informal presentation describes the stable marriage of Poisson and Lebesgue, a stochastic process that generalizes to continuous spaces the famous Gale—Shapley algorithm for which Lloyd Shapley received the Nobel Prize in 2012. See [here](https://github.com/user-attachments/assets/dbfd1f4b-fd22-41da-9fc2-56098e6cc7fa) a cool simulation done with chatgpt. I have studied percolation and large deviations properties of stable allocations. My interests is now twofold: first, studying the connection between stable allocations and continuous $\Xi$-Fleming—Viot processes, and its  applications to population genetics and epidemics modeling; second, studying percolation of other models and graphs as this my favorite topic in all of probability! 
3. **COVID-19**: During the COVID-19 pandemic, understanding the true prevalence of the virus was critical, but biased sampling hindered accurate estimations. Specifically, I realized that symptomatic individuals were more likely to seek testing. This bias led to overestimation of prevalence in first-world countries... and their subsequent adoption of horrible public health policies! Using the maximum entropy principle, my colleagues and I introduced corrected estimators as readily implementable algorithms directed to practitioners, while providing theoretical guarantees for our corrections. Among others, I am now interested in implementing these developments to artificial intelligence, where biases of algorithms are a huge ethical problem.
4. **Clustering**: Since my days as a postdoc, I started working on machine learning problems related to bump-hunting. A unified definition of a cluster (or bump) is elusive. Nonetheless, it is clear that if $\mathsf S$ is bounded, it will not contain clusters when the data is uniformly distributed. For $\mathbf P$ and $\mathbf P_0$ the empirical and uniform distributions over $\mathsf S$, this is equivalent to saying that there is a cluster in $\mathsf A \subset \mathsf S$ if the active information $I^+(\mathsf A) = \log (\mathbf{P}(\mathsf A)/ \mathbf{P}_0(\mathsf A))> 0$, or in $\mathsf A^c$ if $I^+(\mathsf A) < 0$ (importantly, by contrast, the KL divergence, an averaged global measure, can only detect the existence of a cluster in $\mathsf S$ but not its location). Accordingly, I have developed algorithms for business applications using $I^+(\mathsf A)$ as a test statistic for cluster detection in different regions of $\mathsf S$, offering guarantees for these algorithms.

---

Besides research, my hobbies are crossfit, reading, and writing.

I am happily married to Lis. She is much more than I could ever deserve! We have a beautiful baby boy called Juan Pablo, our [mustard seed](https://www.biblegateway.com/passage/?search=Mateo+13%3A31-32&version=NIV).

The most significant aspect of my life is that I love Jesus, but not as much as [He loves me](https://www.biblegateway.com/passage/?search=John%203%3A16&version=NIV)! If you are interested, we can talk about it!
