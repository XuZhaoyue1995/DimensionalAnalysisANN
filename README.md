# DimensionalAnalysisANN

Code for the paper

> Zhaoyue Xu, Xinlei Zhang, Shizhao Wang, Guowei He.
> **Artificial neural network based response surface for data-driven dimensional analysis.**
> *Journal of Computational Physics* 459 (2022) 111145.
> https://doi.org/10.1016/j.jcp.2022.111145

A neural network is trained as the response surface of a physical quantity. Its
gradients are taken by finite differences, and the active subspace of those
gradients gives the dominant dimensionless numbers.

## Contents

| Folder | Case |
|---|---|
| `Pipe/` | Friction factor of rough pipe flow (Colebrook equation). `Pipe1.py`, `Pipe2.py` and `Pipe3.py` use three different parameter ranges. |
| `Flexibleload/NumericalData/` | Drag on a flexible body, synthetic data. |
| `Flexibleload/ExperimentalData/` | Drag on a flexible body, experimental data. |

Each script loads the trained network stored next to it and prints the
eigenvalues and eigenvectors of the active subspace, followed by the exponents
of the identified dimensionless numbers. Run a script from its own folder.
The scripts run with TensorFlow 2.15.

## Citation

```bibtex
@article{xu2022ann,
  title   = {Artificial neural network based response surface for data-driven dimensional analysis},
  author  = {Xu, Zhaoyue and Zhang, Xinlei and Wang, Shizhao and He, Guowei},
  journal = {Journal of Computational Physics},
  volume  = {459},
  pages   = {111145},
  year    = {2022},
  doi     = {10.1016/j.jcp.2022.111145}
}
```
