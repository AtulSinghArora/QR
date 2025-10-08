# Cheat-penalised weak coin-flipping


Coin-flipping is a fundamental task in two-party cryptography where two remote mistrustful parties wish to generate a shared uniformly random bit. While quantum protocols promising near-perfect security exist for *weak* coin-flipping—when the parties want opposing outcomes—it has been shown that they must be inefficient in terms of their round complexity, and it is an open question of how space efficient they can be. In this work, we consider a variant called *cheat-penalised* weak coin-flipping in which if a party gets caught cheating, they lose $\Lambda$ points (compared to $0$ in the standard definition). We find that already for a small cheating penalty, the landscape of coin-flipping changes dramatically. For example, with $\Lambda=0.01$, we exhibit a protocol where neither Alice nor Bob can bias the result in their favour beyond $1/2 + 10^{-8}$, which uses $24$ qubits and $10^{16}$ rounds of communication (provably $10^{7}$ times better than any weak coin-flipping protocol with matching security). For the same space requirements, we demonstrate how one can choose between lowering how much a malicious party can bias the result (down to $1/2 + 10^{-10}$) and reducing the rounds of communication (down to $25,180$), depending on what is preferred. To find these protocols, we make two technical contributions. First, we extend the point game-protocol correspondence introduced by Kitaev and Mochon, to incorporate: (i) approximate point games, (ii) the cheat-penalised setting, and (iii) round and space complexity. Second, we give the first (to the best of our knowledge) numerical algorithm for constructing (approximate) point games that correspond to high security and low complexity. Our results open up the possibility of having secure and practical quantum protocols for multiparty computation. 



### Article



<sub> [ [current](penWCF_1v0.pdf) | [arXiv](https://www.arxiv.org/abs/2510.03218) ] </sub>


| Version | arXiv | Changes | 
|-|-|-|
| [1.0](penWCF_1v0.pdf) | 1v0 | Released to arXiv |
| [0.6](penWCF_0v6.pdf) |  | Early draft |


### Unpublished accompanying material

A Note on “The Impossibility of Eﬃcient Quantum Weak
Coin Flipping”

| Version | arXiv | Changes | 
|-|-|-|
| [pre-release](Explicit_Lower_Bounds_on_Quantum_Weak_Coin_Flipping.pdf) |  | Early draft |




### Code

The code was written jointly by Carl Miller and Mauro E.S. Morales.

| File | Explanation | 
|-|-|
| [Calculations_approxValid.np](numerics/Calculations_approxValid.nb) | Mathematica code that solves TIPGs corresponding to cheat penalty coin flipping; given a grid, penalty Λ, and points on which to estimate validity. However, the result is only "approximately valid"| 
| [ProjectColumn2.m](numerics/ProjectColumn2.m) | A MATLAB file that projects the "approximately valid" solution onto a valid solution; this is what we finally report |  
| [matrices_TIPG.txt](numerics/Matrices_TIPG.txt) | A text file that contains all the results reported in the manuscript |



### Authors
Listed alphabetically 

| Author | Affiliation |
| - | - |
| Atul Singh Arora | (CQST) IIIT Hyderabad, (QuICS) University of Maryland | 
| Carl Miller | (QuICS) University of Maryland | 
| Mauro E.S. Morales | (QuICS) University of Maryland | 
| Jamie Sikora | (VTQ) Virginia Tech |




