# Awesome Evidence Accumulation Models

This repo aimed at curating all information related to evidence accumulation models (EAMs) or seqeuntial sampling models (SSMs). Drift-diffusion models (DDMs) and linear balstic accumulator (LBA) are two prominent models in this family. 

All people in the field are welcome to contribute to this repo and make is an awesome resource for EAM/SSM. 

## What is EAM/SSM? 
Broadly speaking, EAM/SSM is a family of models, which can be used to describe the process of evidence accumulation/decay in human decision-making. In the simplest case, it can be described as a one-dimensional random walk, where the probability of going up or down is determined by a drift parameter (Ratcliff et al., 2016). This family of models are widely used in cognitive science, computational psychiatry, neuroscience, behavioral economics, etc.

## Software for EAM

### Overview
<!-- insert a table with four columns: software name, languages, key features, and url-->
There has been a lot of work in this area, and many software have been developed. Here is a list of software that are currently available. 

### EAMs in Python
| Software name | Key features | URL |
| --- | --- | --- |
| HDDM |  Hierarchical Bayesian parameter estimation of the Drift Diffusion Model | [link](https://hddm.readthedocs.io/en/latest/); [tutorial in dockerHDDM](https://doi.org/10.1177/25152459241298700)|
| HSSM | An upgraded version of HDDM, include more EAMs | [link](https://lnccbrown.github.io/HSSM/) |
| PyDDM | A simulator and modeling framework for generalized drift-diffusion models | [link](https://github.com/mwshinn/PyDDM) |
| PyBEAM | A Python package for fitting two-boundary, binary choice models to choice-RT data using Bayesian inference methods | [link](https://github.com/murrowma/pybeam); [paper](https://doi.org/10.3758/s13428-023-02162-w) |

### EAMs in R
| Software name | Key features | URL |
| --- |  --- | --- |
| EMC2 | An R package for Bayesian hierarchical cognitive modeling | [link](https://github.com/ampl-psych/EMC2); [paper](https://doi.org/10.3758/s13428-025-02869-y) |
| rdist |  A general-purpose r package for DDM and related function | [link](https://cran.r-project.org/web/packages/rdist/index.html) |
| RWiener | A R package Wiener process distribution functions | [link](https://cran.r-project.org/web/packages/RWiener/index.html) |
| flankr |An R package for Flanker task | [link](https://github.com/JimGrange/flankr); [paper](https://link.springer.com/article/10.3758/s13428-015-0615-y) |
| dynConfiR | A R package for sequential sampling models of decision confidence | [link](https://github.com/SeHellmann/dynConfiR); [paper](https://osf.io/preprints/psyarxiv/e354s_v5)|
| `wiener_full_lpdf()` | A seven parameter DDM in Stan | [link](https://osf.io/486up/files/zqm2f); [paper](https://link.springer.com/article/10.3758/s13428-023-02179-1) |

### EAMs in Julia
| Software name  | Key features | URL |
| --- | --- | --- |
| SequentialSamplingModels.jl | A unified interface for simulating and evaluating sequential sampling models | [link](https://juliapackages.com/p/sequentialsamplingmodels) |

### EAMs in Matlab

| Software name |  Key features | URL |
| --- | ---  | --- |
| DMAT | A Matlab interface for DDM | [link](https://ppw.kuleuven.be/okp/software/dmat/) |

### Standalone software for EAMs
| Software name | Languages | Key features | URL |
| --- | --- | --- | --- |
| fast-dm-30 | standalone | A fast implementation of DDM | [link](https://www.psychologie.uni-heidelberg.de/projekt/fast-dm/) |
| EZ-DDM | javascript | A simplified version of DDM | [link](https://www.ejwagenmakers.com/EZ.html); see also [EZ Bayesian hierarchical model](https://link.springer.com/article/10.3758/s13423-025-02729-y) |

## EAM in neuroscience

### Human studies using EEG

- Kelly, S. P., & O’Connell, R. G. (2013). Internal and External Influences on the Rate of Sensory Evidence Accumulation in the Human Brain. *Journal of Neuroscience*, 33(50), 19434–19441. https://doi.org/10.1523/JNEUROSCI.3355-13.2013
- O’Connell, R. G., Dockree, P. M., & Kelly, S. P. (2012). A supramodal accumulation-to-bound signal that determines perceptual decisions in humans. *Nature Neuroscience*, 15(12), 1729–1735. https://doi.org/10.1038/nn.3248
- Twomey, D. M., Murphy, P. R., Kelly, S. P., & O’Connell, R. G. (2015). The classic P300 encodes a build-to-threshold decision variable. *European Journal of Neuroscience*, 42(1), 1636–1643. https://doi.org/10.1111/ejn.12936 
- O’Connell, R. G., & Kelly, S. P. (2021). Neurophysiology of Human Perceptual Decision-Making. *Annual Review of Neuroscience*, 44, 495–516. https://doi.org/10.1146/annurev-neuro-092019-100200

### Human studies using fMRI

### Human studies using iEEG
- Pereira, M., Megevand, P., Tan, M. X., Chang, W., Wang, S., Rezai, A., … Faivre, N. (2021). Evidence accumulation relates to perceptual consciousness and monitoring. *Nature Communications*, 12(1), 3261. https://doi.org/10.1038/s41467-021-23540-y


## Important references

- Ratcliff, R., Smith, P. L., Brown, S. D., & McKoon, G. (2016). Diffusion Decision Model: Current Issues and History. *Trends in Cognitive Sciences*, 20(4), 260–281. https://doi.org/10.1016/j.tics.2016.01.007 \[Note: This paper is a good introduction to the DDM, its history and its variants. \]

- Forstmann, B. U., Ratcliff, R., & Wagenmakers, E.-J. (2016). Sequential Sampling Models in Cognitive Neuroscience: Advantages, Applications, and Extensions. Annual Review of Psychology, 67(1), 641–666. https://doi.org/10.1146/annurev-psych-122414-033645 \[Note: This paper focus more on how SSM help to connect behavioral and neural data. \]

- Ratcliff, R., & McKoon, G. (2008). The Diffusion Decision Model: Theory and Data for Two-Choice Decision Tasks. Neural Computation, 20(4), 873–922. https://doi.org/10.1162/neco.2008.12-06-420 \[Note: An in-depth introduction to DDM and its paramenters \]

- Ratcliff, R. (1978). A theory of memory retrieval. Psychological Review, 85(2), 59–108. https://doi.org/10.1037/0033-295X.85.2.59 \[Note: The first paper introducing DDM. \]

## Books and book sections
- Smith, P. L., & Ratcliff, R. (2025). Diffusion Process Models of Decision Making: Fundamental Processes (Vol. 1). Cambridge: Cambridge University Press. [URL](https://doi.org/10.1017/9781009652667)
- Smith, P. L., & Ratcliff, R. (2024). An Introduction to the Diffusion Model of Decision-Making. In B. U. Forstmann & B. M. Turner (Eds.), *An Introduction to Model-Based Cognitive Neuroscience* (pp. 67–100). Cham: Springer International Publishing. https://doi.org/10.1007/978-3-031-45271-0_4



## How to contribute

This repo is still under developing, please help us to improve it. You can fork this repo, make changes, and submit a pull request. We will review the pull request and merge it if it follows our style guide.

## Contact

If you have any question, please contact Dr. Hu Chuan-Peng at [email](hcp4715@hotmail.com).
