# A computational test of quantum contextuality, and even simpler proofs of quantumness

Bell non-locality is a fundamental feature of quantum mechanics whereby
measurements performed on "spatially separated" quantum systems can exhibit
correlations that cannot be understood as revealing predetermined values. This
is a special case of the more general phenomenon of "quantum contextuality",
which says that such correlations can occur even when the measurements are not
necessarily on separate quantum systems, but are merely "compatible" (i.e.
commuting). Crucially, while any non-local game yields an experiment that
demonstrates quantum advantage by leveraging the "spatial separation" of two or
more devices (and in fact several such demonstrations have been conducted
successfully in recent years), the same is not true for quantum contextuality:
finding the contextuality analogue of such an experiment is arguably one of the
central open questions in the foundations of quantum mechanics.

  In this work, we show that an arbitrary contextuality game can be compiled
into an operational "test of contextuality" involving a single quantum device,
by only making the assumption that the device is computationally bounded. Our
work is inspired by the recent work of Kalai et al. (STOC '23) that converts
any non-local game into a classical test of quantum advantage with a single
device. The central idea in their work is to use cryptography to enforce
spatial separation within subsystems of a single quantum device. Our work can
be seen as using cryptography to enforce "temporal separation", i.e. to
restrict communication between sequential measurements.

  Beyond contextuality, we employ our ideas to design a "proof of quantumness"
that, to the best of our knowledge, is arguably even simpler than the ones
proposed in the literature so far.


### Article
* [Latest version](PoC.pdf)
<!-- * [arXiv version](https://arxiv.org/) -->


### Authors

Atul Singh Arora, Kishor Bharti, Alexandru Cojocaru, Andrea Coladangelo