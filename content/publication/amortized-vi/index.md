---
title: "Amortized Variational Inference in Hierarhical Distributions"
authors:
- abhinav
- Justin Domke
date: "2021-09-28T00:00:00Z" 
doi: 

# Schedule page publish date (NOT publication's date).
publishDate: "2021-09-28T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In **Neural Information Processing Systems**
publication_short: In **NeurIPS** 2021

abstract: It is difficult to use subsampling with variational inference in hierarchical models since the number of local latent variables scales with the dataset. Thus, inference in hierarchical models remains a challenge at large scale. It is helpful to use a variational family with a structure matching the posterior, but optimization is still slow due to the huge number of local distributions. Instead, this paper suggests an amortized approach where shared parameters simultaneously represent all local distributions, and a "feature pooling" network is learned to represent conditionally i.i.d. observations. This approach is similarly accurate as using a given joint distribution (e.g. a full-rank Gaussian) but is feasible on datasets that are several orders of magnitude larger. It is also dramatically faster than using a structured variational distribution.


# Summary. An optional shortened abstract.
summary: 

tags:
- BBVI
- Amortized Variational Inference
- Hierarchical Models
- Scalable Inference
featured: true
links:
url_pdf: "https://proceedings.neurips.cc/paper_files/paper/2021/file/b28d7c6b6aec04f5525b453411ff4336-Paper.pdf"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Complementary CDF plots of improvement'
  focal_point: "smart"
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

