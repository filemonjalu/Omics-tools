# Batman NMR
Version: 1.06

![image](https://github.com/user-attachments/assets/e140f45a-e44e-4bf2-982c-f927e21b7be5)

## Website
https://batman.r-forge.r-project.org/

## Description
Batman is an R package designed to estimate metabolite concentrations from Nuclear Magnetic Resonance (NMR) spectral data through a specialized Markov Chain Monte Carlo (MCMC) algorithm. The package deconvolutes peaks from 1D NMR spectra, assigns them to specific metabolites from a predefined target list, and calculates their concentrations. Its Bayesian model integrates prior knowledge of metabolite-specific peak patterns and accommodates peak position shifts frequently observed in biological NMR samples. By employing the MCMC algorithm, BATMAN samples from the joint posterior distribution of model parameters, delivering concentration estimates with reduced error compared to conventional numerical integration methods and achieving accuracy on par with manual deconvolution by expert spectroscopists.

## Functionality
- NMR data annotation

## Instrument Data Type
- NMR

## Approaches
- Estimated compound concentration

## Software Type
R Package

## Operating System (OS)
- Unix/Linux
- Mac OS
- Windows

## Language
R, C++, MATLAB

## Dependencies
R ≥ 2.15.0,doSNOW, foreach, iterators, snow, utils, plotrix

## Input Formats - Open
ASCII, R

## Input Formats - Proprietary
Bruker

## Published
2011

## Last Updated
2016

## License
GPL-2

## Publications
- https://europepmc.org/article/med/24853927 (2014)
- https://pubs.acs.org/doi/10.1021/ac400237w (2013)
- https://europepmc.org/article/med/22635605 (2012)
- https://arxiv.org/abs/1105.2204 (2012)
