# Computational Work Extraction: The Complexity of Catalysts

Thermodynamics has been repeatedly reshaped by improving how one models the capabilities of agents that extract work. 
For an isolated quantum system, the maximal extractable work, the *ergotropy*, assumes that the agent can apply any unitary. However, achieving it can be computationally intractable. In this work we introduce and study *computational ergotropy*, restricting extraction to *polynomially-sized* uniform unitary circuits acting on the system alone. 

We prove *maximal separations*: $n$-qubit systems can have $\Theta(n)$ ergotropy, while every efficient process extracts negligible work, even for Hamiltonians consisting of single-qubit terms. We establish an *unconditional* existential separation and give an explicit construction in the *random oracle model*. Assuming the existence of quantum-secure pseudorandom functions, this separation extends to the *plain model*.


This work uncovers an important connection between ergotropy and the *complexity of catalytic computation*—computation where auxiliary qubits must be finally restored to their initial state. 
Relative to a random oracle, we establish relational and decision problems that:
(i) can be solved efficiently with $\lambda$ catalysts; but
(ii) cannot be solved by any algorithm with $c\lambda$ catalysts, for any $c<1$.
We show this by proving query lower bounds for *quantum-space bounded* algorithms. 
    
As a consequence, for computational ergotropy, catalysts prove to be surprisingly powerful—there is a family of Hamiltonians and states for which catalysts enable efficient extraction of the full $\Theta(n)$ ergotropy, while every efficient non-catalytic process extracts negligible work. Furthermore, catalysts also allow us to introduce and instantiate the notion of *pseudoergotropy*—analogous to pseudorandomness. On the other hand, we show catalysts do not change (information-theoretic) ergotropy. 

Finally, our work also sheds light on the classical aspect of the problem. First, most of our constructions rely on classical states and Hamiltonians and therefore imply analogous results for *classical ergotropy*. Second, we show that certain *proof of quantumness* protocols can be used to generically  *separate classical and quantum* catalytic ergotropy.

Overall, these results point towards a theory of thermodynamics where computational complexity plays a fundamental role. 


### Article

<sub> [ [current](BoundedThermo_1v0.pdf) | [arXiv](http://arxiv.org/abs/2609.40323) ] </sub>


| Version | arXiv | Changes | 
| -- | -- | -- |
| [1.0](BoundedThermo_1v0.pdf) | v1 | arXiv version |


### Authors


| Name | Affiliation | Email | 
| -- | -- | -- | 
| Atul Singh *Arora* | CQST, IIIT Hyderabad | atul.singh.arora@gmail.com |
| Shantanav *Chakraborty* | CQST and CSTAR, IIIT Hyderabad | shchakra@iiit.ac.in |
| Alexandru *Cojocaru* | University of Edinburgh | cojocaru.alex.3010@gmail.com |
| Sreyas *Saminathan* | CQST, IIIT Hyderabad | futuresreyas@gmail.com |
| Uttam *Singh* | CQST, IIIT Hyderabad |  uttam@iiit.ac.in |


For various insightful discussions and comments, we are grateful to Andrea Coladangelo (in particular, for the "last query" approach) and Venkata Koppula (in particular, during our misguided forays into database arguments).

(Listed alphabetically)

(AI was only used for looking up and debugging LaTeX commands)