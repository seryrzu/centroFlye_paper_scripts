# centroFlye paper scripts

This repository contains scripts to replicate results of centroFlye paper (see `Publications`).

## centroFlye version
[centroFlye repository](https://github.com/seryrzu/centroFlye/tree/cF_NatBiotech_paper_Xv0.8.3-6v0.1.3) is included as a submodule (note, the used branch: `cF_NatBiotech_paper_Xv0.8.3-6v0.1.3`).
Thus, please clone the repo with the following command

```
git clone --recurse-submodules git@github.com:seryrzu/centroFlye_paper_scripts.git
```

## Necessary data
Please, download necessary data from [ZENODO](http://doi.org/10.5281/zenodo.3897531) (latest version).
Note that the versions of assemblies that are described in the paper and are used here: cenX - v0.8.3, cen6 - v0.1.3.
Updated versions of these assemblies may be available in the future — they will be described in the [master branch of the centroFlye repository](https://github.com/seryrzu/centroFlye/).

Unzip data with command
```
tar -xvf ccentroFlye_data_cenXv0_8_3_cen6v0_1_3_20191224-updatedAndUplodaded_20200616.tgz
```

## Jupyter notebooks
The following notebooks (in directory `jupyters`) replicate the results in the paper.
Below we specify the section of the paper for each notebook.
+ `Appendix_analysis_structural_variations.ipynb` replicates `Appendix: Abnormal units in centroFlye cenX assembly`.
+ `Appendix_Benchmark_simulated_reads.ipynb` replicates `Appendix: Benchmarking centroFlye on simulated datasets`
+ `Appendix_cen6.ipynb` replicates `Appendix: Assembly of centromere on chromosome 6`
+ `Appendix_Deriving_accurate_consensus_HOR.ipynb` replicates `Appendix: Deriving accurate consensus HORs`
+ `Appendix_DXZ1BothOrient_Alu_NonunifCov.ipynb` replicates `Appendices`: `Analysis of reads with reported DXZ1 alignments to both strand orientations`, `Search for Alu insertions in cenX`, `Analyzing non-uniform read coverage of the T2T4 read-set`
+ `Appendix_Evolution.ipynb` replicates `Appendix: Variations in HORs provide insights into evolutionary history of cenX`
+ `Appendix_nonunique_kmers.ipynb` replicates `Analysis of frequencies of recruited k-mers in the centroFlye cenX assembly`
+ `Appendix_subsampling.ipynb` replicates `Appendix N: Effects of downsampling and read trimming on centromere assembly`.
+ `Classifying_centromeric_reads_into_prefix_internal_and_suffix_reads.ipynb` replicates `Methods: Classifying centromeric reads into prefix, internal, and suffix reads (Figure 2.3)`
+ `Constructing_the_distance_graph.ipynb` replicates `Methods: Identifying rare centromeric k-mers (Figure 2.4)` and `Methods: Constructing the distance graph (Figure 2.5)`
+ `Dataset.ipynb` replicates `Methods: Dataset`
+ `Identifying_rare_centromeric_k-mers.ipynb` replicates `Methods: Identifying rare centromeric k-mers (Figure 2.4)`
+ `Partitioning_centromeric_reads_into_units.ipynb` replicates `Methods: Partitioning centromeric reads into units (Figure 2.2)`
+ `Polishing_the_constructed_centromere_sequence.ipynb` replicates `Polishing the reconstructed centromere sequence (Figure 2.7)`
+ `Recruiting_centromeric_reads.ipynb` replicates `Recruiting centromeric reads (Figure 2.1)`
+ `Results_and_several_Appendices.ipynb` replicates `Results` and `Appendices`: `Analysis of centromeric reads that do not map to centroFlye assembly`, `Hanging index test`, and `Breakpoint test`.


## Publications
Bzikadze A.V., Pevzner P.A. centroFlye: Assembling Centromeres with Long Error-Prone Reads, 2020, _Nature Biotechnology, in press_
