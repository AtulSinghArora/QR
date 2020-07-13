# Analytic quantum weak coin flipping protocols with arbitrarily small bias

### Abstract

Weak coin flipping (WCF) is a fundamental cryptographic primitive for two-party secure computation, where two distrustful parties need to remotely establish a shared random bit whilst having opposite preferred outcomes. It is the strongest known primitive with arbitrarily close to perfect security quantumly while classically, its security is completely compromised (unless one makes further assumptions, such as computational hardness).  A WCF protocol is said to have bias <img src="/WCF2/tex/7ccca27b5ccc533a2dd72dc6fa28ed84.svg?invert_in_darkmode&sanitize=true" align=middle width=6.672392099999992pt height=14.15524440000002pt/> if neither party can force their preferred outcome with probability greater than <img src="/WCF2/tex/e9633b50dd9c859072b67374544f6ce9.svg?invert_in_darkmode&sanitize=true" align=middle width=51.42121049999998pt height=24.65753399999998pt/>. Classical WCF protocols are shown to have bias <img src="/WCF2/tex/d5d5564ce0bb9999695f32da6ba7af42.svg?invert_in_darkmode&sanitize=true" align=middle width=24.657628049999992pt height=24.65753399999998pt/>, i.e., a cheating party can always force their preferred outcome. On the other hand, there exist quantum WCF protocols with arbitrarily small bias, as Mochon showed in his seminal work in 2007 [arXiv:0711.4114]. In particular, he proved the existence of a family of WCF protocols approaching bias <img src="/WCF2/tex/522c4b3472ec407a4353c9db934b0c1f.svg?invert_in_darkmode&sanitize=true" align=middle width=125.27964239999999pt height=24.65753399999998pt/> for arbitrarily large <img src="/WCF2/tex/63bb9849783d01d91403bc9a5fea12a2.svg?invert_in_darkmode&sanitize=true" align=middle width=9.075367949999992pt height=22.831056599999986pt/> and proposed a protocol with bias <img src="/WCF2/tex/1f2e78c6abdca51193a251d24229cc8d.svg?invert_in_darkmode&sanitize=true" align=middle width=24.657628049999992pt height=24.65753399999998pt/>. Last year, Arora, Roland and Weis presented a protocol with bias <img src="/WCF2/tex/bbe56a4adda015427dc0338af0ce9433.svg?invert_in_darkmode&sanitize=true" align=middle width=32.876837399999985pt height=24.65753399999998pt/> and to go below this bias, they designed an algorithm that *numerically* constructs unitary matrices corresponding to WCF protocols with arbitrarily small bias [STOC'19, p.205-216]. In this work, we present new techniques which yield a fully analytical construction of WCF protocols with bias arbitrarily close to zero, thus achieving a solution that has been missing for more than a decade. Furthermore, our new techniques lead to a simplified proof of existence of WCF protocols by circumventing the non-constructive part of Mochon's proof. As an example, we illustrate the construction of a WCF protocol with bias <img src="/WCF2/tex/0387a7dc95884370668c2f3d27011371.svg?invert_in_darkmode&sanitize=true" align=middle width=32.876837399999985pt height=24.65753399999998pt/>.



### Remark

In the previous version of this article we presented a geometric solution. The new solution is simpler and more compact. We intend to release a full version with both solutions in the coming months.



### Drafts

*Latest version*: The latest draft has been updated on the arXiv (see [arXiv:1911.13283](https://arxiv.org/abs/1911.13283)).


| Versions                     | Release Date     | Remark(s)                                                    | Hindsight                                           |
| ---------------------------- | ---------------- | ------------------------------------------------------------ | ---------------------------- |
| [WCF_Article_algebraic_SODA](./WCF_Article_algebraic_SODA) | July 13, 2020 | SODA submission (with FOCS-referee suggestions accommodated) [*] | Simplified Algebraic Solution |
| [WCF_Article_algebraic_1v3_submission.pdf](./WCF_Article_algebraic_1v3_submission.pdf) |  | FOCS 2020 submission [EDIT: rejected] | Simplified Algebraic Solution |
| [analyticCF1_1v3](./analyticCF1_1v3.pdf) | November 29, 2019 | Various minor improvements and added an argument to clarify some proofs. Uploaded to the arXiv. | Geometric Solution |
| [analyticCF1_1v0_STOC_submission](./analyticCF1_1v0_submissionSTOC.pdf)   | November 5, 2019  | STOC 2020 submission (see [known issues](#known-issues-version-Nov-5-2019)) [EDIT: rejected] | Geometric Solution |



### Known Issues (version Nov 5, 2019)

1. Page 2
	* <img src="/WCF2/tex/aeccf52d7964f8fd476fc0b6fe2658fa.svg?invert_in_darkmode&sanitize=true" align=middle width=97.66817114999999pt height=27.77565449999998pt/> as opposed to the equality.
	* The statement "while in the final frame there is only one point with coordinates <img src="/WCF2/tex/4b1bdcff2daee73a371a2b8c56c36071.svg?invert_in_darkmode&sanitize=true" align=middle width=37.18036244999999pt height=24.65753399999998pt/>" should have <img src="/WCF2/tex/c745b9b57c145ec5577b82542b2df546.svg?invert_in_darkmode&sanitize=true" align=middle width=10.57650494999999pt height=14.15524440000002pt/>  and <img src="/WCF2/tex/8217ed3c32a785f0b5aad4055f432ad8.svg?invert_in_darkmode&sanitize=true" align=middle width=10.16555099999999pt height=22.831056599999986pt/> swapped.
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