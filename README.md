# centroFlye paper scripts

This repository contains scripts to replicate results of the centroFlye paper in Nature Biotechnology, 2020 (see `Publications`).

## centroFlye version
[centroFlye repository](https://github.com/seryrzu/centroFlye/tree/cF_NatBiotech_paper_Xv0.8.3-6v0.1.3) is included as a submodule (note, the used branch: `cF_NatBiotech_paper_Xv0.8.3-6v0.1.3`).
Thus, please, clone the repo with the following command

```
git clone --recurse-submodules git@github.com:seryrzu/centroFlye_paper_scripts.git
```

## Necessary data
Please, download necessary data from [ZENODO](http://doi.org/10.5281/zenodo.3897531) (latest version) and place the archive `centroFlye_data_cenXv0_8_3_cen6v0_1_3_20191224-uploaded20200407.tar.gz` in the root of the repo.
Note that the versions of assemblies that are described in the paper and are used here: cenX - v0.8.3, cen6 - v0.1.3.
Updated assemblies may be available in the future — they will be described in the [master branch of the centroFlye repository](https://github.com/seryrzu/centroFlye/).

Extract the data collection with the following command
```
tar -xvf centroFlye_data_cenXv0_8_3_cen6v0_1_3_20191224-updatedAndUplodaded_20200616.tgz
```
All information will be extracted in the `data` directory.

## Jupyter notebooks
The following notebooks (in directory `jupyters`) replicate the results in the paper.
Below we specify the section of the paper for each notebook.
+ `01-Results-cenX_assembly-dataset.ipynb` replicates `Results: cenX assembly, dataset description`
+ `02-Results_SuppNote2_4.ipynb` replicates `Results` (comparison of T2T and centroFlye assemblies) and `Supp. notes`: `4: Analysis of centromeric reads that do not map to centroFlye assembly`, `2: Hanging index test and Breakpoint test`
+ `03-Results_CentromereEvolutionInsights.ipynb` replicates `Results: Variations in HORs provide insights into centromere evolution`
+ `04-Methods_Recruiting_centromeric_reads.ipynb` replicates `Methods: Recruiting centromeric reads (Figure 1.1)`
+ `05-Methods_Partitioning_centromeric_reads_into_units.ipynb` replicates `Methods: Partitioning centromeric reads into units (Figure 1.2)`
+ `06-Methods_Classifying_centromeric_reads_into_prefix_internal_and_suffix_reads.ipynb` replicates `Methods: Classifying centromeric reads (Figure 1.3)`
+ `07-Methods_Identifying_rare_centromeric_k-mers.ipynb` replicates `Methods: Identifying rare centromeric k-mers (Figure 1.4)`
+ `08-Methods_Constructing_the_distance_graph.ipynb` replicates `Methods: Constructing the distance graph (Figure 1.5)`
+ `09-Methods_Polishing_the_constructed_centromere_sequence.ipynb` replicates `Methods: Polishing the reconstructed centromere sequence (Figure 1.7)`
+ `10-Methods_cen6.ipynb` replicates `Methods: Assembly of cen6, Recruitment of centromeric reads from cen6, Transforming reads into monoreads, Error correction of monoreads, Constructing iterative de Bruijn graph of monoreads, Assembling monocentromere by scaffolding, Translating monocentromere to the nucleotide alphabet`
+ `11-SuppNote1_Benchmarking_centroFlye_on_simulated_dataset.ipynb` replicates `Supplementary Note 1: Benchmarking centroFlye on simulated datasets`
+ `12-SuppNote3_Abnormal_units_in_centroFlye_cenX_assembly.ipynb` replicates `Supplementary Note 2: Abnormal units in centroFlye cenX assembly`
+ `13-SuppNote4_DXZ1BothOrient_Alu_NonunifCov.ipynb` replicates parts of `Supplementary Note 4. Analysis of centromeric reads that do not map to centroFlye assembly` (also see jupyter #2)
+ `14-SuppNote5_Deriving_accurate_consensus_HOR.ipynb` replicates `Supplementary Note 5: Deriving accurate consensus HORs`
+ `15-SuppNote6-Effects_of_downsampling.ipynb` replicates `Supplementary Note 6. Assembly of centromere on chromosome 6: Effects of downsampling and read trimming on cen6 assembly`
+ `16-SuppFigure1-Frequencies_of_the_recruited_19-mers_in_the_centroFlye_cenX_assembly.ipynb` replicates `Supplementary Figure 1: Frequencies of the recruited 19-mers in the centroFlye cenX assembly`

## Figures in the paper -> Jupyter notebook number
| # Figure | # Jupyter notebook |
| --- | --- |
| 1 | Manual |
| 2 | Manual |
| 3a | 07 |
| 3b | 09 |
| 3cde | 02 |
| 3d | 02 |
| 3e | 02 |
| 4abcd | 02 |
| 5 | 02 |
| 6 | 02 |
| S2.1 | 02 |
| S2.2 | 02 |
| S3.1 | 12 |
| S3.2 | 12, `data/abnormal_units` |
| S3.3 | 12, `data/abnormal_12_mers` |
| S3.4 | Manual |
| S4.1 | 02 |
| S4.2 | Can be reproduced with [gepard](http://cube.univie.ac.at/gepard), `data/centroFlye_results/centromeric_reads/centromeric_reads.fasta`|
| S5.1 | Can be reproduced with [gepard](http://cube.univie.ac.at/gepard) `data/DXZ1/DXZ1_rc.fasta`|
| S5.2 | 14 |
| S6.1 | 10, `data/cen6_hor_graph` |
| S6.2 left | cen6 assembly (main algorithm): left saved* in `data/centroFlyeMono_results_cen6/centroFlyeMono_cen6/idb/db_k400.dot`.     pdf can be generated with `dot -Tpdf db_k400.dot -o db_k400.pdf` |
| S6.2 right | Manual from S6.2 |
| S6.3 | 10, `data/centroFlyeMono_results_cen6/tandemQUAST_report/report` |
| S6.4 | 15 |
| S6.5 | 15, `data/subsampling` |
| SF1 | 16 |
| SF2 | 13 |
| SF3,4 | 03 |
| SF5 | 03 + Manual |


## Publications
Bzikadze A.V., Pevzner P.A. centroFlye: Assembling Centromeres with Long Error-Prone Reads, 2020, _Nature Biotechnology, in press_
