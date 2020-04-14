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
BDB | The Binding Database | 1,813,538 | [Link](https://www.bindingdb.org/bind/index.jsp)
CAS | CAS COVID-19 Antiviral Candidate Compounds | 49,437 | [Link](https://www.cas.org/covid-19-antiviral-compounds-dataset)
DCL | DrugCentral Online Drug Compendium | 3,981 | [Link](http://drugcentral.org)
DBK | Drugbank | 9,678 | [Link](https://www.drugbank.ca)
DUD | DUDE database of useful decoys | 99,782 | [Link](http://dude.docking.org)
E15 | 15.5M-molecule subset of ENA | 15,547,091 | N/A
EDB | Enamine REAL subset | 310,782 | N/A
EMO | eMolecules | 25,946,988 | [Link](https://www.emolecules.com/info/products-data-downloads.html)
ENA | Enamine REAL Database | 1,211,723,723 | [Link](https://enamine.net/library-synthesis/real-compounds/real-database)
FFI | CureFFI | 1,497 | [Link](https://www.cureffi.org/2013/10/04/list-of-fda-approved-drugs-and-cns-drugs-with-smiles/)
G13 | GDB-13| 977,468,301 | [Link](http://gdb.unibe.ch/downloads/)
G17 | GDB-17-Set| 50,000,000 | [Link](http://gdb.unibe.ch/downloads/)
HOP | Harvard Organic Photovoltaic Dataset | 350 | [Link](https://www.nature.com/articles/sdata201686)
L1K | L1000 | 10,141 | [Link](http://www.lincsproject.org)
MOS | Molecular Sets (MOSES) | 1,936,962 | [Link](https://github.com/molecularsets/moses)
PCH | PubChem | 97,545,266 | [Link](https://www.ncbi.nlm.nih.gov/guide/data-software/)
QM9 | QM9 subset of GDB-17 | 133,885 | [Link](http://quantum-machine.org/datasets/)
REP | REP | 6,244 | TBD
SAV | Synthetically Accessible Virtual Inventory (SAVI) | 265,047,097 | [Link](https://cactus.nci.nih.gov/download/savi_download/)
SUR | SureChEML | 17,915,384 | [Link](https://surechembl.org/)
ZIN | ZINC15 | 1,225,804,829 | [Link](http://zinc15.docking.org)
    |        | **3,891,374,956** |

Notes:
* The numbers above may be less than what can be found at the source, due to conversion failures and/or version differences.
* These numbers do not account for de-duplication, within or between datasets.
* We may want to look at [MoleculeNet](http://moleculenet.ai/datasets-1)
* EDB needs a better description


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

