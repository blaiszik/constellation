---
layout: default
title: Home
nav_order: 1
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---

# The Constellation Data Repository
{: .fs-9 .no_toc }

## A Data Repository to Share AI- and HPC-enabled Generated for SARS-CoV-2 Drugs
{: .no_toc }

This repository is for sharing data used and models produced to generate leads for potential SARS-CoV-2 drugs. These data will be updated regularly as the collaboration produces new results. Shared data are located on the ALCF Petrel data store ([here](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2F)), from where they can be retrieved via Globus (**request access [here](<https://app.globus.org/groups/ebcae90a-60c9-11ea-a443-0a990c2810ad/about>)**)

## Table of contents
{: .no_toc }

* TOC
{:toc}

## Data Processing Pipeline
The data processing pipeline is used to compute different types of features and representations of billions of small molecules.  The pipeline first converts the SMILES representation for each molecule to the canonical SMILES form and removes duplicates. It then creates three different types of features: 1) molecular descriptors (using [Mordred](<https://github.com/mordred-descriptor/mordred));  2) molecular fingerprints that encode the structure of molecules; and 3) 2D images of the molecular structure.  These features are used as input to various machine learning and deep learning models that predict important characteristics including docking scores, toxicity, and more.

![](./assets/images/pipeline.png)

<!-- 
[Get started now](#getting-started){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 } [View it on GitHub](https://github.com/pmarsceill/just-the-docs){: .btn .fs-5 .mb-4 .mb-md-0 } -->

---

## Data Summary Table

Key | Full name | # Molecules | Details
----- | --- | --- | --- 
BDB | BindingDB | TBD | TBD
CAS | CAS COVID-19 Antiviral Candidate Compounds | TBD | [Link](https://www.cas.org/covid-19-antiviral-compounds-dataset)
DCL | DrugCentral | TBD | TBD
DBK | Drugbank | 9,679 | TBD
DUD | DUDE database of useful decoys | 101,337 | [Link](http://dude.docking.org)
E15 | 15.5M-molecule subset of ENA | TBD | TBD 
EDB | Enamine REAL subset | TBD | TBD
EMO | eMolecules | 22,318,616 | TBD 
ENA | Enamine REAL | TBD | TBD
FFI | Cure | TBD | TBD
G13 | GDB-13| 977,468,301 | TBD
G17 | GDB-17| 50,000,000 | TBD
HOP | Harvard Organic Photovoltaic Dataset | 350 | [Link](https://www.nature.com/articles/sdata201686)
L1K | L1000 | 10,148 | TBD
MOS | Moses | 1,936,963 | TBD
PCH | PubChem | 97,584,282 | TBD
QM9 | QM9 | 133,885 | TBD
REP | REP | 10,148 | TBD
SAV | Synthetically Accessible Virtual Inventory (SAVI) | 283,194,319 | [Link](https://cactus.nci.nih.gov/download/savi_download/)
SUR | SureChEML | 291,525,153 | [Link](https://surechembl.org/)
ZIN | ZINC15 | 1,475,876,222 | TBD

Notes:
* The numbers above need to be validated. Note that they may be less than what can be found at the source.
* These numbers do not account for de-duplication, within or between datasets.
* We may want to look at [MoleculeNet](http://moleculenet.ai/datasets-1)


Key | Canonical SMILES | Fingerprints | Descriptors | Images
----- | --- | --- | ---  | ---
E15 | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
G13 | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
G17 | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
HOP | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
L1K | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
MOS | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
PCH | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
QM9 | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
REP | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
SAV | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
SUR | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)
ZIN | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F) | [Link](https://app.globus.org/file-manager?origin_id=a386b552-6086-11ea-9688-0e56c063f437&origin_path=%2Fdata%2Fdescriptors%2FDrunkBank_descriptors%2F)



## Methodology

### Converting SMILES Canonical Form


### Generating Fingerprints


### Calculating Descriptors

# Contributing

# Acknowledgements

Data storage and computational support for this research project has been generously supported by the following resources.

## Petrel Data Service at the Argonne Leadership Computing Facility (ALCF)
{: .no_toc }
This research used resources of the Argonne Leadership Computing Facility, which is a DOE Office of Science User Facility supported under Contract DE-AC02-06CH11357.
[Petrel](https://press3.mcs.anl.gov/petrel/)

## Theta at the Argonne Leadership Computing Facility (ALCF)
{: .no_toc }
This research used resources of the Argonne Leadership Computing Facility, which is a DOE Office of Science User Facility supported under Contract DE-AC02-06CH11357.
[ALCF](https://www.alcf.anl.gov)


## Frontera at the Texas Advanced Computing Center (TACC)
{: .no_toc }
[TACC](https://www.tacc.utexas.edu)


## Comet at the San Diego Supercomputing Center (SDSC)
{: .no_toc }
[SDSC](https://www.sdsc.edu)

