---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Land cover harmonization using Latent Dirichlet Allocation
subtitle: ''
summary: ''
authors:
- Zhan Li
- Joanne C. White
- Michael A. Wulder
- Txomin Hermosilla
- Andrew M. Davidson
- Alexis J. Comber
tags:
- '"agriculture"'
- '"bayesian"'
- '"Forest"'
- '"land cover"'
- '"land use"'
- '"landsat"'
- '"LDA"'
categories: []
date: '2020-07-01'
lastmod: 2021-03-30T23:31:42+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2021-03-30T21:31:42.110788Z'
publication_types:
- '2'
abstract: 'Large-area land cover maps are produced to satisfy different information
  needs. Land cover maps having partial or complete spatial and/or temporal overlap,
  different legends, and varying accuracies for similar classes, are increasingly
  common. To address these concerns and combine two 30-m resolution land cover products,
  we implemented a harmonization procedure using a Latent Dirichlet Allocation (LDA)
  model. The LDA model used regionalized class co-occurrences from multiple maps to
  generate a harmonized class label for each pixel by statistically characterizing
  land attributes from the class co-occurrences. We evaluated multiple harmonization
  approaches: using the LDA model alone and in combination with more commonly used
  information sources for harmonization (i.e. error matrices and semantic affinity
  scores). The results were compared with the benchmark maps generated using simple
  legend crosswalks and showed that using LDA outputs with error matrices performed
  better and increased harmonized map overall accuracy by 6–19% for areas of disagreement
  between the source maps. Our results revealed the importance of error matrices to
  harmonization, since excluding error matrices reduced overall accuracy by 4–20%.
  The LDA-based harmonization approach demonstrated in this paper is quantitative,
  transparent, portable, and efficient at leveraging the strengths of multiple land
  cover maps over large areas.'
publication: '*International Journal of Geographical Information Science*'
url_pdf: https://doi.org/10.1080/13658816.2020.1796131
doi: 10.1080/13658816.2020.1796131
---
