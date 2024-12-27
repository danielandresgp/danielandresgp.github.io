---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---


<p align="justify">My research revolves around <b>probability</b>, <b>information theory</b>, and <b>mathematical statistics</b>. I have applied these tools to cosmology, machine learning, origin of life, population genetics, and infectious diseases. I also have a penchant for the philosophy of science, which motivates a lot of my research. </p>

## Stable allocations
   
   <p align="justify">I have studied <a href="https://arxiv.org/pdf/0909.5325">percolation</a> and <a href="https://arxiv.org/pdf/0911.1429">large deviations</a> properties of stable allocations to Poisson points. To get an intuition, imagine that you have a set of random points, or "centers", in the space. Assume that every center wants to colonize a random amount of territory which is as close to it as possible. To acquire territory, all centers grow around them a ball that increases its size at the same speed in such a way that (a) each center colonizes all the territory in the ball that was not previously colonized by any other center, and (b) each center stops growing its ball only when it has colonized the amount of territory it wanted to have. This stochastic process generalizes to continuous spaces the famous <a href="https://www.eecs.harvard.edu/cs286r/courses/fall09/papers/galeshapley.pdf">Gale—Shapley algorithm</a> for which Lloyd Shapley received the Nobel Prize in 2012.</p> 

   <div>
      <center>
         <img src="https://github.com/user-attachments/assets/dbfd1f4b-fd22-41da-9fc2-56098e6cc7fa" width="300" height="300">
      </center>   
      <p style="text-align: center"><font size="2"><b>Figure 1:</b> A stable allocation to a Poisson process of intensity 1 where each center wants to colonize a territory whose expected volume is 1.<br> Simulation performed by chatgpt.</font></p>
   </div>


## Local measures of information

<p align="justify">Shannon's information theory is almost exclusively focused on global averaged measures of information (entropy, mutual information, KL divergence, etc.) This approach overlooks the significance of local and unaveraged information measures of specific events. Paradoxically, since averages are by definition a reduction of information, information theory is constantly losing information. Consider, for instance, the <a href="https://arxiv.org/pdf/2111.06865">active information</a>
\begin{equation}
  I^+(\mathsf A) := \log \frac{\mathbf P(\mathsf A)}{\mathbf P_0(\mathsf A)},
   \label{AIN}
\end{equation}
where $\mathbf P$ and $\mathbf P_0$ are probability measures on a measurable space $(\Omega, \mathcal F)$ and $\mathsf A \subset \mathcal F$. In words, $I^+(\mathsf A)$ measures how  much information is added/removed from the event $\mathsf A$ when it is measured with $\mathbf P$, instead of the baseline $\mathbf P_0$. In more detail, $I^+(\mathsf A)$ will be positive/negative/zero, when $\mathbf P(\mathsf A)$ is bigger/smaller/equal to $\mathbf P_0$, respectively. By contrast, the Kullback-Leibler divergence $\mathrm{KL}(\mathbf P \mid \mathbf P_0)$ is a nonnegative global average that can only be zero when $\mathbf P = \mathbf P_0$ with probability 1. Most of what follows shows that these differences matter, and that progress has been hindered in many areas by ignoring local measures of information.</p>

<div>
   <center>
   <img src="https://github.com/user-attachments/assets/012796d6-9a9d-4a3d-ad02-75ac7e0365b1" style="width:40%">
   <img src="https://github.com/user-attachments/assets/7efca092-254d-46a5-8836-cfec05117fe4" style="width:40%">
   </center>    
   <p style="text-align: justify"><font size="2"><b>Figure 2:</b> The LHS depicts the different values of the Kullback-Leibler divergence between any two probability measures on a space $\Omega=\{\omega_1, \omega_2\}$ with two states: $\mathrm{KL}(\mathbf P \mid \mathbf P_0) = \mathbf P(\omega_1)\log[\mathbf P(\omega_1)/\mathbf P(\omega_1)] + \mathbf P(\omega_2)\log[\mathbf P(\omega_2)/\mathbf P(\omega_2)]$. Observe that the KL divergence is zero only when $\mathbf P = \mathbf P_0$; anywhere else, it is positive. On the same space, the RHS depicts the different values of the total active information, defined as 
$\mathbf I^+(\mathbf P \mid \mathbf P_0) :=  \log[\mathbf P(\omega_1)/\mathbf P_0(\omega_1)] + \log[\mathbf P(\omega_2)/\mathbf P_0(\omega_2)]$. Notice that the total active information can be negative.</font></p> 
</div>


   
## Fine-tuning

<p align="justify">Cosmological fine-tuning (FT) states that some constants of nature must pertain to intervals of minuscule probability in
order to permit the existence of carbon-based life. The problem is twofold for each constant of nature: First, finding the constant's life permitting interval (LPI)—the set of possible values of the constant that would permit life (a physics problem); second, finding the probability that the constant of nature pertains to its LPI (a mathematical problem). When this probability is small, there is fine-tuning. However, the second step remained elusive for 50 years, as estimating the probability of the LPI required using a sample of size 1 (the value of the constant in our <i>uni</i>-verse), taken from an unknown distribution, supported in an unknown sample space, where the sample is affected by selection bias because it corresponds to a universe that permits life. My colleagues and I developed a sound solution to this problem through a Bayesian approach that relies on maximum entropy and optimization.</p> 

In terms of (1), we say that there is fine-tuning when $I^+(\mathsf A)$ is large, for $\mathsf A$ the LPI of a given constant, $\mathbf P$ is a distribution highly concentrated in $\mathsf A$, and $\mathbf P_0$ is an upper bound of a maximum entropy distribution.

<p align="justify">Moreover, as many question whether the study of fine-tuning is a proper scientific endeavor, we proved the following principle: the fine-tuning of a constant of nature can only be known when the parameter takes nonnegative values and when the size of the LPI is small relative to the observed value of the constant in our universe. This happens for at least two important constants of nature: the critical density of the universe and the gravitational force. However, our method also says that the exact level of tuning of other constants which have been touted as fine-tuned cannot be known; this is the case, for instance, of the Higgs vacuum expectation value and the amplitude of primordial fluctuations (a nice presentation can be watched <a href="https://www.youtube.com/watch?v=3_ZrLrrSTTE">here</a>).</p>

<div>
      <center>
         <img src="https://github.com/user-attachments/assets/890bda35-ad28-42c4-b5dd-526b74fd8b54" width="500" height="500">
      </center>   
      <p style="text-align: justify"><font size="2"><b>Figure 3:</b> The reason we cannot know the level of tuning of a constant that can take any real value. The Bayesian approach first considers all distributions that belong to a certain family (say, the normal family of distributions), then it maximizes the probability of the LPI among all members of the family. Thus, if the LPI includes the mean value (as in the left-hand side), the estimated upper bound of the probability of the LPI tends to 1 as the variance approaches 0.</font></p>
   </div>


## COVID-19

<p align="justify">During the COVID-19 pandemic, understanding the true prevalence of the virus was critical, but biased sampling hindered accurate estimations. Specifically, I realized that symptomatic individuals were more likely to seek testing. This bias led to overestimation of prevalence in First-World countries... and the subsequent adoption of horrible lockdown policies! Using the maximum entropy principle, my colleagues and I introduced corrected estimators as readily implementable algorithms directed to practitioners, while providing theoretical guarantees for our corrections. More specifically, we developed corrected estimators in the following cases: when all the symptomatic individuals are tested (as it was the case in most universities and companies in the US during the pandemic) and when not all the symptomatic individuals are tested but are still overrepresented in the sample, considering in the two cases the presence and absence of testing errors.</p>

<div>
   <center>
   <img src="https://github.com/user-attachments/assets/93dc2395-5cea-45c2-b048-02ec1e88781d" style="width:45%">
   <img src="https://github.com/user-attachments/assets/40f64213-1be6-40ed-bd99-0be26b85f970" style="width:45%">
   </center>    
   <p style="text-align: justify"><font size="2"><b>Figure 4:</b> Boxplots of a simulation of prevalence estimators when the true prevalence is 20%, false positive and false negative rates for the asymptomatic group are, respectively, 1% and 20%, and false positive and false negative rates of symptomatic individuals are, respectively, 3% and 2%. The X axis represents increasing proportions of asymptomatic individuals being sampled. The LHS shows boxplots of estimators when all the symptomatic group is sampled (as it was the case in many universities and companies in First World countries). The RHS shows boxplots of estimators when 70% of the symptomatic population was sampled. In the two cases, the corrected estimator of prevalence greatly reduces the naive estimator.</font></p> 
</div>



## Clustering

<p align="justify">Since my days as a postdoc, I started working on machine learning problems related to bump-hunting. A unified definition of a cluster (or bump) is elusive. Nonetheless, it is clear that if $\mathsf S$ is bounded, it will not contain clusters when the data is uniformly distributed. For $\mathbf P$ and $\mathbf P_0$ the empirical and uniform distributions over $\mathsf S$, this is equivalent to saying that there is a cluster in $\mathsf A \subset \mathsf S$ if the active information $I^+(\mathsf A) > 0$, or in $\mathsf A^c$ if $I^+(\mathsf A) < 0$ (importantly, by contrast, the KL divergence, an averaged global measure, can only detect the existence of a cluster in $\mathsf S$ but not its location). Accordingly, in my first approach I have developed algorithms using $I^+(\mathsf A)$ as a test statistic for cluster detection in different regions of $\mathsf S$, offering guarantees for these algorithms. My second approach uses spectral algorithms for the detection of clusters... with a twist: I realized that as the leading eigenvectors correspond to larger variances, then data must be more clustered in the dimensions corresponding to the eigenvectors with the smallest eigenvalues.</p>
