# NestedLoRA-VMC

[![NeurIPS 2026](https://img.shields.io/badge/NeurIPS-2026-blue.svg)](https://neurips.cc/)

 **Official JAX Implementation** for the paper:

> **Variational Monte Carlo for Quantum Excited States via Nested Low-Rank Approximation**\
> Minchan Jeong*, J. Jon Ryu*, Se-Young Yun, Gregory W. Wornell\
> *NeurIPS 2026*

NestedLoRA-VMC computes the lowest $K$ eigenstates of a molecule with neural-network variational Monte Carlo.
Each state has its own network, trained on a reparameterized low-rank approximation (LoRA) objective whose gradient is estimated without bias by sampling each state's Born density.
A sequential nesting scheme recovers the states in eigenvalue order without overlap penalties, at $O(K)$ Laplacians per step.
The code is built on [DeepQMC](https://github.com/deepqmc/deepqmc) v1.2.0.

**Status:** we are cleaning up the code for release, and it will be available here by the end of November 2026.

## Citation

If you find this work useful, please cite our paper:

```bibtex
@inproceedings{jeong2026nestedloravmc,
title={Variational Monte Carlo for Quantum Excited States via Nested Low-Rank Approximation},
author={Minchan Jeong and Jongha Jon Ryu and Se-Young Yun and Gregory W. Wornell},
booktitle={The Fortieth Annual Conference on Neural Information Processing Systems},
year={2026}
}
```

This work builds upon the nested low-rank approximation (NestedLoRA) framework. Please also consider citing:

```bibtex
@inproceedings{ryu2024nestedlora,
title={Operator {SVD} with Neural Networks via Nested Low-Rank Approximation},
author={Ryu, Jongha Jon and Xu, Xiangxiang and Erol, Hasan Sabri Melihcan and Bu, Yuheng and Zheng, Lizhong and Wornell, Gregory W.},
booktitle={Proceedings of the 41st International Conference on Machine Learning},
year={2024},
url={https://proceedings.mlr.press/v235/ryu24b.html},
}
```
