---
layout: page
title: vistan
description: A simple Python library to run VI on Stan models
img: assets/img/projects/vistan_thumbnail.png
importance: 1
category: work
related_publications: false
---


[vistan][4] uses [autograd][1] and [PyStan][2] under the hood. The aim is to provide a "petting zoo" to make it easy to play around with the different variational methods discussed in the NeurIPS 2020 paper [Advances in BBVI][3]. Please check out the [repository][4] for full details. Read more below for a brief overview. 


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="https://raw.githubusercontent.com/abhiagwl/vistan/master/vistan-example.png" title="A beta-bernoulli example with vistan" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    A simple beta-bernoulli example with <a href="https://github.com/abhiagwl/vistan">vistan</a>. The posterior predicted by the flows is more similar to the true posterior than meanfield. See <a href="https://proceedings.neurips.cc/paper/2020/file/c91e3483cf4f90057d02aa492d2b25b1-Paper.pdf">paper</a> for more details about the algorithms used.
</div>


[1]: https://github.com/HIPS/autograd
[2]: https://github.com/stan-dev/pystan
[3]: https://proceedings.neurips.cc/paper/2020/file/c91e3483cf4f90057d02aa492d2b25b1-Paper.pdf
[4]: https://github.com/abhiagwl/vistan

## Features

- **Initialization:** Laplace's method to initialize full-rank Gaussian
- **Gradient Estimators:** Total-gradient, STL, DReG, closed-form entropy   
- **Variational Families:** Full-rank Gaussian, Diagonal Gaussian, RealNVP
- **Objectives:** ELBO, IW-ELBO
- **IW-sampling:** Posterior samples using importance weighting

## Installation

```
pip install vistan
```

## Usage
The typical usage of the package would have the following steps:
1. Create an algorithm. This can be done in two wasy:
 - The easiest is to use a pre-baked recipe as `algo=vistan.recipe('meanfield')`. There are various options: 
    + `'advi'`: Run our implementation of ADVI's PyStan.
    + `'meanfield'`: Full-factorized Gaussia a.k.a meanfield VI
    + `'fullrank'`: Use a full-rank Gaussian for better dependence between latent variables 
    + `'flows'`: Use a RealNVP flow-based VI
    + `'method x'`: Use methods from the paper [Advances in BBVI][3] where x is one of `[0, 1, 2, 3a, 3b, 4a, 4b, 4c, 4d]`
- Alternatively, you can create a custom algorithm as `algo=vistan.algorithm()`. Some most frequent arguments:
    + `vi_family`: This can be one of `['gaussian', 'diagonal', 'rnvp']` (Default: `gaussian`)
    + `max_iter`: The maximum number of optimization iterations. (Default: 100)
    + `optimizer`: This can be `'adam'` or `'advi'`. (Default: `'adam'`)
    + `grad_estimator`: What gradient estimator to use. Can be `'Total-gradient'`, `'STL'`, `'DReG'`, or `'closed-form-entropy'`. (Default: `'DReG'`)
    + `M_iw_train`: The number of importance samples. Use `1` for standard variational inference or more for importance-weighted variational inference. (Default: 1)
    + `per_iter_sample_budget`: The total number of evaluations to use in each iteration. (Default: 100)
2. Get an approximate posterior as `posterior=algo(code, data)`. This runs the algorithm on Stan model given by the string `code` with observations given by the `data`.
3. Draw samples from the approximate posterior as `samples=posterior.sample(100)`. You can also draw samples using importance weighting as `posterior.sample(100, M_iw_sample=10)`. Further, you can evaluate the log-probability of the posterior as `posterior.log_prob(latents)`. 

## Citing vistan
If you use vistan, please, consider citing:

```
@inproceedings{aagrawal2020,
  author    = {Abhinav Agrawal and
               Daniel R. Sheldon and
               Justin Domke},
  title     = {Advances in Black-Box {VI:} Normalizing Flows, Importance Weighting,
               and Optimization},
  booktitle = {Advances in Neural Information Processing Systems 33: Annual Conference
               on Neural Information Processing Systems 2020, NeurIPS 2020, December
               6-12, 2020, virtual},
  year      = {2020},
}
```

