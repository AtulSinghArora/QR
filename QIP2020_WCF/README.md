# Almost perfect weak coin flipping protocols

### Poster

The current version of the [poster](QIPposter.pdf) and the article [arXiv:1911.13283](https://arxiv.org/abs/1911.13283) can be accessed through these links.

### Abstract

We investigate weak coin flipping, a fundamental cryptographic primitive where two distrustful parties need to remotely establish a shared random bit. A cheating player can try to bias the output bit towards a preferred value. A weak coin-flipping protocol has a bias *ϵ* if neither player can force the outcome towards their preferred value with probability more than 1/2+*ϵ*. While it is known that classically *ϵ*=1/2, Mochon
showed in 2007 [[arXiv:0711.4114](https://arxiv.org/abs/0711.4114)] that quantumly weak coin flipping can beachieved with arbitrarily small bias, i.e. *ϵ*(*k*)=1/(4*k*+2) for arbitrarily large *k*, and he proposed an explicit protocol approaching bias 1/6. So far, the best known explicit protocol is the one by Arora, Roland and Weis, with *ϵ*(2)=1/10 (corresponding to *k*=2) [STOC'19, p. 205-216]. In the current work, we present the construction of protocols approaching arbitrarily close to zero bias, i.e. *ϵ*(*k*) for arbitrarily large *k*. We connect the algebraic properties of Mochon's assignments—at the heart of his proof of existence—with the geometric properties of the unitaries whose
existence he proved. It is this connection that allows us to find these unitaries analytically.

### References

* For a nice overview of the coin flipping problem, Kitaev's frameworks and the fundamental result that WCF is quantumly possible:


  Carlos Mochon  
  [Quantum weak coin flipping with arbitrarily small bias](https://arxiv.org/abs/0711.4114) (2007)

* For a peer-reviewed indpendent confirmation of the aforesaid:

  Dorit Aharonov, André Chailloux, et. al.  
  [A simpler proof of existence of quantum weak coin flipping with arbitrarily small bias](https://arxiv.org/abs/1402.7166) (2016 in [SIAM J. Comput](https://doi.org/10.1137/14096387X))

* The former best explicit weak coin flipping protocol (bias 1/6) is described in its neatest form in the aforesaid. The original article by the same author on the said topic:  

  Carlos Mochon  
  [Large family of quantum weak coin-flipping protocols](https://arxiv.org/abs/quant-ph/0502068) (2005 in [Phys Rev A](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.72.022341))

* Current best known explicit weak coin flipping protocol (bias 1/10) and the Elliptic Monotone Align (EMA) algorithm which can numerically yield near zero bias protocols.  

  Arora, Roland, Weis.  
  [arXiv:1811.02984](https://arxiv.org/abs/1811.02984). [51st ACM Symposium on Theory of Computing (STOC'19), pages 205-216, 2019](http://dx.doi.org/10.1145/3313276.3316306). [ Web](https://atulsingharora.github.io/WCF).

* Kitaev's contributions:  

  Alexei Kitaev  
  Quantum coin flipping. Talk at the 6th workshop on Quantum Information Processing, 2003.

* The current best explicit strong coin flipping protocol:  


  Andris Ambainis  
  [A New Protocol and Lower Bounds for Quantum Coin Flipping](https://arxiv.org/abs/quant-ph/0204022) (2002 in [J. Comp. & Sys. Sc.](https://www.sciencedirect.com/science/article/pii/S0022000003001417))

### Contact
All of us were affiliated with the Université libre de Bruxelles (ULB) when contributions were made to the work. Our group [QuIC website](http://quic.ulb.ac.be) may be of interest. Our contact information
- [Atul Singh Arora](https://atulsingharora.github.io) 
	- aarora@ulb.ac.be, atul.singh.arora@gmail.com
- Jérémie Roland
	- jroland@ulb.ac.be
- Chrysoula Vlachou
	- chrisoula.vlachou@ulb.ac.be



Address:  
QuIC  
Ecole Polytechnique de Bruxelles  
Université Libre de Bruxelles  
50 av. F.D. Roosevelt - CP165/59  
B-1050 Bruxelles  
Belgique  