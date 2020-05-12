# datascripts
Collection of scripts / notebooks to reliably select datasets


## Current sources

* `data`: Some definition data used to query other datasets. These files are mostly static because they don't change often.
* `kinases-in-chembl`: Maps human kinases UniProt IDs (from KinHub) to ChEMBL target IDs.
* `chembl-25`: Retrieve activities (IC50, Ki, Kd) of small compounds against human kinases in ChEMBL v25 (requires local SQL copy).
* `chembl-26`: Retrieve activities (IC50, Ki, Kd) of small compounds against human kinases in ChEMBL v26 (requires local SQL copy).

## Installation

Create a `conda` environment using the included environment file:

```
conda env create -f devtools/environment.yml
conda activate openkinome-datascripts
```