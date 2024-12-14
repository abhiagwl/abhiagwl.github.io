---
title: "Disentangling impact of capacity, objective, batchsize, estimators, and step-size on flow VI"
authors:
- abhinav
- Justin Domke

date: "2024-05-30T00:00:00Z" 
doi: 

# Schedule page publish date (NOT publication's date).
publishDate: "2020-10-23T00:00:00Z"

# Publication type.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: Arxiv
publication_short:  Under submission

abstract: "Normalizing flow-based variational inference (flow VI) is a promising approximate inference approach, but its performance remains inconsistent across studies. Numerous algorithmic choices influence flow VI's performance. We conduct a step-by-step analysis to disentangle the impact of some of the key factors: capacity, objectives, gradient estimators, number of gradient estimates (batchsize), and step-sizes. Each step examines one factor while neutralizing others using insights from the previous steps and/or using extensive parallel computation. To facilitate high-fidelity evaluation, we curate a benchmark of synthetic targets that represent common posterior pathologies and allow for exact sampling. We provide specific recommendations for different factors and propose a flow VI recipe that matches or surpasses leading turnkey Hamiltonian Monte Carlo (HMC) methods."
# Summary. An optional shortened abstract.
summary: 

tags:
- Normalizing Flows
- Variational Inference
- Hamiltonian Monte Carlo

featured: true
links:
url_pdf: "https://arxiv.org/abs/2412.08824"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Flow-based VI can be better than HMC'
  focal_point: "smart"
  preview_only: false

projects: 

slides: ""
---
