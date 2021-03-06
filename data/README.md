# Data

This directory contains processed data generated from 16S and shotgun analysis, with the full OTU relative or rarefied absolute abundance table provided in `biom` format. The rest are provided in `csv` format, and were used in relavant part of analysis as described below.

### Contents

1.) [human_16S.sampleinfo.csv](human_16S.sampleinfo.csv)
<br>Metadata table consisting of patient samples, response groups, and RECIST scores.

2.) [human_16S.even13190.abs.sig.csv](human_16S.even13190.abs.sig.csv)
<br>Rarefied absolute abundance of 63 human OTUs differentially abundant between 16S NR and R groups (42 samples in total, pre-treatment). 

3.) [human_16S.even13190.rel.sig.csv](human_16S.even13190.rel.sig.csv)
<br>Rarefied relative abundance of 63 human OTUs differentially abundant between 16S NR and R groups (42 samples in total, pre-treatment). This table was generated by taking the rarefied absolute abundance table and divide by the even sequencing depth (13190 reads). This file is essentially table S2 in the manuscript.

4.) [human_16S.even13190.stats.sig.csv](human_16S.even13190.stats.sig.csv)
<br>Permutation test (`QIIME` v1.91 option `nonparametric_t_test`) stats of 63 human OTUs differentially abundant between 16S NR and R groups (42 samples in total, pre-treatment). This file is essentially table S4 in the manuscript.

5.) [human_16S.even13190.abs.full.biom](human_16S.even13190.abs.full.biom)
<br>Rarefied absolute abundance of full list of human OTUs assembled in 42 16S sequencing fecal samples. The `biom` format serves as the input for many tools. It can be converted to plain text format (e.g. tsv) using command `biom convert -i table.biom -o table.txt --to-tsv`

6.) [human_16S.even13190.rel.full.biom](human_16S.even13190.rel.full.biom)
<br>Rarefied relative abundance of full list of human OTUs assembled in 42 16S sequencing fecal samples. This table was generated by taking the rarefied absolute abundance table and divide by the even sequencing depth (13190 reads). 

7.) [human_16S_qPCR.csv](human_16S_qPCR.csv)
<br>qPCR abundance of 10 validated human OTUs, including 8 bacteria more abundant in R, and 2 bacteria more abundant in NR. This file is essentially table S5 in the manuscript.

8.) [human_shotgun.rel.full.csv](human_shotgun.rel.full.csv)
<br>Relative abundance of full list of species profiled in 39 metagenomic shotgun sequencing human fecal samples. 

9.) [human_joint_evidence.csv](human_joint_evidence.csv)
<br>The biomarker summary table consisting of 16S qPCR score, OTU ratio, somatic mutational load, PDL1 and PD1 gene expression, and CD8+ IHC cell density in tumor.

10.) [mouse_16S.sampleinfo.csv](mouse_16S.sampleinfo.csv)
<br>Metadata table consisting of colonized mice samples, mice gender, patient donor, response groups, and mouse tumor growth groups.

11.) [mouse_16S.even22560.abs.sig.csv](mouse_16S.even22560.abs.sig.csv)
<br>Rarefied absolute abundance of 519 mouse OTUs differentially abundant between slow and fast tumor growth group (91 samples in total, including TAC mice as control). 

12.) [mouse_16S.even22560.rel.sig.csv](mouse_16S.even22560.rel.sig.csv)
<br>Rarefied relative abundance of 519 mouse OTUs differentially abundant between human 16S NR and R groups (91 samples in total, including TAC mice as control). This table was generated by taking the rarefied absolute abundance table and divide by the even sequencing depth (22560 reads). 

13.) [mouse_16S.even22560.abs.full.biom](mouse_16S.even22560.abs.full.biom)
<br>Rarefied absolute abundance of full list of OTUs assembled in 91 16S sequencing mouse samples. 

14.) [mouse_16S.even22560.rel.full.biom](mouse_16S.even22560.rel.full.biom)
<br>Rarefied absolute abundance of full list of OTUs assembled in 91 16S sequencing mouse samples. This table was generated by taking the rarefied absolute abundance table and divide by the even sequencing depth (22560 reads). 


