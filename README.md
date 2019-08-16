# centroFlye paper scripts

This repository contains scripts to replicate results of centroFlye paper (see `Publications`).

## centroFlye version
[centroFlye repository](https://github.com/seryrzu/centroFlye) is included as a submodule.
Thus, please clone the repo with the following command

```git clone --recurse-submodules git@github.com:seryrzu/centroFlye_paper_scripts.git```


## Necessary data
Please, download necessary data from [ZENODO](TODO) and put the results in `data` directory (TODO: add command).


## Jupyter notebooks
The following notebooks (in directory `jupyters`) replicate the results in the paper.
Below we specify the section of the paper for each notebook.
+ `Appendix_analysis_structural_variations.ipynb` replicates `Appendix: Abnormal units in centroFlye cenX assembly`.
+ `Appendix_Benchmark_simulated_reads.ipynb` replicates `Appendix: Benchmarking centroFlye on simulated datasets`
+ `Appendix_Deriving_accurate_consensus_HOR.ipynb` replicates `Appendix: Deriving accurate consensus HORs`
+ `Appendix_DXZ1BothOrient_Alu_NonunifCov.ipynb` replicates `Appendices`: `Analysis of reads with reported DXZ1 alignments to both strand orientations`, `Search for Alu insertions in cenX`, `Analyzing non-uniform read coverage of the T2T4 read-set`
+ `Appendix_Evolution.ipynb` replicates `Appendix: Variations in HORs provide insights into evolutionary history of cenX`
+ `Appendix_nonunique_kmers.ipynb` replicates `Analysis of frequencies of recruited k-mers in the centroFlye cenX assembly`
+ `Classifying_centromeric_reads_into_prefix_internal_and_suffix_reads.ipynb` replicates `Methods: Classifying centromeric reads into prefix, internal, and suffix reads (Figure 2.3)`
+ `Constructing_the_distance_graph.ipynb` replicates `Methods: Identifying rare centromeric k-mers (Figure 2.4)` and `Methods: Constructing the distance graph (Figure 2.5)`
+ `Dataset.ipynb` replicates `Methods: Dataset`
+ `Identifying_rare_centromeric_k-mers.ipynb` replicates `Methods: Identifying rare centromeric k-mers (Figure 2.4)`
+ `Partitioning_centromeric_reads_into_units.ipynb` replicates `Methods: Partitioning centromeric reads into units (Figure 2.2)`
+ `Polishing_the_constructed_centromere_sequence.ipynb` replicates `Polishing the reconstructed centromere sequence (Figure 2.7)`
+ `Recruiting_centromeric_reads.ipynb` replicates `Recruiting centromeric reads (Figure 2.1)`
+ `Results_and_several_Appendices.ipynb` replicates `Results` and `Appendices`: `Analysis of centromeric reads that do not map to centroFlye assembly`, `Hanging index test`, and `Breakpoint test`.


## Publications
Bzikadze A., Pevzner P.A. centroFlye: Assembling Centromeres with Long Error-Prone Reads, 2019, *bioRxiv* TODO add DOI
