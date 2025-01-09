---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---


<p align="justify">My research revolves around <b>probability</b>, <b>information theory</b>, and <b>mathematical statistics</b>. I have applied these tools to cosmology, machine learning, the origin of life, population genetics, and infectious diseases. I also have a passion for the philosophy of science, which motivates a lot of my research.</p>

## Stable allocations
   
   <p align="justify">I have studied percolation and large deviations properties of stable allocations to Poisson points. To gain intuition, imagine a set of random points, or "centers," in the space. Assume that every center desires to colonize a random amount of territory as close to it as possible. To acquire territory, all centers grow a ball around them that expands at the same speed so that (a) each center colonizes all the territory in the ball that any other center did not previously colonize and (b) each center stops growing its ball only when it has colonized the territory it desired. This stochastic process generalizes to continuous spaces the famous <a href="https://www.eecs.harvard.edu/cs286r/courses/fall09/papers/galeshapley.pdf">Gale—Shapley algorithm</a> for which Lloyd Shapley received the Nobel Prize in 2012.</p> 

   <div>
      <center>
         <img src="https://github.com/user-attachments/assets/dbfd1f4b-fd22-41da-9fc2-56098e6cc7fa" width="300" height="300">
      </center>   
      <p style="text-align: center"><font size="2"><b>Figure 1:</b> A stable allocation to a Poisson process of intensity 1 where each center wants to colonize a territory whose expected volume is 1.<br> Simulation performed by chatgpt.</font></p>
   </div>


### Relevant publications

<font size="3">
<ul> 
   <li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b>. Percolation for the stable marriage of Poisson and Lebesgue with random appetites. <i>Stochastics</i>, 85(2):252–261, 2013. <a href="https://www.tandfonline.com/doi/abs/10.1080/17442508.2011.651215"> [Journal]</a> <a href="https://arxiv.org/pdf/0909.5325.pdf">[arχiv]</a></li> 
   
   <li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b>. A note on large deviations for the stable marriage of Poisson and Lebesgue with random appetites. <i>Journal of Theoretical Probability</i>, 25(1):77–91, 2012. <a href="https://link.springer.com/article/10.1007/s10959-010-0304-9">[Journal]</a> <a href="https://arxiv.org/pdf/0911.1429.pdf">[arχiv]</a></li>
</ul></font>


## Local measures of information

<p align="justify">Shannon's information theory is almost exclusively focused on global averaged measures of information (entropy, mutual information, KL divergence, etc.) This approach overlooks the significance of local and unaveraged information measures of specific events. Paradoxically, since averages are by definition a reduction of information, information theory is constantly losing information. Consider, for instance, the active information
\begin{equation}
  I^+(\mathsf A) := \log \frac{\mathbf P(\mathsf A)}{\mathbf P_0(\mathsf A)},
   \label{AIN}
\end{equation}
where $\mathbf P$ and $\mathbf P_0$ are probability measures on a measurable space $(\Omega, \mathcal F)$ and $\mathsf A \subset \mathcal F$. In words, $I^+(\mathsf A)$ measures how  much information is added/removed from the event $\mathsf A$ when it is measured with $\mathbf P$, instead of the baseline $\mathbf P_0$. In more detail, $I^+(\mathsf A)$ will be positive/negative/zero, when $\mathbf P(\mathsf A)$ is bigger/smaller/equal to $\mathbf P_0$, respectively. By contrast, the Kullback-Leibler divergence $\mathrm{KL}(\mathbf P \mid \mathbf P_0)$ is a nonnegative global average that can only be zero when $\mathbf P = \mathbf P_0$. These differences matter, as explained in all projects below, which shows that progress has been hindered in many areas by ignoring local or unaveraged measures of information.</p>

<div>
   <center>
   <img src="https://github.com/user-attachments/assets/012796d6-9a9d-4a3d-ad02-75ac7e0365b1" style="width:40%">
   <img src="https://github.com/user-attachments/assets/7efca092-254d-46a5-8836-cfec05117fe4" style="width:40%">
   </center>    
   <p style="text-align: justify"><font size="2"><b>Figure 2:</b> The LHS depicts the different values of the Kullback-Leibler divergence between any two probability measures on a space $\Omega=\{\omega_1, \omega_2\}$ with two states: $\mathrm{KL}(\mathbf P \mid \mathbf P_0) = \mathbf P(\omega_1)\log[\mathbf P(\omega_1)/\mathbf P(\omega_1)] + \mathbf P(\omega_2)\log[\mathbf P(\omega_2)/\mathbf P(\omega_2)]$. Observe that the KL divergence is zero only when $\mathbf P = \mathbf P_0$; anywhere else, it is positive. On the same space, the RHS depicts the different values of the total active information, defined as 
$\mathbf I^+(\mathbf P \mid \mathbf P_0) :=  \log[\mathbf P(\omega_1)/\mathbf P_0(\omega_1)] + \log[\mathbf P(\omega_2)/\mathbf P_0(\omega_2)]$. Notice that the total active information can be negative.</font></p> 
</div>

### Relevant publications

<font size="3"><ul> 
<li style="text-align: justify">Ola Hössjer, <b>Daniel Andrés Díaz-Pachón</b>, Chen Zhao, and J. Sunil Rao. An Information Theoretic Approach to Prevalence Estimation and Missing Data. <i>IEEE Transactions on Information Theory</i>, 70(5):3567–3582, 2024. <a href="https://ieeexplore.ieee.org/abstract/document/10295527">[Journal]</a> <a href="https://arxiv.org/pdf/2206.05120.pdf">[arχiv]</a></li> 

<li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b> and Ola Hössjer. Assessing, testing, and estimating the amount of fine-tuning by means of active information. <i>Entropy</i>, 24(10):1323, 2022 (<b>Editor’s choice article</b>). <a href="https://www.mdpi.com/1099-4300/24/10/1323">[Journal]</a> (Open source)</li>

<li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b> and Robert J. Marks II. Generalized active information: Extensions to unbounded domains. <i>BIO-Complexity</i>, 2020(3):1–6, 2020. <a href="https://bio-complexity.org/ojs/index.php/main/article/view/BIO-C.2020.3/BIO-C.2020.3">[Journal]</a> (Open source)</li>

<li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b>, Juan P. Sáenz, and J. Sunil Rao. Hypothesis testing with active information. <i>Statistics & Probability Letters</i>, 161:108742, 2020. <a href="https://www.sciencedirect.com/science/article/abs/pii/S0167715220300456">[Journal]</a> <a href="https://arxiv.org/pdf/2011.04834.pdf">[arχiv]</a></li>
</ul></font> 

   
## Fine-tuning

<p align="justify">Cosmological fine-tuning (FT) states that some constants of nature must pertain to intervals of minuscule probability in
order to permit the existence of carbon-based life. The problem is twofold for each constant of nature: First, finding the constant's life permitting interval (LPI)—the set of possible values of the constant that would permit life (a physics problem); second, finding the probability that the constant of nature pertains to its LPI (a mathematical problem). When this probability is small, there is fine-tuning. However, the second step remained elusive for 50 years, as estimating the probability of the LPI required using a sample of size 1 (the value of the constant in our <i>uni</i>-verse), taken from an unknown distribution, supported in an unknown sample space, where the sample is affected by selection bias because it corresponds to a universe that permits life. My colleagues and I developed a sound solution to this problem through a Bayesian approach that relies on maximum entropy and optimization.</p> 

<p align="justify">Moreover, as many question whether the study of fine-tuning is a proper scientific endeavor, we proved the following principle: the fine-tuning of a constant of nature can only be known when the parameter takes nonnegative values and when the size of the LPI is small relative to the observed value of the constant in our universe. This happens for at least two important constants of nature: the critical density of the universe and the gravitational force. However, our method also says that the exact level of tuning of other constants which have been touted as fine-tuned cannot be known; this is the case, for instance, of the Higgs vacuum expectation value and the amplitude of primordial fluctuations (a nice presentation can be watched <a href="https://www.youtube.com/watch?v=3_ZrLrrSTTE">here</a>).</p>

<p align="justify">In terms of \eqref{AIN}, we say that there is fine-tuning when $I^+(\mathsf A)$ is large, for $\mathsf A$ the LPI of a given constant, $\mathbf P$ is a distribution highly concentrated in $\mathsf A$, and $\mathbf P_0$ is an upper bound of a maximum entropy distribution.</p>

<div>
      <center>
         <img src="https://github.com/user-attachments/assets/890bda35-ad28-42c4-b5dd-526b74fd8b54" width="500" height="500">
      </center>   
      <p style="text-align: justify"><font size="2"><b>Figure 3:</b> The reason we cannot know the level of tuning of a constant that can take any real value. The Bayesian approach first considers all distributions that belong to a certain family (say, the normal family of distributions), then it maximizes the probability of the LPI among all members of the family. Thus, if the LPI includes the mean value (as in the left-hand side), the estimated upper bound of the probability of the LPI tends to 1 as the variance approaches 0.</font></p>
   </div>

   ### Relevant publications

<font size="3"><ul> 
<li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b>, Ola Hössjer, and Calvin Mathew. Is It Possible to Know Cosmological
Fine-Tuning? <i>The Astrophysical Journal Supplement Series</i>, 271(2):56, 2024. <a href="https://iopscience.iop.org/article/10.3847/1538-4365/ad2c88">[Journal]</a> (Open source)</li> 

<li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b>, Ola Hössjer, and Robert J. Marks II. Sometimes size does not matter.
<i>Foundations of Physics</i>. 53,1, 2023. <a href="https://link.springer.com/article/10.1007/s10701-022-00650-1">[Journal]</a> <a href="https://github.com/danielandresgp/danielandresgp.github.io/blob/master/files/Size%20does%20not%20matter.pdf">[Preprint]</a> < a href="https://github.com/danielandresgp/danielandresgp.github.io/blob/master/files/Poster.pdf">[Poster]</a></li>

<li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b> and Ola Hössjer. Assessing, testing, and estimating the amount of fine-tuning by means of active information. <i>Entropy</i>, 24(10):1323, 2022 (<b>Editor’s choice article</b>). <a href="https://www.mdpi.com/1099-4300/24/10/1323">[Journal]</a> (Open source)</li>

<li style="text-align: justify"><b>Daniel Andrés Díaz-Pachón</b>, Ola Hössjer, and Robert J. Marks II. Is cosmological tuning fine or
coarse? <i>Journal of Cosmology and Astroparticle Physics</i>, JCAP07(2021)020, 2021. <a href="https://iopscience.iop.org/article/10.1088/1475-7516/2021/07/020">[Journal]</a> <a href="https://arxiv.org/pdf/2104.05400.pdf">[arχiv]</a></li>
</ul></font> 


## COVID-19

<p align="justify">During the COVID-19 pandemic, understanding the true prevalence of the virus was critical, but biased sampling hindered accurate estimations. Specifically, I realized that symptomatic individuals were more likely to seek testing. This bias led to overestimation of prevalence in First-World countries... and the subsequent adoption of horrible lockdown policies! Using the maximum entropy principle, my colleagues and I introduced corrected estimators as readily implementable algorithms directed to practitioners, while providing theoretical guarantees for our corrections. More specifically, we developed corrected estimators in the following cases: when all the symptomatic individuals are tested (as it was the case in most universities and companies in the US during the pandemic) and when not all the symptomatic individuals are tested but are still overrepresented in the sample, considering in the two cases the presence and absence of testing errors.</p>

<p align="justify">In terms of \eqref{AIN}, we define the informational bias using $I^+(\mathsf A)$, where $\mathsf A$ corresponds to the infected group, $\mathbf P_0(\mathsf A)$ is the actual prevalence of infected individuals, and $\mathbf P(\mathsf A)$ is a given estimator of prevalence. The estimator is unbiased when the statistics $I^+(\mathsf A)$ is close to 0, it has positive bias when $I^+(\mathsf A) > 0$, and it has negative bias when $I^+(\mathsf A) < 0$.</p>

<div>
   <center>
   <img src="https://github.com/user-attachments/assets/93dc2395-5cea-45c2-b048-02ec1e88781d" style="width:45%">
   <img src="https://github.com/user-attachments/assets/40f64213-1be6-40ed-bd99-0be26b85f970" style="width:45%">
   </center>    
   <p style="text-align: justify"><font size="2"><b>Figure 4:</b> Boxplots of a simulation of prevalence estimators when the true prevalence is 20%, false positive and false negative rates for the asymptomatic group are, respectively, 1% and 20%, and false positive and false negative rates of symptomatic individuals are, respectively, 3% and 2%. The X axis represents increasing proportions of asymptomatic individuals being sampled. The LHS shows boxplots of estimators when all the symptomatic group is sampled (as it was the case in many universities and companies in First World countries). The RHS shows boxplots of estimators when 70% of the symptomatic population was sampled. In the two cases, the corrected estimator of prevalence greatly reduces the naive estimator.</font></p> 
</div>



## Clustering

<p align="justify">Since my days as a postdoc, I started working on machine learning problems related to bump-hunting. Even though a unified definition of a cluster (or bump) is elusive, we can still use \eqref{AIN} to detect a cluster. Indeed, it is clear that if $\Omega$ is bounded, it will not contain clusters when the data is uniformly distributed. For $\mathbf P$ and $\mathbf P_0$ the empirical and uniform distributions over $\Omega$, this is equivalent to saying that there is a cluster in $\mathsf A \subset \Omega$ if the active information $I^+(\mathsf A) > 0$, or in $\mathsf A^c$ if $I^+(\mathsf A) < 0$ (importantly, by contrast, the Kullback-Leibler divergence can only detect the existence of a cluster in $\Omega$ but not its location). Accordingly, in my first approach I have developed algorithms, with their respective statistical guarantees, using $I^+(\mathsf A)$ as a test statistic for cluster detection in different regions of $\Omega$. My second approach uses spectral algorithms for the detection of clusters, but I do it with a twist: I realized that as the leading eigenvectors correspond to larger variances, data must be more clustered in the dimensions corresponding to the eigenvectors with the smallest eigenvalues, that we call <i>pettiest components</i>.</p>

<div>
   <center>
   <img src="https://github.com/user-attachments/assets/9d5ad9cd-1a42-43cc-a87a-bdca3ce9c8c2" style="width:25%"> &nbsp; &nbsp; &nbsp; &nbsp; 
   <img src="https://github.com/user-attachments/assets/8ace7357-8f00-4c7d-ba58-1fe047708899" style="width:25%">
   </center>    
   <p style="text-align: justify"><font size="2"><b>Figure 4:</b> Using the famous MNIST database of handwritten digits, the left-hand side shows equidistant points of the digit 1 inside the cluster found using principal components, while the right-hand side shows equidistant points for the same digit inside the cluster found using pettiest components.</font></p> 
</div>


## Learning and knowledge acquisition

<p align="justify">Philosophers usually define knowledge as "justified true belief." This means that an agent $\mathcal A$ <i>knows</i> a proposition $p$ if the following three properties are satisfied:</p>
1. $\mathcal A$ believes $p$,
2. $p$ is true,
3. $\mathcal A$'s belief about $p$ is justified.
<p align="justify">If only properties 1–2 are satisfied, $\mathcal A$ <i>learns</i> $p$. Clearly, acquiring knowledge requires more than learning. We have applied \eqref{AIN} to formalize the concepts 1–3 behind learning and knowledge acquisition. To this end, it is assumed that $\Omega$ is a set of parameters of a statistical model; in this context, we take a mixed frequentist and Bayesian approach. On the one hand, it is postulated that one element $\omega_0\in\Omega$ is the true parameter value (a frequentist assumption). On the other hand, uncertainty about $\omega_0$ is formulated as a probability measure on $\Omega$ that varies between persons (a Bayesian assumption). More specifically, $\mathbf P$ and $\mathbf P_0$ represent degrees of beliefs about $\omega_0\in\Omega$, of an agent $\mathcal A$ and an ignorant agent $\mathcal I$, respectively. It is assumed that $\mathcal A$ acquired data $\mathsf D$ that $\mathcal I$ lacks, so that $\mathbf P$ and $\mathbf P_0$ are posterior and prior distributions on $\Omega$ that represent degrees of beliefs of $\mathcal A$ about $\omega_0$, after and before he received data. In particular, if we choose $\mathsf A$ as the set of parameter values for which a given proposition $p$ is true, then the objective of $\mathcal A$ is to use data to learn whether the proposition is true ($\omega_0\in \mathsf A$) or not ($\omega_0 \notin \mathsf A$). In this case, data represents the exogenous information that helps agent $\mathcal A$ modify his beliefs about $\mathsf A$ compared to the ignorant person $\mathcal I$. Knowledge acquisition goes beyond learning since it additionally requires that $\mathcal A$ learns about the proposition for the right reason. This corresponds to increasingly correct beliefs about $\omega_0$, not only increasingly correct beliefs of whether $\omega_0\in\mathsf A$ or not (as for learning).</p> 

<p align="justify">Our approach proposes a very sensible solution to the old dispute between Bayesians and frequentists. We consider propositions and states of reality that are objectively true or false, but learning and knowledge are naturally Bayesian. Thus, ontology is partially frequentist, whereas epistemology is Bayesian. Our definitions differentiate between them, and this is an essential aspect of our theory.</p> 

<div>
      <center>
         <img src="https://github.com/user-attachments/assets/7fb8f0fc-789e-4eaf-983d-52ca0a896b9d" width="500" height="500">
      </center>   
      <p style="text-align: justify"><font size="2"><b>Figure 5:</b> The set of possible worlds is $\Omega=[0,1]$, the set of worlds where a given proposition $p$ is true is given by $\mathsf A$, the true world is $\omega_0$, and $\mathbf P_0$ is the uniform measure. Thus $\mathbf P_0(\mathsf A) = \textrm{length}(\mathsf A) < 1$. The light blue region in the LHS represents the beliefs of an agent $\mathcal A_1$, whereas the gray region in the RHS represents the beliefs of another agent $\mathcal A_2$. Since the beliefs of the two agents are fully concentrated in $\mathsf A$, $\mathbf P_{\mathcal A_1}(\mathsf A) = \mathbf P_{\mathcal A_2}(\mathsf A) = 1$. Therefore, the two agents fully learned about proposition $p$. However, since in the RHS $\omega_0 \notin \textrm{supp}(\mathbf P_{\mathcal A_2})$, agent $\mathcal A_2$ does not acquire knowledge, whereas agent $\mathcal A_1$ does as his beliefs are more concentrated around $\omega_0$ than those of the ignorant agent with belief $\mathbf P_0$. Nonetheless, full knowledge is not possible for $\mathcal A_1$ as $\mathbf P_{\mathcal A_1}$ is continuous.</font></p>
   </div>
