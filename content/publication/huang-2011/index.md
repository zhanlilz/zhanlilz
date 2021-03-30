---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Automated Methods for Measuring DBH and Tree Heights with a Commercial Scanning
  Lidar
subtitle: ''
summary: ''
authors:
- Huabing Huang
- Zhan Li
- Peng Gong
- Xiao Cheng
- Nick Clinton
- Chunxiang Cao
- Wenjian Ni
- Lei Wang
tags: []
categories: []
date: '2011-03-01'
lastmod: 2021-03-30T23:31:10+02:00
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
publishDate: '2021-03-30T21:31:10.080328Z'
publication_types:
- '2'
abstract: Accurate forest structural parameters are crucial to forest inventory, and
  modeling of the carbon cycle and wildlife habitat. Lidar (Light Detection and Ranging)
  is particularly suitable to the measurement of forest structural parameters. In
  this paper, we describe a pilot study to extract forest structural parameters, such
  as tree height, diameter at breast height (DBH), and position of individual tree
  using a terrestrial lidar (LMS-Z360i; Riegel, Inc.). The lidar was operated to acquire
  both vertical and horizontal scanning in the field in order to obtain a point cloud
  of the whole scene. An Iterative Closet Point (ICP) algorithm was introduced to
  obtain the transformation matrix of each range image and to mosaic multiple range
  images together. Based on the mosaiced data set, a variable scale and threshold
  filtering method was used to separate ground from the vegetation. Meanwhile, a Digital
  Elevation Model (DEM) and a Canopy Height Model (CHM) were generated from the classified
  point cloud. A stem detection algorithm was used to extract the location of individual
  trees. A slice above 1.3 m from the ground was extracted and rasterized. A circle
  fitting algorithm combined with the Hough transform was used to retrieve the DBH
  based on the rasterized grid. Tree heights were calculated using the height difference
  between the minimum and maximum Z values within the position of each individual
  tree with a 1 m buffer. All of the 26 trees were detected correctly, tree height
  and DBH were determined with a precision of 0.76 m and 3.4 cm, respectively, comparing
  with those visually measured in the lidar data. Our methods and results confirm
  that terrestrial lidar can provide nondestructive, high-resolution, and automatic
  determination of parameters required in forest inventory.
publication: '*Photogrammetric Engineering & Remote Sensing*'
url_pdf: http://dx.doi.org/10.14358/PERS.77.3.219
doi: 10.14358/PERS.77.3.219
---
