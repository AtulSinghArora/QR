# Explicit quantum weak coin flipping protocols with arbitrarily small bias

### Abstract

We investigate weak coin flipping, a fundamental cryptographic primitive where two distrustful parties need to remotely establish a shared random bit. A cheating player can try to bias the output bit towards a preferred value. A weak coin-flipping protocol has a bias ε if neither player can force the outcome towards their preferred value with probability more than <img src="/WCF2_backup/tex/e9633b50dd9c859072b67374544f6ce9.svg?invert_in_darkmode&sanitize=true" align=middle width=51.42121049999998pt height=24.65753399999998pt/>. While it is known that classically <img src="/WCF2_backup/tex/6fc1585e939955d20d1a0b7b96be936e.svg?invert_in_darkmode&sanitize=true" align=middle width=53.24764994999999pt height=24.65753399999998pt/>, Mochon showed in 2007 that quantumly weak coin flipping can be achieved with arbitrarily small bias, i.e. <img src="/WCF2_backup/tex/429c0b4fdb102aae18d2eac667e018ad.svg?invert_in_darkmode&sanitize=true" align=middle width=125.27964239999999pt height=24.65753399999998pt/> for arbitrarily large k, and he proposed an explicit protocol approaching bias <img src="/WCF2_backup/tex/1f2e78c6abdca51193a251d24229cc8d.svg?invert_in_darkmode&sanitize=true" align=middle width=24.657628049999992pt height=24.65753399999998pt/> . So far, the best known explicit protocol is the one by Arora et al, with <img src="/WCF2_backup/tex/0e96e2778ee20ef844bfb1c154671d29.svg?invert_in_darkmode&sanitize=true" align=middle width=82.47150284999998pt height=24.65753399999998pt/> (corresponding to <img src="/WCF2_backup/tex/e021cb770c745ec45faa5ae82936a9b8.svg?invert_in_darkmode&sanitize=true" align=middle width=39.21220214999999pt height=22.831056599999986pt/>) . In the current work, we present the construction of protocols approaching arbitrarily close to zero bias, i.e. <img src="/WCF2_backup/tex/6bc2de780a440b6a3b65d9aae3b67a76.svg?invert_in_darkmode&sanitize=true" align=middle width=28.53318764999999pt height=24.65753399999998pt/> for arbitrarily large <img src="/WCF2_backup/tex/63bb9849783d01d91403bc9a5fea12a2.svg?invert_in_darkmode&sanitize=true" align=middle width=9.075367949999992pt height=22.831056599999986pt/>. We connect the algebraic properties of Mochon's assignments—at the heart of his proof of existence—with the geometric properties of the unitaries whose existence he proved. It is this connection that allows us to find these unitaries analytically. 





### Drafts

*Latest version*: Last draft is on the arXiv (see [arXiv:1911.13283](https://arxiv.org/abs/1911.13283)).


| Versions                     | Release Date     | Remark(s)                                                    |
| ---------------------------- | ---------------- | ------------------------------------------------------------ |
| [analyticCF1_1v3](./analyticCF1_1v3.pdf) | November 29, 2019 | Various minor improvements and added an argument to clarify some proofs. Uploaded to the arXiv. |
| [analyticCF1_1v0_STOC_submission](./analyticCF1_1v0_submissionSTOC.pdf)   | November 5, 2019  | Submitted to STOC 2020. (see [known issues](#known-issues-version-Nov-5-2019)) |



### Known Issues (version Nov 5, 2019)

1. Page 2
	* <img src="/WCF2_backup/tex/aeccf52d7964f8fd476fc0b6fe2658fa.svg?invert_in_darkmode&sanitize=true" align=middle width=97.66817114999999pt height=27.77565449999998pt/> as opposed to the equality.
	* The statement "while in the final frame there is only one point with coordinates <img src="/WCF2_backup/tex/4b1bdcff2daee73a371a2b8c56c36071.svg?invert_in_darkmode&sanitize=true" align=middle width=37.18036244999999pt height=24.65753399999998pt/>" should have <img src="/WCF2_backup/tex/c745b9b57c145ec5577b82542b2df546.svg?invert_in_darkmode&sanitize=true" align=middle width=10.57650494999999pt height=14.15524440000002pt/>  and <img src="/WCF2_backup/tex/8217ed3c32a785f0b5aad4055f432ad8.svg?invert_in_darkmode&sanitize=true" align=middle width=10.16555099999999pt height=22.831056599999986pt/> swapped.
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