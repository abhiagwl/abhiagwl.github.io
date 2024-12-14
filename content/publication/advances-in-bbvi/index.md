---
title: "Advances in black-box VI: Normalizing flows, importance weighting, and optimization"
authors:
- abhinav

date: "2020-10-23T00:00:00Z" 
doi: 

# Schedule page publish date (NOT publication's date).
publishDate: "2020-10-23T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["paper-conference"]

# Publication name and optional abbreviated publication name.
publication: In **Neural Information Processing Systems** 2020.
publication_short: In **NeurIPS** 2020

abstract: Recent research has seen several advances relevant to black-box variational inference (VI), but the current state of automatic posterior inference is unclear. One such advance is the use of normalizing flows to define flexible posterior densities for deep latent variable models. Another direction is the integration of Monte-Carlo methods to serve two purposes; first, to obtain tighter variational objectives for optimization, and second, to define enriched variational families through sampling. However, both flows and variational Monte-Carlo methods remain relatively unexplored for black-box VI. Moreover, on a pragmatic front, there are several optimization considerations like step-size scheme, parameter initialization, and choice of gradient estimators, for which there is no clear guidance in the literature. In this paper, we postulate that black-box VI is best addressed through a careful combination of numerous algorithmic components. We evaluate components relating to optimization, flows, and Monte-Carlo methods on a benchmark of 30 models from the Stan model library. The combination of these algorithmic components significantly advances the state-of-the-art "out of the box" variational inference.

# Summary. An optional shortened abstract.
summary: 

tags:
- BBVI
- Normalizing Flows
- Stan Models
featured: true


url_pdf: "https://arxiv.org/pdf/2006.10343.pdf"
url_code: 'https://github.com/abhiagwl/Advances_in_BBVI'
url_poster: 'https://drive.google.com/file/d/1JsnZnOaybdIUotf4pK7PeZN6CSZOetoX/view?usp=sharing'
url_slides: 'https://drive.google.com/file/d/14vbCVxBFRX4zLG5WD83CDI_On1hNZKgF/view?usp=sharing'

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
projects: 

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

