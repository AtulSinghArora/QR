# Oracle separations of hybrid quantum-classical circuits

An important theoretical problem in the study of quantum computation, that is also practically relevant in the context of near-term quantum devices, is to understand the computational power of hybrid models, that combine polynomial-time classical computation with short-depth quantum computation. Here, we consider two such models: CQ_d which captures the scenario of a polynomial-time classical algorithm that queries a d-depth quantum computer many times; and QC_d which is more analogous to measurement-based quantum computation and captures the scenario of a d-depth quantum computer with the ability to change the sequence of gates being applied depending on measurement outcomes processed by a classical computation. Chia, Chung and Lai (STOC 2020) and Coudron and Menda (STOC 2020) showed that these models (with d=polylog(n)) are strictly weaker than BQP (the class of problems solvable by polynomial-time quantum computation), relative to an oracle, disproving a conjecture of Jozsa in the relativised world.

In this paper, we show that, despite the similarities between CQ_d and QC_d, the two models are incomparable, i.e. CQ_d ⊈ QC_d and QC_d ⊈ CQ_d relative to an oracle. In other words, we show that there exist problems that one model can solve but not the other and vice versa. We do this by considering new oracle problems that capture the distinctions between the two models and by introducing the notion of an intrinsically stochastic oracle, an oracle whose responses are inherently randomised, which is used for our second result. While we leave showing the second separation relative to a standard oracle as an open problem, we believe the notion of stochastic oracles could be of independent interest for studying complexity classes which have resisted separation in the standard oracle model. Our constructions also yield simpler oracle separations between the hybrid models and BQP, compared to earlier works.

### Article
* [Latest version](HQC_beta_1_6_6.pdf)
* [arXiv version](https://arxiv.org/abs/2201.01904)

### Poster
Download the poster [[pdf](HQC_poster.pdf)].

References mentioned in the poster.
* [Chia, Chung, Lai (STOC '20)](https://arxiv.org/abs/1909.10303)
* [Coudron, Menda (STOC '20)](https://arxiv.org/abs/1909.10503)

### Authors

| Author | Affiliation | email |
|-|-|-|
| Atul Singh Arora | atul.singh.arora@gmail.com, asarora@caltech.edu | IQIM, Caltech | 
|Alexandru Gheorghiu | agheorghiu@ethz.ch |Institute for Theoretical Studies, ETH Zürich |
| Uttam Singh | uttam@cft.edu.pl | Centre for Theoretical Physics, Polish Academy of Sciences |
