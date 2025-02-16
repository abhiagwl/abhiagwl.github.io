---
layout: page
title: vijax
description: A simple JAX library to easily run VI  
img: assets/img/projects/vijax_thumbnail.png
importance: 1
category: work
related_publications: false
---

[vijax][vijax] is a flexible and modular library for variational inference (VI) with the aim to make VI algorithms more accessible. It uses [JAX][jax], [numpyro][numpyro], [tensorflow-probability][tfp], and other related libraries under the hood. I build this library as part of my [AISTATS 2025 paper][paper]. Please check out the [repository][vijax] for full details. Read below for a brief overview.




[jax]: https://github.com/jax-ml/jax
[numpyro]: https://github.com/pyro-ppl/numpyro
[tfp]: https://github.com/tensorflow/probabilityc91e3483cf4f90057d02aa492d2b25b1-Paper.pdf
[gym]: https://github.com/tensorflow/probability/tree/main/spinoffs/inference_gym
[vijax]: https://github.com/abhiagwl/vijax
[paper]: https://arxiv.org/pdf/2412.08824

### Design philosophy

The library is designed to be accessible to a wide range of users and applications, enabling them to perform VI without getting tied down by specific abstractions. Three are three main components of `vijax`:

1. [`Model`](https://github.com/abhiagwl/vijax?tab=readme-ov-file#model): Represents a probability model $p(z,x)$, where $z$ are latent variables and $x$ are observed data.
2. [`VarDist`](https://github.com/abhiagwl/vijax?tab=readme-ov-file#vardist): Represents a variational distribution $q_w(z)$.
3. [`Recipe`](https://github.com/abhiagwl/vijax?tab=readme-ov-file#recipe): Provides a high-level interface for running pre-defined VI algorithms.

By adhering to these abstractions, users can easily plug in their own optimization routines, models, and variational distributions, while still benefiting from the core features and utilities provided by the `vijax` library. 

For more information, see the [repository][vijax].


### Installation

```
pip install vijax
```



## Citing
If you use [vijax][vijax], please consider citing:

```
@inproceedings{agrawal2024disentangling,
  title={Disentangling impact of capacity, objective, batchsize, estimators, and step-size on flow VI},
  author={Agrawal, Abhinav and Domke, Justin},
  booktitle={AISTATS},
  year={2025},
}
```

