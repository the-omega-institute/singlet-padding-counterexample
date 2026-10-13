# Singlet padding and the universal precession GME threshold

**Haobo Ma and Wenlin Zhang**

This note gives a singlet-padding counterexample to the composition-independent implication in Conjecture 3 of [arXiv:2311.00806v2](https://arxiv.org/abs/2311.00806v2), *Certification of genuine multipartite entanglement in spin ensembles with measurements of total angular momentum*. For $K=3$, take constituent spins $(1/2,1/2,3/2)$ in the state $\psi=s\otimes g$, where $s$ is the normalized two-spin singlet and $g=(|3/2,3/2\rangle-|3/2,-3/2\rangle)/\sqrt{2}$. This state is separable across the singlet-pair/rest bipartition, yet its precession score is $P_3=3/4=24/32>23/32$, exceeding the proposed threshold by exactly $1/32$. Singlet padding preserves the score of any remaining finite spin ensemble; the note also proves a counterexample family for every odd $K\geq3$ and equality of the attainable biseparable and unrestricted quantum score sets when the ensemble may vary. The counterexample uses an effective spin-zero sector. As clarified by the authors for their erratum, their results hold under the assumption that **no 0-sector appears in any bipartition in decomposition (14)-(15)**. The counterexample falls outside that restriction and outside Result 1's hypothesis $\sum_n j_n=K/2$.

Read the [mathematical note (PDF)](note/note.pdf), dated 9 October 2026.

## Lean verification

The [Lean source at the pinned revision](https://github.com/the-omega-institute/trureturing/blob/3155010510edfab84323e848b07abac257ed5ed5/D5/S3/Quantum/Entanglement/PrecessionUniversalThresholdRefutation.lean) contains the theorem `result : ¬ claim` for the three-particle $K=3$ counterexample and the helper `singlet_padding_ensemble_score` for the general padding identity. The all-odd family and the score-set consequence are proved in the note; they are not separate Lean theorems in this module. This package links to the recorded source revision and does not report a new Lean build.

## How to cite

```bibtex
@misc{MaZhang2026singlet,
  author = {Haobo Ma and Wenlin Zhang},
  title = {Singlet padding and the universal precession {GME} threshold},
  year = {2026},
  howpublished = {\url{https://github.com/the-omega-institute/singlet-padding-counterexample}}
}
```

## License

Copyright 2026 Haobo Ma and Wenlin Zhang. The note and accompanying documentation in this repository are licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). See [LICENSE](LICENSE) for the full terms.
