---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Waveform lidar over vegetation: An evaluation of inversion methods for estimating
  return energy'
subtitle: ''
summary: ''
authors:
- Steven Hancock
- John D. Armston
- Zhan Li
- Rachel Gaulton
- Philip E. Lewis
- Mathias I. Disney
- F. Mark Danson
- Alan H. Strahler
- Crystal Schaaf
- Karen Anderson
- Kevin J Gaston
tags:
- '"Forests"'
- '"Full waveform"'
- '"Lidar"'
- '"Reflectance"'
- '"Signal processing"'
categories: []
date: '2015-07-01'
lastmod: 2021-03-30T23:31:14+02:00
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
publishDate: '2021-03-30T21:31:11.581111Z'
publication_types:
- '2'
abstract: Full waveform lidar has a unique capability to characterise vegetation in
  more detail than any other practical method. The reflectance, calculated from the
  energy of lidar returns, is a key parameter for a wide range of applications and
  so it is vital to extract it accurately. Fifteen separate methods have been proposed
  to extract return energy (the amount of light backscattered from a target), ranging
  from simple to mathematically complex, but the relative accuracies have not yet
  been assessed. This paper uses a simulator to compare all methods over a wide range
  of targets and lidar system parameters. For hard targets the simplest methods (windowed
  sum, peak and quadratic) gave the most consistent estimates. They did not have high
  accuracies, but low standard deviations show that they could be calibrated to give
  accurate energy. This may be why some commercial lidar developers use them, where
  the primary interest is in surveying solid objects. However, simulations showed
  that these methods are not appropriate over vegetation. The widely used Gaussian
  fitting performed well over hard targets (0.24% root mean square error, RMSE), as
  did the sum and spline methods (0.30% RMSE). Over vegetation, for large footprint
  (15 m) systems, Gaussian fitting performed the best (12.2% RMSE) followed closely
  by the sum and spline (both 12.7% RMSE). For smaller footprints (33 cm and 1 cm)
  over vegetation, the relative accuracies were reversed (0.56% RMSE for the sum and
  spline and 1.37% for Gaussian fitting). Gaussian fitting required heavy smoothing
  (convolution with an 8 m Gaussian) whereas none was needed for the sum and spline.
  These simpler methods were also more robust to noise and far less computationally
  expensive than Gaussian fitting. Therefore it was concluded that the sum and spline
  were the most accurate for extracting return energy from waveform lidar over vegetation,
  except for large footprint (15 m), where Gaussian fitting was slightly more accurate.
  These results suggest that small footprint (≪ 15 m) lidar systems that use Gaussian
  fitting or proprietary algorithms may report inaccurate energies, and thus reflectances,
  over vegetation. In addition the effect of system pulse length, sampling interval
  and noise on accuracy for different targets was assessed, which has implications
  for sensor design.
publication: '*Remote Sensing of Environment*'
url_pdf: http://www.sciencedirect.com/science/article/pii/S003442571500142X
doi: 10.1016/j.rse.2015.04.013
---
