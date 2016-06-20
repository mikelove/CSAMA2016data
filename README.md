# CSAMA2016data

Additional datasets for CSAMA2016

## Steps taken to prepare data:

### Schurch et al, 2016: Highly replicated yeast RNA-seq

* Went to https://github.com/bartongroup/profDGE48
* From `Preproccesed_data` dir, downloaded `Snf2_countdata.tar.gz`
  and `WT_countdata.tar.gz`.
* Use `tar -xvf` to decompress and extract files and move them
  into dirs called `Snf2` and `WT` in `inst/extdata`
* Download `exclude.lst` from `Bad_replicate_identification` dir.
* Move this to `inst/extdata/bad_replicate` dir.

### SECQ data subset

* Install Bioconductor package `seqc`.
* `agr <- ILM_refseq_gene_AGR`
* `save(agr, file="agr.rda", compress="xz")`

