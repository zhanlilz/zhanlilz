---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Towards analysis ready data of optical CubeSat images: Demonstrating a hierarchical
  normalization framework at a wetland site'
subtitle: ''
summary: ''
authors:
- Zhan Li
- Daniel Scheffler
- Nicholas C. Coops
- Nicholas Leach
- Torsten Sachs
tags:
- '"Landsat"'
- '"Time series analysis"'
- '"MODIS"'
- '"PlanetScope"'
- '"Sentinel-2"'
- '"RapidEye"'
- '"Radiometric normalization"'
- '"Co-registration"'
categories: []
date: '2021-12-01'
lastmod: 2021-10-18T23:47:41+02:00
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
publishDate: '2021-10-18T21:47:39.441839Z'
publication_types:
- '2'
abstract: Optical images of the Earth at very high spatial resolutions (VHR, typically textless 5 m)
  are seeing rapid growth in volumes over the past 5 years, due in part to the fast-expanding
  constellations of CubeSats. Special preprocessing of these VHR images is required
  to ensure their geometric and radiometric consistency for quantitative analyses
  for a wide range of Earth and environmental sciences and applications. Here we describe
  a hierarchical normalization framework (HiNF) to achieve and evaluate geometric
  and radiometric normalization of these VHR images towards producing analysis ready
  data (ARD) of optical CubeSat images. We demonstrated HiNF at a spatially heterogeneous
  and temporally dynamic wetland site in northeastern Germany by generating a stack
  of temporally consistent ~ biweekly 5-m images over 8 years (2013–2020) at visible
  and near infrared bands (VNIR). The HiNF combined images from rigorously calibrated
  multispectral sensors onboard large satellites (Landsat-7/8 and Sentinel-2) and
  less well calibrated sensors onboard RapidEye (SmallSats) and PlanetScope (CubeSats).
  A two-stage radiometric normalization procedure produced two levels of image normalization
  and resulted in more normalized images that passed the quality control in time series
  compared to common one-stage procedures. The outcome of this novel procedure allows
  for downstream applications to balance between the quality and the quantity of available
  normalized CubeSat images in a time series. The HiNF provides a new approach to
  quantitative evaluations of radiometric normalizations using daily MODIS imagery
  as bridging benchmark data. The quantitative evaluations showed the HiNF resulted
  in greater normalization efficacy in the visible bands than in the NIR over the
  predominantly wetland area. The two normalization levels yielded statistically similar
  efficacy for the NIR band and the widely-used normalized difference vegetation index
  according to the Chow test (at significance level of 0.05) but less so for the visible
  bands. The HiNF facilitates generating ARD of optical CubeSat images and assuring
  their qualities through its demonstrated efficacy and its quantitative evaluation
  approach. Such ARD-quality time series of VHR images from CubeSats allow for improved
  analyses and quantitative applications of this new stream of multispectral images
  at spatial scales that are better related to ground measurements and environmental
  management in terrestrial ecosystems.
publication: '*International Journal of Applied Earth Observation and Geoinformation*'
url_pdf: https://www.sciencedirect.com/science/article/pii/S0303243421002099
doi: 10.1016/j.jag.2021.102502
---
