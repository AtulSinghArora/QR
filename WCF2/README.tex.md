# Analytic quantum weak coin flipping protocols with arbitrarily small bias

### Abstract

Weak coin flipping (WCF) is a fundamental cryptographic primitive for two-party secure computation, where two distrustful parties need to remotely establish a shared random bit whilst having opposite preferred outcomes. It is the strongest known primitive with arbitrarily close to perfect security quantumly while classically, its security is completely compromised (unless one makes further assumptions, such as computational hardness).  A WCF protocol is said to have bias $\epsilon$ if neither party can force their preferred outcome with probability greater than $1/2+\epsilon$. Classical WCF protocols are shown to have bias $1/2$, i.e., a cheating party can always force their preferred outcome. On the other hand, there exist quantum WCF protocols with arbitrarily small bias, as Mochon showed in his seminal work in 2007 [arXiv:0711.4114]. In particular, he proved the existence of a family of WCF protocols approaching bias $\epsilon (k)=1/(4k+2)$ for arbitrarily large $k$ and proposed a protocol with bias $1/6$. Last year, Arora, Roland and Weis presented a protocol with bias $1/10$ and to go below this bias, they designed an algorithm that *numerically* constructs unitary matrices corresponding to WCF protocols with arbitrarily small bias [STOC'19, p.205-216]. In this work, we present new techniques which yield a fully analytical construction of WCF protocols with bias arbitrarily close to zero, thus achieving a solution that has been missing for more than a decade. Furthermore, our new techniques lead to a simplified proof of existence of WCF protocols by circumventing the non-constructive part of Mochon's proof. As an example, we illustrate the construction of a WCF protocol with bias $1/14$.



### Remark

In the previous version of this article we presented a geometric solution. The new solution is simpler and more compact. We intend to release a full version with both solutions in the coming months.



### Drafts

*Latest version*: The latest draft has been updated on the arXiv (see [arXiv:1911.13283](https://arxiv.org/abs/1911.13283)).


| Versions                     | Release Date     | Remark(s)                                                    | Hindsight                                           |
| ---------------------------- | ---------------- | ------------------------------------------------------------ | ---------------------------- |
| [WCF_Article_algebraic_SODA](./WCF_Article_algebraic_SODA.pdf) | July 13, 2020 | SODA submission [*] <br />(with FOCS-referee suggestions accommodated) | Simplified Algebraic Solution |
| [WCF_Article_algebraic_1v3_submission](./WCF_Article_algebraic_1v3_submission.pdf) |  | FOCS 2020 submission <br />(addressed the main criticism from the STOC reviews) <br />[EDIT: rejected] | Simplified Algebraic Solution |
| [analyticCF1_1v3](./analyticCF1_1v3.pdf) | November 29, 2019 | Various minor improvements and added an argument to clarify some proofs. Uploaded to the arXiv. | Geometric Solution |
| [analyticCF1_1v0_STOC_submission](./analyticCF1_1v0_submissionSTOC.pdf)   | November 5, 2019  | STOC 2020 submission (see [known issues](#known-issues-version-Nov-5-2019)) <br />[EDIT: rejected] | Geometric Solution |



### Known Issues (version Nov 5, 2019)

1. Page 2
	* $P^*_{A/B}\le \frac{1}{2} + \epsilon$ as opposed to the equality.
	* The statement "while in the final frame there is only one point with coordinates $\left[  \alpha, \beta \right]$" should have $\alpha$  and $\beta$ swapped.
2. Page 8
   * First line of the proof (of Lemma 13), the term with $D$ should not be present.
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