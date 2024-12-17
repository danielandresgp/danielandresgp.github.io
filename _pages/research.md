---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---


My research revolves around **probability** and **information theory**. I have applied these tools to cosmology, machine learning, statistics, and infectious disesaes, among others. I also have a penchant for the philosophy of science, which motivates a lot of my research. 

## Probability

In mathematical research, probability is the apple of my eye. I really, really, like probability and stochastic processes! Some areas in which I have worked in the past are:

1. **Stable allocations**: Imagine you have a set of points in the space. Assume that every point wants to colonize a territory of the space with a random volume which is as close to the point as possible. To acquire their territory, all points grow around them a ball that increases at the same radial speed in such a way that (a) each point claims for itself all the territory in the ball around it that has not claimed by any other point, and (b) each point stops growing its ball only when it has claimed for itself a territory it wanted to colonize. This informal presentation describes stable allocations, a stochastic process that generalizes to continuous spaces the famous Gale—Shapley algorithm for which Lloyd Shapley received the Nobel Prize in 2012. See [here](https://github.com/user-attachments/assets/dbfd1f4b-fd22-41da-9fc2-56098e6cc7fa) a cool simulation I did with chatgpt!).

I have studied percolation and large deviations properties of stable allocations. My interests is now twofold: first, studying the connection between stable allocations and continuous $\Xi$-Fleming—Viot processes, and its  applications to population genetics and epidemics modeling; second, studying percolation of other models and graphs, as this my favorite topic in all of probability! 


Most of my research revolves around local measures of information, like the active information
\begin{equation}
  I^+ := \log \frac{\mathbf P(\mathsf A)}{\mathbf P_0(\mathsf A)},
\end{equation}
where $\mathbf P$ and $\mathbf P_0$ are probability measures on a measurable space $(\Omega, \mathcal F)$ and $\mathsf A \subset \mathcal F$.
1. **Fine-tuning**: Cosmological fine-tuning (FT) states that some constants of nature must pertain to intervals of minuscule probability in
order to permit the existence of carbon-based life. The problem is twofold for each constant of nature: First, finding the constant's life permitting interval (LPI)---the set of possible values of the constant that would permit life (a physics problem); second, finding the probability that the constant of nature pertains to its LPI (a mathematical problem). When this probability is small, there is fine-tuning. However, the second step remained elusive for 50 years, as estimating the probability of the LPI required using a sample of size 1 (the value of the constant in our _uni_-verse), taken from an unknown distribution, supported in an unknown sample space, where the sample is affected by selection bias because it corresponds to a universe that permits life. My colleagues and I developed a sound solution to this problem through a Bayesian approach that relies on maximum entropy and optimization (a nice presentation can be watched [here](https://www.youtube.com/watch?v=3_ZrLrrSTTE)). I am now interested in estimating the probabilities of LPIs for more local conditions (as oposed to the universal ones determined by the constants of nature), like gallactic, planetary, and biological ones. 
2. **COVID-19**: During the COVID-19 pandemic, understanding the true prevalence of the virus was critical, but biased sampling hindered accurate estimations. Specifically, I realized that symptomatic individuals were more likely to seek testing. This bias led to overestimation of prevalence in first-world countries... and their subsequent adoption of horrible public health policies! Using the maximum entropy principle, my colleagues and I introduced corrected estimators as readily implementable algorithms directed to practitioners, while providing theoretical guarantees for our corrections. Among others, I am now interested in implementing these developments to artificial intelligence, where biases of algorithms are a huge ethical problem.
3. **Clustering**: Since my days as a postdoc, I started working on machine learning problems related to bump-hunting. A unified definition of a cluster (or bump) is elusive. Nonetheless, it is clear that if $\mathsf S$ is bounded, it will not contain clusters when the data is uniformly distributed. For $\mathbf P$ and $\mathbf P_0$ the empirical and uniform distributions over $\mathsf S$, this is equivalent to saying that there is a cluster in $\mathsf A \subset \mathsf S$ if the active information $$I^+(\mathsf A) := \log \frac{\mathbf{P}(\mathsf A)}{\mathbf{P}_0(\mathsf A)}> 0$$, or in $\mathsf A^c$ if $I^+(\mathsf A) < 0$ (importantly, by contrast, the KL divergence, an averaged global measure, can only detect the existence of a cluster in $\mathsf S$ but not its location). Accordingly, in my first approach I have developed algorithms using $I^+(\mathsf A)$ as a test statistic for cluster detection in different regions of $\mathsf S$, offering guarantees for these algorithms. My second approach uses spectral algorithms for the detection of clusters... with a twist: I realized that as the leading eigenvectors correspond to larger variances, then data must be more clustered in the dimensions corresponding to the eigenvectors with the smallest eigenvalues
