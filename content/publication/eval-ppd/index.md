---
title: "Understanding and mitigating difficulties in posterior predictive evaluation"
authors:
- abhinav

date: "2024-05-30T00:00:00Z" 
doi: 

# Schedule page publish date (NOT publication's date).
publishDate: "2020-10-23T00:00:00Z"

# Publication type.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: Arxiv
publication_short:  Under submission

abstract: Predictive posterior densities (PPDs) are of interest in approximate Bayesian inference. Typically, these are estimated by simple Monte Carlo (MC) averages using samples from the approximate posterior. We observe that the signal-to-noise ratio (SNR) of such estimators can be extremely low. An analysis for exact inference reveals SNR decays exponentially as there is an increase in (a) the mismatch between training and test data, (b) the dimensionality of the latent space, or (c) the size of the test data relative to the training data. Further analysis extends these results to approximate inference. To remedy the low SNR problem, we propose replacing simple MC sampling with importance sampling using a proposal distribution optimized at test time on a variational proxy for the SNR and demonstrate that this yields greatly improved estimates.
# Summary. An optional shortened abstract.
summary: 

tags:
- Posterior Predictive Evaluation
- Importance Sampling
- Approximate Inference
featured: true
links:
url_pdf: "https://arxiv.org/abs/2405.19747"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'We find that the accuracy of simple MC PPD estimator suffers when dataset mismatch, latent dimension, or test data size increases. Adaptive importance sampling can help.'
  focal_point: 
  preview_only: false

projects: 

slides: ""
---
