# datascripts
Collection of scripts / notebooks to reliably select datasets


## Current sources

* `data`: Some definition data used to query other datasets. These files are mostly static because they don't change often, but they are versioned just in case.
* `kinases-in-chembl`: Maps human kinases UniProt IDs (from [KinHub](http://kinhub.org/kinases.html)) to ChEMBL target IDs.
* `chembl-25`: Retrieve activities (IC50, Ki, Kd) of small compounds against human kinases in ChEMBL v25 (requires [local SQLite copy](ftp://ftp.ebi.ac.uk/pub/databases/chembl/ChEMBLdb/releases/chembl_25/)).
* `chembl-26`: Retrieve activities (IC50, Ki, Kd) of small compounds against human kinases in ChEMBL v26 (requires [local SQLite copy](ftp://ftp.ebi.ac.uk/pub/databases/chembl/ChEMBLdb/releases/chembl_26/)).
* `chembl-27`: Retrieve activities (IC50, Ki, Kd) of small compounds against human kinases in ChEMBL v27 (requires [local SQLite copy](ftp://ftp.ebi.ac.uk/pub/databases/chembl/ChEMBLdb/releases/chembl_27/)).

## Installation

Create a `conda` environment using the included environment file:

```
conda env create -f devtools/environment.yml
conda activate openkinome-datascripts
```