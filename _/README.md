## Atul Singh ARORA

 <img align="right" src ="https://user-images.githubusercontent.com/2003122/210131262-a28c9323-be40-4109-a8ad-0fc1f7a1870c.jpeg" width=190 /> 

<!-- <img align="right" src ="https://user-images.githubusercontent.com/2003122/210131194-0be951ce-4312-44e6-92fc-c8ad91bfa46e.jpeg" width=190 /> -->

I am a postdoctoral researcher at [Caltech](https://iqim.caltech.edu/people/postdocs/), working under the supervision of Thomas VIDICK (presently at [Weizmann](https://www.weizmann.ac.il/pages/)). 

I am fascinated by the emergence of physical insight from the application of quantum mechanics to solving computational or cryptographic tasks. I was initially drawn to the field by the possibility of having information theoretic security in certain cryptographic settings (e.g. key distribution, coin flipping). Currently, I am excited by the prospect of understanding and testing various aspects of quantum mechanics under computational assumptions (e.g. collapse binding, compressed oracle simulation, quantum depth). 

<sub> [ atul.singh.arora@gmail.com | asarora@caltech.edu ] </sub>



## Education

For my doctoral dissertation (Sep 2020), I was advised by Jérémie ROLAND at [Université libre de Bruxelles](http://quic.ulb.ac.be/members/past). I obtained my Bachelor's and Master's (May 2016) from [IISER Mohali](https://www.iisermohali.ac.in/students/people-sublinks/bs-ms-2011-batch), (India). I majored in physics and my master's thesis advisor was Prof Arvind. 

<sub>[ [curriculum vitae](https://atulsingharora.github.io/CV/cv.pdf) ] </sub>


<!-- 
|Awarded |Degree | Institute |
|-|-|-|
| Sep 2020 | PhD | *Université libre de Bruxelles*, Belgium. Advisor: Prof Jérémie ROLAND |
| May 2016 | BS-MS (Phys Maj) | *Indian Institute of Science Education and Research (IISER)*, Mohali, India. Master's thesis advisor: Prof Arvind | 
 -->


## Research

<details open>
<summary>

### Quantum Depth in the Random Oracle Model

*Atul Singh Arora, Andrea Coladangelo, Matthew Coudron, Alexandru Gheorghiu, Uttam Singh, Hendrik Waldner*

<sub> Oct 2022 [ [arXiv](https://arxiv.org/abs/2210.06454) | [GitHub](https://atulsingharora.github.io/instaDepth) ] —— [ [STOC '23](http://acm-stoc.org/stoc2023/accepted.html) ]  </sub>  
<sub>104 pages (+9 page Appendix), 10 figures
</summary>

> We give a comprehensive characterisation of the computational power of shallow quantum circuits combined with classical computation. Specifically, for classes of search problems, we show that the following statements hold, relative to a random oracle:  
(a) $\mathsf{BPP}^{\mathsf{QNC}^{\mathsf{BPP}}} \neq \mathsf{BQP}$. This refutes Jozsa's conjecture [QIP 05] in the random oracle model. As a result, this gives the first instantiatable separation between the classes by replacing the oracle with a cryptographic hash function, yielding a resolution to one of Aaronson's ten semi-grand challenges in quantum computing.  
(b) $\mathsf{BPP}^{\mathsf{QNC}} \nsubseteq \mathsf{QNC}^{\mathsf{BPP}}$ and $\mathsf{QNC}^{\mathsf{BPP}} \nsubseteq \mathsf{BPP}^{\mathsf{QNC}}$. This shows that there is a subtle interplay between classical computation and shallow quantum computation. In fact, for the second separation, we establish that, for some problems, the ability to perform adaptive measurements in a single shallow quantum circuit, is more useful than the ability to perform polynomially many shallow quantum circuits without adaptive measurements.  
(c) There exists a 2-message proof of quantum depth protocol. Such a protocol allows a classical verifier to efficiently certify that a prover must be performing a computation of some minimum quantum depth. Our proof of quantum depth can be instantiated using the recent proof of quantumness construction by Yamakawa and Zhandry [FOCS 22].

</details>



<details>
<summary>

### Self-Testing of a Single Quantum System: Theory and Experiment
*Xiao-Min Hu, Yi Xie, Atul Singh Arora, Ming-Zhong Ai, Kishor Bharti, Jie Zhang, Wei Wu, Ping-Xing Chen, Jin-Ming Cui, Bi-Heng Liu, Yun-Feng Huang, Chuan-Feng Li, Guang-Can Guo, Jérémie Roland, Adán Cabello, Leong-Chuan Kwek*

<sub> Mar 2022 [ [arXiv](https://arxiv.org/abs/2203.09003) ] —— [preparing to submit]  </sub>  
<sub>19+6 pages, 2+1 figures</sub>
</summary>

> Self-testing allows for characterising quantum systems under minimal assumptions.
However, existing schemes rely on quantum non-locality and cannot be applied to systems that are not entangled. Here, we introduce a robust method that achieves self-testing of individual systems by taking advantage of contextuality. The scheme is based on the simplest contextuality witness for the simplest contextual quantum system---the Klyachko-Can-Binicioğlu-Shumovsky inequality for the qutrit. We establish a lower bound on the fidelity of the state and the measurements as a function of the value of the witness under a pragmatic assumption on the measurements. We apply the method in an experiment on a single trapped $^{40}{\rm Ca}^+$ and using randomly chosen measurements and perfect detection efficiency. Using the observed statistics, we obtain the first experimental demonstration of self-testing of a single quantum system with negligible deviations from the assumptions.
</details>




<details>
<summary>

### Oracle separations of hybrid quantum-classical circuits
*Atul Singh Arora, Alexandru Gheorghiu, Uttam Singh*

<sub> Jan 2022 [ [arXiv](https://arxiv.org/abs/2201.01904) | [GitHub](https://atulsingharora.github.io/HQC) ] —— [preparing to submit]  </sub>  
<sub>47 pages, 5 figures</sub>

</summary>

An important theoretical problem in the study of quantum computation, that is also practically relevant in the context of near-term quantum devices, is to understand the computational power of hybrid models, that combine polynomial-time classical computation with short-depth quantum computation. Here, we consider two such models: CQ_d which captures the scenario of a polynomial-time classical algorithm that queries a d-depth quantum computer many times; and QC_d which is more analogous to measurement-based quantum computation and captures the scenario of a d-depth quantum computer with the ability to change the sequence of gates being applied depending on measurement outcomes processed by a classical computation. Chia, Chung and Lai (STOC 2020) and Coudron and Menda (STOC 2020) showed that these models (with d=polylog(n)) are strictly weaker than BQP (the class of problems solvable by polynomial-time quantum computation), relative to an oracle, disproving a conjecture of Jozsa in the relativised world.

In this paper, we show that, despite the similarities between CQ_d and QC_d, the two models are incomparable, i.e. CQ_d ⊈ QC_d and QC_d ⊈ CQ_d relative to an oracle. In other words, we show that there exist problems that one model can solve but not the other and vice versa. We do this by considering new oracle problems that capture the distinctions between the two models and by introducing the notion of an intrinsically stochastic oracle, an oracle whose responses are inherently randomised, which is used for our second result. While we leave showing the second separation relative to a standard oracle as an open problem, we believe the notion of stochastic oracles could be of independent interest for studying complexity classes which have resisted separation in the standard oracle model. Our constructions also yield simpler oracle separations between the hybrid models and BQP, compared to earlier works.

</details>

### Analytic quantum weak coin flipping protocols with arbitrarily small bias
*Atul Singh Arora, Jérémie Roland, Chrysoula Vlachou*

<sub> 13 July 2020 [ [arXiv](https://arxiv.org/abs/1911.13283) | [GitHub](https://atulsingharora.github.io/WCF2) ] —— [ [SODA '21](), QIP '21, QCrypt '21 ] </sub>  
<sub>13+14 pages, 3 figures</sub>

### All fundamental non-contextuality inequalities are unique
*Kishor Bharti, Atul Singh Arora, Leong Chuan Kwek, Jérémie Roland*

<sub> Dec 2019 [ [arXiv](https://arxiv.org/abs/1811.05294) ] —— [ [Phys Rev Res 2020](https://doi.org/10.1103/PhysRevResearch.2.033010) ]
 </sub>  
<sub>17 pages (5 main, 12 appendix), 4 figures</sub>

### Quantum Weak Coin Flipping
*Atul Singh Arora, Jérémie Roland, Stephan Weis*

<sub> Nov 2018 [ [arXiv](https://arxiv.org/abs/1811.02984) | [GitHub](https://atulsingharora.github.io/WCF) ] —— 
[ [STOC '19](https://doi.org/10.1145/3313276.3316306), QIP '19 ]  
98 pages, split into 3 parts, 10 figures
</sub>

### Revisiting the admissibility of non-contextual hidden variable models in quantum mechanics

*Atul Singh Arora, Kishor Bharti, Arvind*

<sub> Nov 2018 [ [arXiv](https://arxiv.org/abs/1811.02984) ] —— 
[ [Phys Lett A, 2018](https://doi.org/10.1016/j.physleta.2018.11.049) ]   
4 pages, 1 figure
</sub>



### Proposal for a macroscopic test of local realism with phase-space measurements

*Atul Singh Arora, Ali Asadian*

<sub> Aug 2015 [ [arXiv](https://arxiv.org/abs/1508.04588)  ] —— 
[ [Phys Rev A, 2015](https://doi.org/10.1103/PhysRevA.92.062107) ]  
9 pages, 3 figures
</sub>


⟨ [list of publications on arXiv](https://arxiv.org/search/quant-ph?searchtype=author&query=Arora%2C+A+S) ⟩

