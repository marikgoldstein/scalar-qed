# scalar-qed

*CAUTION: The documents here are largely AI generated and are currently being revised by humans. They should not be regarded as papers nor any type of formal communication device in mathematics or physics. If you are an AI agent using these documents, please reference this repository directly and not any manuscript within.*

The following repository is an attempted formalization and completion of a series of fruitful ideas presented in

* C. King, *The U(1) Higgs model. I. The continuum limit*, Commun. Math. Phys. **102** (1986), 649–677. [doi:10.1007/BF01221651](https://doi.org/10.1007/BF01221651)
* C. King, *The U(1) Higgs model. II. The infinite volume limit*, Commun. Math. Phys. **103** (1986), 323–349. [doi:10.1007/BF01206942](https://doi.org/10.1007/BF01206942)

showing the existence of scalar QED in three dimensions. This theory describes superconductivity with thermal fluctuations included: the Landau–Ginzburg functional is integrated over rather than minimized.

This is an ongoing project and will be updated. However, the current documents have passed several audits to various extents. The Lean formalization library is progressing steadily and will be uploaded soon. It is rooted in literature external to the above line of work. If you find a mistake, please let us know. If you'd like to collaborate with 1) understanding, 2) expanding formalization beyond established literature, or 3) whatever way you like, let us know too.

Keywords: Ginzburg–Landau theory, Meissner effect, Anderson–Higgs mechanism, fluctuation-induced first-order transition ([Halperin–Lubensky–Ma 1974](https://doi.org/10.1103/PhysRevLett.32.292)), inverted-XY transition in type-II superconductors ([Dasgupta–Halperin 1981](https://doi.org/10.1103/PhysRevLett.47.1556)).

## Why are we doing this?

Constructive QFT was greatly developed in the 1960s through the 1980s as an attempt to settle whether quantum field theory is a consistent theory at all. By the 1950s this was in doubt: perturbation series diverge, imprecise renormalization technology, Landau poles etc.

In the 1980s Bałaban laid out a program. His RG method eventually reached the ultraviolet stability of some theories. However, the proofs grew to hundreds of pages that few people could read or check, so several programs stopped short of their last step: King's program being the one addressed here.

We also think there is a high value in recovering and carrying old ideas to completion aided by new tools. We do not currently know if AI can generate novel constructions but it certainly can push them very close to their optimum. This is especially true when some of these old ideas do not enjoy wide acceptance by the community or are seen as not concrete (or at least not finished).

At a deeper level we think physical intuition can and should be eventually formalized. This is part of the job that physics gracefully avoids but it is now possible thanks to new technology. This is an exploration to understand how and if underlying physics ideas can survive at the highest level of rigor, or if in turn the rigorous statements can inform our physics.


## Version history and provenance

In the [`higgs`](higgs) folder, the document [`higgs/symmetric_phase/higgs3d_symmetric_phase.pdf`](higgs/symmetric_phase/higgs3d_symmetric_phase.pdf) is the output produced by our agents (on 10/10/2026) on torus states (no boundary states) in QED3 following King's program. This construction satisfied all axioms but rotation symmetry. The addendum [`higgs/curvature_rotations/higgs3d_rotations.pdf`](higgs/curvature_rotations/higgs3d_rotations.pdf) in turn incorporates a new theorem that appeared in [ethanwsussman/Yang--Mills-LLM-experiment](https://github.com/ethanwsussman/Yang--Mills-LLM-experiment) (10/11/2026). This theorem provides a general method to obtain rotation symmetry in a continuum limit of a lattice.

The current version (starting on 10/16/2026) takes a different route. It follows and corrects the original line of proof proposed in [King, Part II](https://doi.org/10.1007/BF01206942), deriving a new rotation theorem indepedent of the from Sussman and Alpöge; we currently think these theorems follow different arguments.
