# Awesome Evidence Accumulation Models

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A curated collection of resources for evidence accumulation models (EAMs) and sequential sampling models (SSMs) in computational psychology, neuroscience, and decision-making research.

This repository aims to curate comprehensive information related to evidence accumulation models (EAMs) or sequential sampling models (SSMs). Drift-diffusion models (DDMs) and linear ballistic accumulator (LBA) are two prominent models in this family, which have become fundamental tools for understanding decision-making processes across various disciplines.

**🤝 All researchers and practitioners in the field are welcome to contribute to this repository and help make it an awesome resource for the EAM/SSM community!** 

## What is EAM/SSM?

Broadly speaking, EAM/SSM is a family of computational models that describe the process of evidence accumulation/decay in human decision-making. In the simplest case, it can be described as a one-dimensional random walk, where the probability of moving up or down is determined by a drift parameter (Ratcliff et al., 2016).

### Key Concepts

- **Evidence Accumulation**: Models describe how information is gathered over time until a decision threshold is reached
- **Stochastic Process**: Decision-making is modeled as a probabilistic process with inherent noise
- **Response Time Distribution**: These models naturally account for both choice accuracy and response time distributions
- **Parameter Interpretation**: Model parameters map onto cognitive processes (e.g., drift rate → evidence quality, boundary separation → response caution)

### Applications

This family of models is widely used in:
- **Cognitive Science**: Understanding attention, memory, and perception
- **Computational Psychiatry**: Characterizing cognitive deficits in mental disorders
- **Neuroscience**: Linking behavioral data to neural mechanisms
- **Behavioral Economics**: Modeling choice under uncertainty
- **Artificial Intelligence**: Human-inspired decision-making systems
- **Educational Psychology**: Understanding learning and skill acquisition

## Software for EAM

### Quick Start Guide

| Use Case | Recommended Software | Language | Difficulty |
|---|---|---|---|
| **Beginners** | EZ-DDM, HDDM | Python/R | ⭐ |
| **Bayesian Analysis** | HDDM, HSSM, Stan | Python/R/Stan | ⭐⭐⭐ |
| **Custom Models** | PyDDM, SequentialSamplingModels.jl | Python/Julia | ⭐⭐⭐⭐ |
| **Large Datasets** | fast-dm-30, PyDDM | C++/Python | ⭐⭐ |
| **Neural Integration** | VAM, HSSM (EEG) | Python | ⭐⭐⭐⭐ |

### Overview

The ecosystem for evidence accumulation modeling has grown significantly, with mature software packages available across multiple programming languages. Below is a comprehensive list of currently available tools, organized by language and platform. 

### EAMs in Python

| Software | Key Features | Status | URL |
|---|---|---|---|
| **HDDM** | Hierarchical Bayesian parameter estimation of DDM, MCMC sampling | 🔧 Active | [docs](https://hddm.readthedocs.io/en/latest/) • [paper](https://www.frontiersin.org/articles/10.3389/fninf.2013.00014/full) |
| **dockerHDDM** | Dockerized HDDM environment for reproducible research | 🔧 Active | [Docker Hub](https://hub.docker.com/r/hcp4715/hddm) • [tutorial](https://doi.org/10.1177/25152459241298700) |
| **HSSM** | Enhanced HDDM with more EAMs, GPU support, modern backend | 🔧 Active | [docs](https://lnccbrown.github.io/HSSM/) • [GitHub](https://github.com/lnccbrown/HSSM) • [paper](https://www.biorxiv.org/content/10.64898/2026.06.05.730398v1)|
| **PyDDM** | Generalized DDM simulator, custom models, parallel computing | 🔧 Active | [docs](https://pyddm.readthedocs.io/) • [paper](https://doi.org/10.7554/eLife.56938) |
| **PyDDMBayes** | Bayesian version of PyDDM | 🆕 New | to-be-open? • [paper](https://openreview.net/pdf?id=M7nQBB1sxG) |
| **PyBEAM** | Bayesian evidence accumulation modeling for binary choices (supports multiple accumulator models including LBA) | 🔧 Active | [GitHub](https://github.com/murrowma/pybeam) • [paper](https://doi.org/10.3758/s13428-023-02162-w) |
| **psireact** | Hierarchical Bayesian modeling of response time data, multiple accumulator models including LBA | 🔧 Development | [GitHub](https://github.com/mortonne/psireact) |
| **VAM** | Visual accumulator model with CNN integration for image-based decisions | 🔧 Active | [paper](https://doi.org/10.7554/eLife.98351) • [GitHub](https://github.com/pauljaffe/vam) |
| **RegDDM** | Bayesian regression analysis integrating DDM parameters with covariates | 🆕 New | [paper](https://arxiv.org/abs/2507.01177) |
| **EZ-CDM** | Circular diffusion model for angular decision-making | 🆕 New | [paper](https://link.springer.com/article/10.3758/s13423-024-02483-7) |
| **FlexDDM** | Flexible decision-diffusion modeling framework | 🆕 New | [paper](https://escholarship.org/uc/item/4q57r2x0) ; [code](https://github.com/joyfan00/FlexDDM)|

#### Key Python Packages
- **NumPy/SciPy**: Core numerical computing
- **PyMC/PyMC3**: Probabilistic programming (used by HDDM)
- **JAX**: GPU acceleration (used by HSSM)
- **PyTorch/TensorFlow**: Deep learning integration (VAM)

### EAMs in R

| Software | Key Features | Status | URL |
|---|---|---|---|
| **EMC2** | Bayesian hierarchical cognitive modeling, multiple SSMs (includes LBA, RDM, DDM) | 🔧  Active | [GitHub](https://github.com/awellis/EMC2) • [paper](https://doi.org/10.3758/s13428-025-02869-y) |
| **eam** | simulation-based evidence accumulation models (DDM, LCA, LBA, RDM, LFM) | 🔧  Active | [GitHub](https://github.com/y-guang/eam) • [paper](https://osf.io/preprints/psyarxiv/dg7c2_v1) |
| **ggdmc** | an R package for Bayesian inference on cognitive choice response time models | 🔧  Active  | [website](https://github.com/yxlin/ggdmc) • [paper1](doi.org/10.3758/s13428-018-1067-y) • [paper2](doi.org/10.20982/tqmp.16.2.p133) |
| **dRiftDM** | fitting time-dependent parameters of DDM (DDM, DMC, SSP)| 🔧  Active  | [website](https://bucky2177.github.io/dRiftDM/) • [paper](https://osf.io/preprints/osf/3t2vf_v1) |  
| **DMCfun** | Diffusion Model of Conflict for conflict tasks | 🔧 Active | [OSF](https://osf.io/8hkrj/) • [paper](https://doi.org/10.1016/j.cognition.2021.104607) |
| **rdist** | General-purpose R package for DDM and related functions | 📦 CRAN | `install.packages("rdist")` |
| **RWiener** | Wiener process distribution functions | 📦 CRAN | `install.packages("RWiener")` |
| **lbaModel** | Density, distribution and random generation functions for LBA model | 📦 CRAN | `install.packages("lbaModel")` |
| **glba** | General Linear Ballistic Accumulator models with covariates | 📦 CRAN | `install.packages("glba")` |
| **hBayesDM** | Hierarchical Bayesian modeling with DDM, LBA and other accumulator models, Stan backend | 🔧 Active | [docs](https://ccs-lab.github.io/hBayesDM/reference/choiceRT_lba.html) |
| **flankr** | Flanker task analysis with SSP/DSTP models | 🔧 Active | [GitHub](https://github.com/JimGrange/flankr) • [paper](https://link.springer.com/article/10.3758/s13428-015-0615-y) |
| **dynConfiR** | Sequential sampling models of decision confidence | 🔧 Active | [GitHub](https://github.com/SeHellmann/dynConfiR) • [paper](https://doi.org/10.1038/s13428-022-02385-0) |
| **brms + wiener** | Stan-based Bayesian modeling with Wiener diffusion | 🔧 Active | [brms docs](https://paul-buerkner.github.io/brms/) • [paper](https://doi.org/10.3758/s13428-023-02179-1) |

#### Key R Packages
- **brms**: Bayesian regression models via Stan
- **rstan**: R interface to Stan
- **tidyverse**: Data manipulation and visualization
- **bayesplot**: Bayesian visualization tools

### EAMs in Julia

| Software | Key Features | Status | URL |
|---|---|---|---|
| **SequentialSamplingModels.jl** | Unified interface for SSM (includes LBA, DDM, race models), simulation, plotting, Bayesian inference | 🔧 Active | [GitHub](https://github.com/itsdfish/SequentialSamplingModels.jl) • [paper](https://arxiv.org/abs/2411.06631) • [docs](https://itsdfish.github.io/SequentialSamplingModels.jl/dev/) |

#### Why Julia for SSM?
- **Performance**: Native compilation speed
- **Multiple Dispatch**: Elegant modeling syntax
- **Integration**: Seamless Python/R interoperability
- **Scientific Computing**: Built-in support for differential equations

### EAMs in Matlab

| Software | Key Features | Status | URL |
|---|---|---|---|
| **DMAT** | Matlab interface for DDM, diffusion model analysis toolbox | 📦 Stable | [website](https://ppw.kuleuven.be/okp/software/dmat/) |

### EAMs in Stan/Probabilistic Programming

| Software | Key Features | Language | URL |
|---|---|---|---|
| **Stan-DDM** | Seven-parameter DDM implementation | Stan | [paper](https://doi.org/10.3758/s13428-023-02179-1) • [code (OSF)](https://osf.io/486up/files/zqm2f) |
| **Turing.jl** | Probabilistic programming in Julia | Julia | [docs](https://turing.ml/) |
| **PyMC** | Python probabilistic programming | Python | [docs](https://www.pymc.io/) |

### Standalone Software & Web Tools

| Software | Language | Key Features | Status | URL |
|---|---|---|---|---|
| **fast-dm-30** | Standalone | Fast maximum likelihood estimation | 📦 Stable | [website](https://www.psychologie.uni-heidelberg.de/projekt/fast-dm/) • [tutorial](https://doi.org/10.3389/fpsyg.2015.00336) |
| **EZ-DDM** | JavaScript | Simplified DDM parameter estimation | 📦 Stable | [web app](https://www.ejwagenmakers.com/EZ.html) • [paper](https://doi.org/10.3758/PBR.15.6.1229) |
| **EZ-Bayesian** | Multiple | Bayesian hierarchical EZ-DDM | 🆕 New | [Python](https://github.com/joachimvandekerckhove/ezbhddm) • [R](https://github.com/Adrifelcha/EZ-project) • [paper](https://doi.org/10.3758/s13423-025-02729-y) |
| **DDM Explorer** | Web | Interactive DDM parameter visualization | 🌐 Online | [demo](https://shiny.edition.openhumans.org/ddm_explorer/) |


### 🔗 Link Status Notice

**Some links in this repository may experience intermittent access issues due to:**
- **Certificate verification errors** on academic websites
- **GitHub connection issues** affecting some repositories  
- **Institutional website maintenance** at universities

**Alternatives when links fail:**
- Search for package names on GitHub or CRAN
- Use the package installation commands above
- Check OSF (Open Science Framework) for alternative links
- Contact maintainers directly for access issues

### Choosing the Right Software

1. **For Beginners**: Start with EZ-DDM, fast-dm-30, or HDDM with default settings
2. **For Research Papers**: Use HSSM (Python) or EMC2 (R) for comprehensive modeling
3. **For Custom Models**: Use PyDDM, HSSM, or SequentialSamplingModels.jl
4. **For Large Datasets**: Consider fast-dm-30 or PyDDM with parallel computing
5. **For Neural Integration**: Use VAM or HDDM/HSSM for behavior-EEG/MEG joint modeling


## Tutorials & Learning Resources

### 🚀 Getting Started Tutorials

#### **For Complete Beginners**
- **[Wilson & Collins (2019)](https://doi.org/10.7554/eLife.49547)**: Ten simple rules for computational modeling of behavioral data
- **[Bodner et al. (2021)](https://doi.org/10.1371/journal.pcbi.1008539)**: Graduate student guide to mathematical modeling
- **[Myers et al. (2022)](https://doi.org/10.3389/fpsyg.2022.1039172)**: Practical introduction to DDM in psychology and neuroscience

#### **Hands-On Software Tutorials**
- **[Pan et al. (2025)](https://doi.org/10.1177/25152459241298700)**: dockerHDDM tutorial with reproducible environment
- **[Voss et al. (2015)](https://doi.org/10.3389/fpsyg.2015.00336)**: fast-dm-30 tutorial for diffusion model analysis
- **[Fengler et al. (2022)](https://doi.org/10.1162/jocn_a_01902)**: Advanced HDDM tutorial for decision and reinforcement learning


### 📚 Advanced Topics & Specialized Applications

#### **Experimental Design & Model Selection**
- **[Boag et al. (2025)](https://doi.org/10.1177/25152459251336127)**: Expert guide to planning experiments for evidence-accumulation modeling
- **[Kvam (2024)](https://doi.org/10.3758/s13423-024-02587-0)**: Discriminating between diffusion decision and accumulator models

#### **Neuroscience & Neuroimaging**
- **[Nunez et al. (2024)](https://doi.org/10.3758/s13428-023-02331-x)**: Joint M/EEG and behavior modeling tutorial
- **[Forstmann et al. (2016)](https://doi.org/10.1146/annurev-psych-122414-033645)**: Sequential sampling models in cognitive neuroscience

#### **Bayesian Methods**
- **[RegDDM Tutorial (2025)](https://arxiv.org/abs/2507.01177)**: Bayesian regression analysis with drift-diffusion models
- **[Vloeberghs et al. (2025)](https://doi.org/10.1371/journal.pcbi.1013291)**: Bayesian hierarchical models of decision criterion fluctuations

### 🎥 Video Resources & Online Courses

#### **Online Tutorials**
- **PyDDM Cookbook**: [Interactive examples and recipes](https://pyddm.readthedocs.io/en/latest/cookbook/)
- **HDDM Documentation**: [Step-by-step tutorials](https://hddm.readthedocs.io/en/latest/tutorial.html)
- **SequentialSamplingModels.jl**: [Julia tutorials and examples](https://itsdfish.github.io/SequentialSamplingModels.jl/dev/)

#### **Conference Workshops**
- **CMU Summer School**: Computational modeling tutorials (videos available online)
- **Cognitive Science Society**: Annual workshops on computational modeling

### 📖 Books & Comprehensive Guides

#### **Textbooks**
- **[Smith & Ratcliff (2025)](https://doi.org/10.1017/9781009652667)**: Diffusion Process Models of Decision Making (2-volume set)
- **[Heathcote et al. (2019)](https://doi.org/10.3758/s13428-018-1067-y)**: Dynamic Models of Choice (DMC software)

#### **Handbook Chapters**
- **[Smith & Ratcliff (2024)](https://doi.org/10.1007/978-3-031-45271-0_4)**: Introduction to diffusion modeling in model-based cognitive neuroscience
- **[Heathcote & Hayes (2012)](https://doi.org/10.1017/CBO9780511996236)**: Diffusion modeling in *The Oxford Handbook of Computational Cognitive Science*
- **[Busemeyer & Diederich (2010)](https://doi.org/10.1093/acprof:oso/9780199732989.001.0001)**: *Cognitive Modeling* - Chapter on sequential sampling models


## Best Practices & Guidelines

<!--### 📊 Data Requirements

#### **Minimum Sample Sizes**
- **Individual fitting**: ≥ 100 trials per condition (citation needed)
- **Hierarchical fitting**: ≥ 20-30 participants, each with ≥ 50-100 trials (citation needed)
- **Complex models**: Increase trials proportionally to parameters (citation needed)

#### **Data Quality Checks**
- Remove outliers (> 3 SD from mean RT, excluding < 200ms responses)
- Check for response times < non-decision time estimates
- Ensure sufficient accuracy variability (avoid ceiling/floor effects)

### 🔧 Model Selection & Validation

#### **When to Use Different Models**
| Scenario | Recommended Model | Rationale |
|---|---|---|
| **Simple 2AFC** | Standard DDM | Well-established, interpretable parameters |
| **Multi-choice** | LBA or Race Models | Natural extension to >2 alternatives |
| **Confidence Ratings** | DDM with confidence or 2D DDM | Captures meta-cognitive processes |
| **Neural Correlates** | DDM + Neural Data | Links behavior to brain activity |
| **Time-varying Evidence** | Time-varying DDM or Ornstein-Uhlenbeck | Accounts for changing evidence quality |

#### **Model Comparison**
- **Information Criteria**: Use WAIC, LOO-CV for Bayesian models
- **Cross-validation**: K-fold validation for predictive accuracy
- **Posterior Predictive Checks**: Essential for model validation
- **Parameter Recovery**: Test with simulated data before real analysis -->

### ⚠️ Common Pitfalls & Solutions

#### **Parameter Identifiability**
- **Problem**: Drift rate and boundary separation trade-offs
- **Solution**: Fix non-decision time, use informative priors, collect sufficient data

#### **Speed-Accuracy Trade-offs**
- **Problem**: Confounding experimental manipulation with response strategies
- **Solution**: Manipulate both speed and accuracy conditions, model strategic changes

#### **Hierarchical vs. Individual Fitting**
- **Problem**: Overfitting with individual parameter estimates
- **Solution**: Use hierarchical partial pooling for group-level inference

## EAM in Neuroscience

### 🧠 Human Electrophysiology (EEG/MEG)

#### **Key Findings**
- **[O'Connell et al. (2012)](https://doi.org/10.1038/nn.3248)**: Supramodal accumulation-to-bound signals
- **[Kelly & O'Connell (2013)](https://doi.org/10.1523/JNEUROSCI.3355-13.2013)**: Neural correlates of evidence accumulation rate
- **[Twomey et al. (2015)](https://doi.org/10.1111/ejn.12936)**: P300 as decision variable signal
- **[O'Connell & Kelly (2021)](https://doi.org/10.1146/annurev-neuro-092019-100200)**: Comprehensive review of decision neurophysiology

#### **Neural Markers**
- **Centro-parietal positivity (CPP)**: Accumulation-to-bound signal
- **Beta-band activity**: Evidence accumulation dynamics
- **Pre-stimulus oscillations**: Decision threshold modulation

### 🧠 Functional MRI Studies

#### **Recent Advances (2024-2025)**
- **[Brošová et al. (2025)](https://doi.org/10.3389/fnins.2025.1513083)**: Cross-modal congruency effects on evidence accumulation
- **[Franzen et al. (2025)](https://doi.org/10.1101/2025.07.03.662942)**: Prior information effects in psychosis
- **[Cochrane et al. (2023)](https://doi.org/10.1038/s41539-023-00168-9)**: Multiple timescales of learning in evidence accumulation

### 🧠 Intracranial Recordings (iEEG)

- **[Pereira et al. (2021)](https://doi.org/10.1038/s41467-021-23540-y)**: Evidence accumulation and perceptual consciousness
- **[Human Single-Unit Studies]**: Neural implementations of drift-diffusion processes


## 📚 Important References

### Foundational Papers

| Year | Citation | Key Contribution |
|---|---|---|
| **1978** | [Ratcliff (1978)](https://doi.org/10.1037/0033-295X.85.2.59) | Original DDM paper |
| **2008** | [Ratcliff & McKoon (2008)](https://doi.org/10.1162/neco.2008.12-06-420) | Comprehensive DDM theory and parameters |
| **2008** | [Brown & Heathcote (2008)](https://doi.org/10.3758/BRM.41.4.1095) | Original LBA paper - simplest ballistic accumulator |
| **2016** | [Ratcliff et al. (2016)](https://doi.org/10.1016/j.tics.2016.01.007) | Current issues and historical overview |
| **2016** | [Forstmann et al. (2016)](https://doi.org/10.1146/annurev-psych-122414-033645) | SSM in cognitive neuroscience |



<!--- ### Recent Advances (2024-2025)

**[Khoudary et al. (2025)](https://doi.org/10.1111/ejn.70098)**: Philosophical foundations of computational modeling
- **[Nunez et al. (2025)](https://doi.org/10.1016/j.jmp.2025.102720)**: Cognitive models with identifiable parameters
- **[Fernandez et al. (2024)](https://arxiv.org/abs/2411.06631)**: Julia ecosystem for sequential sampling models

### Methodological Innovations

- **[Vloeberghs et al. (2025)](https://doi.org/10.1371/journal.pcbi.1013291)**: Trial-to-trial fluctuations modeling
- **[Jin et al. (2025)](https://arxiv.org/abs/2507.01177)**: Unified Bayesian regression with DDM
- **[Kvam (2024)](https://doi.org/10.3758/s13423-024-02587-0)**: Model discrimination techniques -->


## 🤝 Contributing

### How to Contribute

We welcome contributions from all researchers and practitioners! Here's how you can help:

#### **Adding New Resources**
1. **Software packages**: Include version, language, key features, and status
2. **Papers**: Add to appropriate sections with DOI links
3. **Tutorials**: Categorize by difficulty and target audience
4. **Bug reports**: Open issues for outdated links or information

#### **Submission Guidelines**
- Follow the existing format and style
- Include DOI links where available
- Add brief descriptions (1-2 sentences) for each entry
- Test all links before submission (many academic sites have certificate issues)
- Note when links are unstable or have access problems
- Check for duplicates before submitting

#### **Pull Request Process**
1. Fork this repository
2. Create a feature branch (`git checkout -b feature/amazing-addition`)
3. Commit your changes (`git commit -m 'Add [resource name]'`)
4. Push to the branch (`git push origin feature/amazing-addition`)
5. Open a Pull Request

### 📋 Maintenance

This repository is actively maintained. Current maintainers:
- **Dr. Hu Chuan-Peng** ([hcp4715@hotmail.com](mailto:hcp4715@hotmail.com))

#### **Review Process**
- All submissions are reviewed within 1-2 weeks
- We prioritize accuracy and relevance
- Outdated or broken resources are periodically reviewed and updated

## 🌟 Community

### 📬 Contact & Support

- **General Inquiries**: Dr. Hu Chuan-Peng ([hcp4715@hotmail.com](mailto:hcp4715@hotmail.com))
- **Bug Reports**: [GitHub Issues](https://github.com/hcp4715/awesomeDDM/issues)
- **Feature Requests**: [GitHub Discussions](https://github.com/hcp4715/awesomeDDM/discussions)

### 🏆 Recognition

Contributors are acknowledged in the repository. Special thanks to:
- All researchers who have shared their software and tutorials
- The cognitive modeling community for continuous innovation
- Open source maintainers who make these tools possible

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

> **Note**: This repository is continuously evolving. Check back regularly for new resources and updates!