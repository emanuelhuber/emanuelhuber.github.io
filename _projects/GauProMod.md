---
layout: project
title: Gaussian Process Modelling
title_short: Gaussian Process Modelling
date: 2022-12-23
description: Software package for Gaussian Process (GP) modelling written in R language. The core functions are coded in C++ and based on the EIGEN library (through RcppEigen).
picture: "GauProMod_logo.png"
---


R functions for Gaussian process (GP) modelling. The core functions are coded in C++ and based on the EIGEN library (through RcppEigen)
Notes

Current features:

- Posterior Gaussian Process with Gaussian likelihood (Gaussian process conditioned to noise-free and noisy observations)
- Space-time Gaussian process
- Gaussian Process with monomial mean functions with vague Gaussian prior on the coefficient parameters
- Gaussian Process conditioned to derivative observations
- Covariance function: Matern, Gaussian, linear
- Anisotropic covariance functions (scale and rotation)
- Log marginal likelihood of the Gaussian process
- Cross-matrix distance (distance between every rows of each matrix): crossdist(x,y,M) (with M a positive semidefinite matrix for anisotropic distances)


This is an ongoing project. If you have any questions, requirements, suggestions, don’t hesitate to contact me (in english, french or german):
emanuel.huber@alumni.ethz.ch
