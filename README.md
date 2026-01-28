# Awesome Evidence Accumulation Models

This repo aimed at curating all information related to evidence accumulation models (EAMs) or seqeuntial sampling models (SSMs). Drift-diffusion models (DDMs) and linear balstic accumulator (LBA) are two prominent models in this family. 

All people in the field are welcome to contribute to this repo and make is an awesome resource for EAM/SSM. 

## What is EAM/SSM? 
Broadly speaking, EAM/SSM is a family of models, which can be used to describe the process of evidence accumulation/decay in human decision-making. In the simplest case, it can be described as a one-dimensional random walk, where the probability of going up or down is determined by a drift parameter (Ratcliff et al., 2016). This family of models are widely used in cognitive science, computational psychiatry, neuroscience, behavioral economics, etc.

## Software for EAM

### Overview
<!-- insert a table with four columns: software name, languages, key features, and url-->
| Software name | Languages | Key features | URL |
| --- | --- | --- | --- |
| HDDM | Python | Hierarchical Bayesian parameter estimation of the Drift Diffusion Model | https://hddm.readthedocs.io/en/latest/ |
| PyDDM | Python | A simulator and modeling framework for generalized drift-diffusion models | https://github.com/mwshinn/PyDDM |
| PyBEAM | Python | A Python package for fitting two-boundary, binary choice models to choice-RT data using Bayesian inference methods | https://github.com/murrowma/pybeam |
| fast-dm-30 | standalone | A fast implementation of DDM | https://www.psychologie.uni-heidelberg.de/projekt/fast-dm/ |
| EZ-DDM | javascript | A simplified version of DDM | https://www.ejwagenmakers.com/EZ.html; see also [EZ Bayesian hierarchical model](https://link.springer.com/article/10.3758/s13423-025-02729-y)|

### EAMs in Python

### EAMs in R

### EAMs in Julia

### EAMs in Matlab

### Standalone software for EAMs


## Important references

- Ratcliff, R., Smith, P. L., Brown, S. D., & McKoon, G. (2016). Diffusion Decision Model: Current Issues and History. Trends in Cognitive Sciences, 20(4), 260–281. https://doi.org/10.1016/j.tics.2016.01.007 \[Note: This paper is a good introduction to the DDM, its history and its variants. \]

- Forstmann, B. U., Ratcliff, R., & Wagenmakers, E.-J. (2016). Sequential Sampling Models in Cognitive Neuroscience: Advantages, Applications, and Extensions. Annual Review of Psychology, 67(1), 641–666. https://doi.org/10.1146/annurev-psych-122414-033645 \[Note: This paper focus more on how SSM help to connect behavioral and neural data. \]

- Ratcliff, R., & McKoon, G. (2008). The Diffusion Decision Model: Theory and Data for Two-Choice Decision Tasks. Neural Computation, 20(4), 873–922. https://doi.org/10.1162/neco.2008.12-06-420 \[Note: An in-depth introduction to DDM and its paramenters \]

- Ratcliff, R. (1978). A theory of memory retrieval. Psychological Review, 85(2), 59–108. https://doi.org/10.1037/0033-295X.85.2.59 \[Note: The first paper introducing DDM. \]

## Books and book sections
- Smith, P. L., & Ratcliff, R. (2025). Diffusion Process Models of Decision Making: Fundamental Processes (Vol. 1). Cambridge: Cambridge University Press. [URL](https://doi.org/10.1017/9781009652667)
- Smith, P. L., & Ratcliff, R. (2024). An Introduction to the Diffusion Model of Decision-Making. In B. U. Forstmann & B. M. Turner (Eds.), *An Introduction to Model-Based Cognitive Neuroscience* (pp. 67–100). Cham: Springer International Publishing. https://doi.org/10.1007/978-3-031-45271-0_4



## How to contribute

 Fork this repo, make changes, and submit a pull request. We will review the pull request and merge it if it follows our style guide.
