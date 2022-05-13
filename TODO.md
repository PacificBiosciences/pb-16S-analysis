* See `https://github.com/benjjneb/dada2/issues/1164` for discussion on losing reads in CCS
* Setting minQ=0 and maxEE to 4 can rescue a lot of reads
  * minQ=0 and maxEE=2 is similar to minQ=3 and maxEE=2 in MSA1003
* Using lima to demux first instead of using DADA2 can give a lot more reads. Downside is
  that we have to modify the `run_dada_ccs.R` script in QIIME plugin.
* Cluster ASV into OTUs using `https://docs.qiime2.org/2022.2/plugins/available/vsearch/cluster-features-open-reference/` 
