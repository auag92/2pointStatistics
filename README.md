## Table of contents
* [General info](#general-info)
* [Dependencies](#dependencies)
* [Setup](#setup)
* [Usage](#usage)
* [Status](#status)
* [References](#references)
* [Issues](#issues)


## General info
This package provides tools for computing spatial statistics for both atomistic and
continuum materials datasets.

## Dependencies
Project is created with:
* scipy version: 1.1.0
* numpy version: 1.16.0
* numba version: 0.39.0
* pytorch version: 0.4.1
* pytoolz version: 0.9.0


## Setup
To run this code, copy correlations.py to working directory:

## Usage

    import correlations
    # for periodic cross autocorrelations for X1
    gg = compute_statistics(boundary="periodic", corrtype="auto", cutoff=None, device=torch.device("cpu"), args0=X1)

    # for periodic cross crosscorrelation between X1 and X2
    gg = compute_statistics(boundary="periodic", corrtype="cross", cutoff=None, device=torch.device("cpu"), args0=X1, args1=X2)

    # for non-periodic cross crosscorrelations between X1 and X2
    gg = compute_statistics(boundary="nonperiodic", corrtype="cross", cutoff=None, device=torch.device("cpu"), args0=X1, args1=X2)

## Status
project is currently under active development.


## References
[Ahmet Cecen's Matlab code](https://github.com/ahmetcecen/MATLAB-Spatial-Correlation-Toolbox)



## Issues

Please send questions and issues about installation and usage of this code to [apaar92@gmail.com](mailto:apaar92@gmail.com)
