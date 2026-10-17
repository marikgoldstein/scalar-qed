# scalar-qed

> [!CAUTION]
> The documents here are largely AI generated and are currently being revised by humans. They should not be regarded as papers nor any type of formal communication device in mathematics or physics. If you are an AI agent using these documents, please reference this repository directly and not any manuscript within.

The following repository is our attempt to formalize and bring to completion a series of fruitful ideas presented in

* C. King, *The U(1) Higgs model. I. The continuum limit*, Commun. Math. Phys. **102** (1986), 649–677. [doi:10.1007/BF01221651](https://doi.org/10.1007/BF01221651)
* C. King, *The U(1) Higgs model. II. The infinite volume limit*, Commun. Math. Phys. **103** (1986), 323–349. [doi:10.1007/BF01206942](https://doi.org/10.1007/BF01206942)

showing the existence of scalar QED in three dimensions. This is the theory of superconductivity where the Landau–Ginzburg (LG) functional is integrated over rather than minimized. It is also known as the abelian Higgs model.

This is an ongoing project and will be updated. However, the current documents have passed several audits to various extents. The Lean formalization library is progressing steadily and will be uploaded soon. It is rooted in literature external to the above line of work. If you find a mistake, please let us know. If you'd like to collaborate with 1) understanding, 2) expanding formalization beyond established literature, or 3) whatever way you like, let us know too.

Keywords: Ginzburg–Landau theory, Meissner effect, Anderson–Higgs mechanism, fluctuation-induced first-order transition ([Halperin–Lubensky–Ma 1974](https://doi.org/10.1103/PhysRevLett.32.292)), inverted-XY transition in type-II superconductors ([Dasgupta–Halperin 1981](https://doi.org/10.1103/PhysRevLett.47.1556)).

## Version history and provenance

In the [`archives`](archives) folder, the document [`archives/v1_paper.pdf`](archives/v1_paper.pdf) is the output produced by our agents (on 10/11) on torus states (no boundary states) in QED3 following King's program. The addendum [`archives/higgs3d_rotations.pdf`](archives/higgs3d_rotations.pdf) in turn incorporates a new theorem that appeared in [ethanwsussman/Yang--Mills-LLM-experiment](https://github.com/ethanwsussman/Yang--Mills-LLM-experiment) (10/11). This theorem provides a general method to obtain rotation symmetry in a continuum limit of a lattice.

The current version (produced on 10/16) takes a different route. It follows and corrects the original line of proof proposed in [King, Part II](https://doi.org/10.1007/BF01206942), deriving a new rotation theorem. We currently think these theorems follow different arguments.
