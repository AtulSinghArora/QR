# Quantum Weak Coin Flipping

### Abstract

We investigate weak coin flipping, a fundamental cryptographic primitive where two distrustful parties need to remotely establish a shared random bit. A cheating player can try to bias the output bit towards a preferred value. For weak coin flipping the players have known opposite preferred values. A weak coin-flipping protocol has a bias ε if neither player can force the outcome towards his/her preferred value with probability more than 1/2+ε. While it is known that classically ε=1/2, Mochon showed in 2007 that quantumly weak coin flipping can be achieved with arbitrarily small bias (near perfect) but the best known explicit protocol has bias 1/6 (also due to Mochon). We propose a framework to construct new explicit protocols achieving biases beyond 1/6. In particular, we construct explicit unitaries for protocols with bias up to 1/10 (the first improvement of its kind in the last thirteen years). To go beyond, we introduce what we call the Elliptic Monotone Align (EMA) algorithm which, together with the framework, allows us to construct protocols with arbitrarily small biases. This solves the open problem of quantum weak coin flipping (in the absence of noise).

The [extended abstract](./QIP_2019_abstract_WCF_1v1.pdf) submitted to QIP is also available.



### Draft

The current version of the [draft](./WCF_0v8c.pdf) is 0v8c which was updated on October 17, 2018.

| Versions                   | Release Date                | Remark(s)                                                    |
| -------------------------- | --------------------------- | ------------------------------------------------------------ |
| TBA                        | (upcoming) November 2, 2018 | A more comprehensive introduction; font size and margins improved; various minor improvements. |
| [WCF_0v8c](./WCF_0v8c.pdf) | October 17, 2018            | Improved plots/figures; added intuition for in the discussion of the algorithm. |
| [WCF_0v8a](./WCF_0v8a.pdf) | October 2, 2018             | It exists therefore I think.                                 |



### EMA Algorithm | Numerical Implementation

A [preliminary implementation](https://mybinder.org/v2/gh/AtulSinghArora/QR/master?filepath=WCF/numerics/EMA_demo.ipynb) of the EMA algorithm, applied to a 5&rarr; 4 move taken from Mochon's bias 1/18 game is given below as an example.

```
For a 5->4 Mochon's bias 1/18 game

The Xh matrix: 
 [[( 49.8) ( 0.0) ( 0.0) ( 0.0) ( 0.0)]
 [( 0.0) ( 50.6) ( 0.0) ( 0.0) ( 0.0)]
 [( 0.0) ( 0.0) ( 51.8) ( 0.0) ( 0.0)]
 [( 0.0) ( 0.0) ( 0.0) ( 52.6) ( 0.0)]
 [( 0.0) ( 0.0) ( 0.0) ( 0.0) ( 1000000.0)]]
The Xg matrix: 
 [[( 1.0) ( 0.0) ( 0.0) ( 0.0) ( 0.0)]
 [( 0.0) ( 49.4) ( 0.0) ( 0.0) ( 0.0)]
 [( 0.0) ( 0.0) ( 50.2) ( 0.0) ( 0.0)]
 [( 0.0) ( 0.0) ( 0.0) ( 51.4) ( 0.0)]
 [( 0.0) ( 0.0) ( 0.0) ( 0.0) ( 52.2)]]
The Initial Vector, v :
 [( 0.000000003) ( 0.163958603) ( 0.622956866) ( 0.637112321) ( 0.423237770)]
The required final vector, w:
 [( 0.404720774) ( 0.627683942) ( 0.641813635) ( 0.174037992) ( 0.000000000)]


Solution

The O Matrix:
 [[( 0.0101) ( 0.8397) ( 0.5238) (-0.1310) ( 0.0572)]
 [(-0.0152) (-0.4274) ( 0.7999) ( 0.4001) (-0.1310)]
 [( 0.0148) ( 0.2136) (-0.1999) ( 0.7999) ( 0.5238)]
 [(-0.0234) (-0.2569) ( 0.2136) (-0.4274) ( 0.8397)]
 [( 0.9994) (-0.0242) ( 0.0148) (-0.0144) ( 0.0093)]]
The O Matrix (to 9 decimal places):
 [[( 0.010124460) ( 0.839702666) ( 0.523797915) (-0.131003782)  ( 0.057189871)]
 [(-0.015201757) (-0.427434145) ( 0.799887373) ( 0.400109727)  (-0.131001355)]
 [( 0.014822755) ( 0.213629625) (-0.199890114) ( 0.799892944)  ( 0.523791838)]
 [(-0.023380660) (-0.256859820) ( 0.213635598) (-0.427449055)  ( 0.839716330)]
 [( 0.999449865) (-0.024184722) ( 0.014822541) (-0.014449894)  ( 0.009303735)]]


Correctness of the solution

O acting on v (should yield w):
 [( 0.404720774) ( 0.627683942) ( 0.641813635) ( 0.174037992) (-0.000000000)]

If O is orthogonal, the following should be identity
O.T.dot(O) =
 [[( 1.0000) ( 0.0000) (-0.0000) ( 0.0000) ( 0.0000)]
 [( 0.0000) ( 1.0000) ( 0.0000) ( 0.0000) ( 0.0000)]
 [(-0.0000) ( 0.0000) ( 1.0000) (-0.0000) ( 0.0000)]
 [( 0.0000) ( 0.0000) (-0.0000) ( 1.0000) (-0.0000)]
 [( 0.0000) ( 0.0000) ( 0.0000) (-0.0000) ( 1.0000)]]
 
The certificate (valid if all non-negative)
 [(-0.000000000) ( 0.000000000) ( 0.000001583) ( 1.654069915) ( 999998.945928502)]
```

The associated raw ipython notebook is present in the [numerics folder](./numerics/).



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