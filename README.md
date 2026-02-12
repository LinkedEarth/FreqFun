![LinkedEarthlogo](https://github.com/LinkedEarth/Logos/blob/master/LinkedEarth/LinkedEarth_small.png?raw=true)

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4556213.svg)](https://doi.org/10.5281/zenodo.4556213)
[![NSF-1541029](https://img.shields.io/badge/NSF-2126510-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=2126510)
[![license](https://img.shields.io/github/license/linkedearth/FreqFun.svg)]()


# Solar and Orbital Forcing in Paleoclimate Records

*A reproducible, data-centric exploration using LinkedEarth Tools*


## Overview

This repository contains a collection of Jupyter notebooks that explore the relationship between **external climate forcings**—in particular **solar variability** and **orbital forcing**—and **paleoclimate variability** across a range of timescales, from the last two millennia to the late Pleistocene.

The notebooks are designed as a **narrative introduction to modern paleoclimate data analysis**, combining standardized data formats, programmatic data discovery, and transparent time-series analysis in a fully reproducible environment. These notebooks are meant to be used as both research and teaching resources.

## Scientific Motivation

Understanding how external forcings influence climate variability is a central question in paleoclimatology. However, detecting these signals in proxy records is challenging due to age uncertainty and irregular sampling, proxy-specific sensitivities, internal climate variability, and the risk of false positives in spectral analysis.

This project emphasizes **statistical rigor**, **careful significance testing**, and **physical interpretation**, rather than simple pattern matching.

---

## Core Questions

The notebooks address questions such as:

- Is there robust evidence for a solar influence on climate variability over the Common Era?
- What periodicities emerge in large paleoclimate temperature compilations?
- How consistent are spectral signals across archives and regions?
- How do orbital-scale forcings manifest in individual high-resolution records?
- What are the limitations of common spectral and coherence methods in paleoclimate applications?

---

## Notebook Structure

The notebooks are intended to be read roughly in the following order.

### 1. Solar forcing and Common Era temperature reconstructions

**`01-solar_climate2k.ipynb`**

Explores the relationship between solar forcing and temperature reconstructions over the last two millennia, including exploratory analysis, visual comparison, and discussion of coherence, significance, and interpretation.

---

### 2. Programmatic data discovery and spectral analysis at scale

**`02a-query_lipd_graph.ipynb`**

Introduces graph-based discovery of paleoclimate datasets using LiPDGraph and SPARQL, demonstrating how metadata-driven queries can be used to assemble analysis-ready datasets.

**`02b-spectral_analysis_temp12k.ipynb`**

Applies spectral analysis techniques to temperature records from the Temp12k database, focusing on methodological choices and their implications.

**`02c-spectral_analysis_peaks_temp12k.ipynb`**

Identifies and evaluates spectral peaks, with emphasis on red-noise benchmarks, uncertainty, and archive-dependent behavior.

---

### 3. Detailed exploration of individual records

**`03-EpicaDomeC_explore.ipynb`**

A deep dive into the EPICA Dome C ice core, exploring long-term variability, spectral structure, and interpretive challenges.

**`04-IODP339-U1385.ipynb`**

Analyzes orbital-scale variability in a marine sediment core, linking observed periodicities to orbital forcing while highlighting uncertainty and methodological caveats.

---

## Tools and Data Ecosystem

This project builds on the open paleoclimate software and data ecosystem, including:

- [LiPD (Linked Paleo Data)](https://lipd.net) for standardized data representation
- [LiPDGraph](https://linkedearth.graphdb.mint.isi.edu) for metadata querying using graph technologies
- [PyLiPD](https://pylipd.readthedocs.io/en/latest/) for opening and manipulating LiPD files. 
- [Pyleoclim](https://pyleoclim-util.readthedocs.io/en/latest/) for time-series, spectral, and coherence analysis
- Public paleoclimate data repositories such as [NOAA NCEI](https://www.ncei.noaa.gov/products/paleoclimatology) and [PANGAEA](https://www.pangaea.de)

All analyses are designed to be **transparent, inspectable, and reusable**.

---

## Intended Audience

This material is intended for:

- Graduate students learning paleoclimate data analysis
- Researchers transitioning to Python-based, reproducible workflows
- Instructors seeking worked examples of spectral analysis and forcing attribution
- Researchers interested in large-scale, metadata-driven paleoclimate synthesis

Some familiarity with time-series analysis and basic climate concepts is helpful, but the notebooks are written to be pedagogical and exploratory.

---

## Reproducibility and Reuse

- All analyses are performed in Jupyter notebooks
- Code and narrative are interleaved to support transparency
- The repository is suitable for use as a Jupyter Book
- Users are encouraged to adapt workflows to their own datasets

If you reuse this material, please cite the relevant datasets and software packages.

---

## Getting Started

To run the notebooks locally:

```bash
git clone <repo-url>
cd <repo>
conda env create -f environment.yml
conda activate <env-name>
jupyter lab
```

## License

All notebooks herein are provided under an [Apache 2.0](https://www.apache.org/licenses/LICENSE-2.0) license.

## Citation
We needn't tell you that making research tools accessible requires time and effort. If you find any of these resources useful and use them in your own research, please do us the kindness of one or more citations. Notebooks in this collection are registered on Zenodo, and associated with a digital object identifier (DOI).  A ready-to-use citation is provided on this GitHub repository in APA and BibTex (in the "About" section on the right panel, click on "Cite this repository"). If you use any of the software, please cite them as well. It will make us (and our sponsors) very happy to hear that these investments spawned more research.

## Acknowledgements

This material is based upon work supported by the National Science Foundation under Grant Number ICER-2126510. Any opinions, findings, and conclusions or recommendations expressed in this material are those of the investigators and do not necessarily reflect the views of the National Science Foundation.
