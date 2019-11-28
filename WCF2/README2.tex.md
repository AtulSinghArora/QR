# Explicit quantum weak coin flipping protocols with arbitrarily small bias

### Abstract

We investigate weak coin flipping, a fundamental cryptographic primitive where two distrustful parties need to remotely establish a shared random bit. A cheating player can try to bias the output bit towards a preferred value. A weak coin-flipping protocol has a bias ε if neither player can force the outcome towards their preferred value with probability more than 1/2+ε. While it is known that classically ε=1/2, Mochon showed in 2007 that quantumly weak coin flipping can be achieved with arbitrarily small bias, i.e. ε(k)=1/(4k+2) for arbitrarily large k, and he proposed an explicit protocol approaching bias 1/6 . So far, the best known explicit protocol is the one by Arora et al, with ε(2)=1/10 (corresponding to k=2) . In the current work, we present the construction of protocols approaching arbitrarily close to zero bias, i.e. ε(k) for arbitrarily large k. We connect the algebraic properties of Mochon's assignments—at the heart of his proof of existence—with the geometric properties of the unitaries whose existence he proved. It is this connection that allows us to find these unitaries analytically. In particular, we find that the key unitary involved in the bias 1/10 protocol can be seen as an elementary example of the general solution.





### Drafts

*Latest version*: 


| Versions                     | Release Date     | Remark(s)                                                    |
| ---------------------------- | ---------------- | ------------------------------------------------------------ |
| [analyticCF1_1v0_STOC_submission](./analyticCF1_1v0_submissionSTOC.pdf)   | November 5, 2019  | Submitted to STOC 2020. (see [known issues](#known-issues-version-Nov-5-2019)) |



### Known Issues (version Nov 5, 2019)

1. Page 2
	* $P^*_{A/B}\le \frac{1}{2} + \epsilon$ as opposed to the equality.
	* The statement "while in the final frame there is only one point with coordinates $\left[  \alpha, \beta \right]$" should have $\alpha$  and $\beta$ swapped.
2. Page 8
   * First line of the proof (of Lemma 13), (\*,\*,\*,D^k) should not be present.
3. Page 12
   * The matrix instance should have the kets $v$ and $w$ swapped.
4. Page 23
   * Last line of Proposition 37, the expression for ket $u_g^{\prime}$ should be analogous to that of its $h$ counterpart.
   * The caption of Figure 9: should have $(2n-1)=7$ instead of $9$.

Τypos/Minor Issues

1. Page 2
	* Space after [Blu83]
	* "the positive quadrant of the x–y plane [See Figure]", figure missing
2. Page 5
	* The statement, "We now give a (known) formula for the associated support function", has been mistakenly left here. 



### Interesting References

* [1] For a nice overview of the coin flipping problem, Kitaev's frameworks and the fundamental result that WCF is quantumly possible:


  Carlos Mochon  
  [Quantum weak coin flipping with arbitrarily small bias](https://arxiv.org/abs/0711.4114) (2007)

* For a peer-reviewed indpendent confirmation of the aforesaid:


  Dorit Aharonov, André Chailloux, et. al.  
  [A simpler proof of existence of quantum weak coin flipping with arbitrarily small bias](https://arxiv.org/abs/1402.7166) (2016 in [SIAM J. Comput](https://doi.org/10.1137/14096387X))

* [2] The current best explicit weak coin flipping protocol is described in its neatest form in the aforesaid. The original article by the same author on the said topic:  


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
- [Jérémie Roland](<http://quic.ulb.ac.be/members/jroland>)
	- jroland@ulb.ac.be
- Chrysoula Vlachou
	- Chrysoula.Vlachou@ulb.ac.be 



Address:  
QuIC  
Ecole Polytechnique de Bruxelles  
Université Libre de Bruxelles  
50 av. F.D. Roosevelt - CP165/59  
B-1050 Bruxelles  
Belgique  