# Weak Coin Flipping

### Abstract

We investigate weak coin flipping, a fundamental cryptographic primitive where two distrustful parties need to remotely establish a shared random bit. A cheating player can try to bias the output bit towards a preferred value. For weak coin flipping the players have known opposite preferred values. A weak coin-flipping protocol has a bias ε if neither player can force the outcome towards his/her preferred value with probability more than 1/2+ε. While it is known that classically ε=1/2, Mochon showed in 2007 that quantumly weak coin flipping can be achieved with arbitrarily small bias (near perfect) but the best known explicit protocol has bias 1/6 (also due to Mochon). We propose a framework to construct new explicit protocols achieving biases beyond 1/6. In particular, we construct explicit unitaries for protocols with bias up to 1/10 (the first improvement of its kind in the last thirteen years). To go beyond, we introduce what we call the Elliptic Monotone Align (EMA) algorithm which, together with the framework, allows us to construct protocols with arbitrarily small biases. This solves the open problem of quantum weak coin flipping (in the absence of noise).

The [extended abstract](./QIP_2019_abstract_WCF_1v1.pdf) submitted to QIP is also available.



### Mathematical/Technical Draft

The current version of the [draft](./WCF_0v8c.pdf) is 0v8c which was updated on October 17, 2018.

| Versions                   | Release Date     |      |
| -------------------------- | ---------------- | ---- |
| [WCF_0v8c](./WCF_0v8c.pdf) | October 17, 2018 |      |
| [WCF_0v8a](./WCF_0v8a.pdf) | October 2, 2018  |      |



### Numerical Implementation

This section is under construction.



### Interesting References

* For a nice overview of the coin flipping problem, Kitaev's frameworks and the fundamental result that WCF is quantumly possible:


  Carlos Mochon  
  [Quantum weak coin flipping with arbitrarily small bias](https://arxiv.org/abs/0711.4114) (2007)

* For a peer-reviewed indpendent confirmation of the aforesaid:


  Dorit Aharonov, André Chailloux, et. al.  
  [A simpler proof of existence of quantum weak coin flipping with arbitrarily small bias](https://arxiv.org/abs/1402.7166) (2016 in [SIAM J. Comput](https://doi.org/10.1137/14096387X))

* The current best explicit weak coin flipping protocol is described in its neatest form in the aforesaid. The original article by the same author on the said topic:  


  Carlos Mochon  
  [Large family of quantum weak coin-flipping protocols](https://arxiv.org/abs/quant-ph/0502068) (2005 in [Phys Rev A](https://journals.aps.org/pra/abstract/10.1103/PhysRevA.72.022341))

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
- Stephan Weis
	- maths@weis-stephan.de



Address:  
QuIC  
Ecole Polytechnique de Bruxelles  
Université Libre de Bruxelles  
50 av. F.D. Roosevelt - CP165/59  
B-1050 Bruxelles  
Belgique  