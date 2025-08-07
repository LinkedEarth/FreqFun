[![DOI](https://zenodo.org/badge/246457932.svg)](https://zenodo.org/badge/latestdoi/246457932)


# Fun with analysis in the frequency domain

## Motivation

This repository contains several [Jupyter](https://jupyter.org) notebooks showcasing paleoclimate workflows making use of the frequency domain. Yes, we are talking about spectral, wavelet, and cross-wavelet analysis! 

These notebooks are using several repositories maintained by [LinkedEarth](https://linked.earth):

### Pyleoclim

[Pyleoclim](https://pyleoclim-util.readthedocs.io/en/master/) is a Python package geared towards timeseries analysis of time-uncertain data.

### PyLiPD

The [PyLiPD](https://pylipd.readthedocs.io/en/latest/) package directly works with data in the Linked Paleo Data ([LiPD](https://lipd.net)) format. The advantage of using LiPD files for paleoclimate studies is that they are standardized, supporting automation of several functionalities. 

## License

All notebooks herein are provided under an [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license.

## Citation
We needn't tell you that making research tools accessible requires time and effort. If you find any of these resources useful and use them in your own research, please do us the kindness of one or more citations. Notebooks in this collection are registered on Zenodo, and associated with a digital object identifier (DOI).  A ready-to-use citation is provided on this GitHub repository in APA and BibTex (in the "About" section on the right panel, click on "Cite this repository"). If you use any of the software, please cite them as well. It will make us (and our sponsors) very happy to hear that these investments spawned more research.

## Setting up the environment

To setup the environment, run the following commands in the terminal:

```
conda install -n base conda-libmamba-solver
conda config --set solver libmamba
conda env create -f environment.yml

conda activate freqfun
conda install ipykernel    
python -m ipykernel install --user --name=freqfun
```

This will create a conda environment named `freqfun` with all the necessary packages installed. The environment can be activated by running `conda activate freqfun`.

Note: the commands about `ipykernel` are necessary to make the environment available in Jupyter notebooks.
