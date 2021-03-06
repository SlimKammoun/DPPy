[![Documentation Status](https://readthedocs.org/projects/dppy/badge/?version=latest)](https://dppy.readthedocs.io/en/latest/?badge=latest)
[![Build Status](https://travis-ci.com/guilgautier/DPPy.svg?branch=master)](https://travis-ci.com/guilgautier/DPPy)

# DPPy: Sampling Determinantal Point Processes with Python

> Anything that can go wrong, will go wrong. − [Murphy's Law](http://phdcomics.com/comics/archive.php?comicid=1867)

## Introduction

Determinantal point processes (DPPs) are specific probability distributions over clouds of points that have been popular as models or computational tools across physics, probability, statistics, and more recently of booming interest in machine learning.
Sampling from DPPs is a nontrivial matter, and many approaches have been proposed. 
DPPy is a Python library that puts together all exact and approximate sampling algorithms for DPPs.

## Requirements

DPPy works with [Python 3.4+](http://docs.python.org/3/)

### Dependencies
- [NumPy](http://www.numpy.org)
- [SciPy](http://www.scipy.org/)
- [Matplotlib](http://matplotlib.org/)
- [Networkx](http://networkx.github.io/) to play with [uniform spanning trees](https://dppy.readthedocs.io/en/latest/exotic_dpps/index.html#uniform-spanning-trees)
- [CVXOPT](http://cvxopt.org) to use the `zono_sampling` MCMC sampler for finite DPPs. **CVXOPT itself requires [GCC](http://gcc.gnu.org)**,
    + On MAC it comes with [Xcode](https://developer.apple.com/xcode/)
    + On UNIX, use your package manager (`apt`, `yum` etc)
        ```bash
        sudo apt install -qq gcc g++
        ```

## Installation
1. If you have a GitHub account
    - Please consider forking DPPy
    - Use git to clone your copy of the repo
        ```bash
        cd <directory_of_your_choice>
        git clone https://github.com/<username>/DPPy.git
        ```
2. If you only use git, clone this repository
    ```bash
    cd <directory_of_your_choice>
    git clone https://github.com/guilgautier/DPPy.git
    ```
3. Otherwise simply dowload the project

Finally, in any case, install the project
```bash
cd DPPy
pip install .
```

### Contribute to the documentation

The [documentation](https://readthedocs.org/projects/dppy/badge/?version=latest) is generated locally with [Sphinx](http://www.sphinx-doc.org/en/master/) and then built online by [ReadTheDocs](https://readthedocs.org/projects/dppy/).

If you wish to contribute to the documentation or just play with it locally, you can:

- Install Sphinx 
```bash
pip install -U sphinx
```
- Generate the docs locally
```bash
cd DPPy/docs
make html
```
- Open the local HTML version of the documentation located at `DPPy/docs/_build/html/index.html`
```bash
open _build/html/index.html
```

If you wish pull request your contribution, please use the `docs` branch.

### How to cite this work?

We wrote a companion paper to [DPPy](https://github.com/guilgautier/DPPy) for latter submission to the [MLOSS](http://www.jmlr.org/mloss/) track of JMLR.

The companion paper is available on

- [arXiv](http://arxiv.org/abs/1809.07258)
- [GitHub](https://github.com/guilgautier/DPPy_paper), see the [`arxiv`](https://github.com/guilgautier/DPPy_paper/tree/arxiv) branch

If you use this package, please consider citing it with this piece of BibTeX:
```bibtex
@article{GaBaVa18,,
    archivePrefix = {arXiv},
    arxivId = {1809.07258},
    author = {Gautier, Guillaume and Bardenet, R{\'{e}}mi and Valko, Michal},
    eprint = {1809.07258},
    journal = {ArXiv e-prints},
    title = {{DPPy: Sampling Determinantal Point Processes with Python}},
    keywords = {Computer Science - Machine Learning, Computer Science - Mathematical Software, Statistics - Machine Learning},
    url = {http://arxiv.org/abs/1809.07258},
    year = {2018},
    note = {Code at http://github.com/guilgautier/DPPy/ Documentation at http://dppy.readthedocs.io/}
}
```

## Reproducibility

We would like to thank [Guillermo Polito](https://guillep.github.io/) for leading our reproducible research [workgroup](https://github.com/CRIStAL-PADR/reproducible-research-SE-notes), this project owes him a lot.

Take a look at the corresponding [booklet](https://github.com/CRIStAL-PADR/reproducible-research-SE-notes) to learn more on how to make your research reproducible!