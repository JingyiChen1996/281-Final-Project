# 281-Final-Project
![Data description](https://github.com/JingyiChen1996/281-Final-Project/blob/master/data%20description.png)


## Downstream analysis

**1. Finding ChIP-seq motifs**
using weeder: http://159.149.160.88/pscan_chip_dev/

same_peak_E2_weeder

![same_peak_E2_weeder](https://github.com/JingyiChen1996/281-Final-Project/blob/master/fig/ea0b1c9970358c19a1bf9cc5c2790ea.png)

same_peak_noE2_weeder

![same_peak_noE2_weeder](https://github.com/JingyiChen1996/281-Final-Project/blob/master/fig/f0d37ebb14aeacaa4535b300799f659.png)


Here only same_peak_E2 and same_peak_noE2 are put into weeder to find motifs, but one can use the PR peaks and TET2 peaks (GSMxxxxxx_summits) under two conditions to find PR/TET2 motifs as well.



**2. Finding enriched GO/Pathway**

ALL 6 putative genes files can be analyzed using David:
  1. what GO/pathways are enriched in the genes regulated by TET2 and PR together under E2 condition?
     use putative_E2_same_target_genes.csv

  2.what GO/pathways are enriched in the genes regulated by TET2 and PR together under no E2 condition?
    use putative_noE2_same_target_genes.csv
  
  3. what GO/pathways are enriched in the genes regulated by TET2 under E2 condition?
    use putative_TET2_E2_target_genes.csv
  
  4. what GO/pathways are enriched in the genes regulated by TET2 under no E2 condition?
    use putative_TET2_noE2_target_genes.csv
    
  5. what GO/pathways are enriched in the genes regulated by PR under E2 condition?
    use putative_PR_E2_target_genes.csv
  
  6. what GO/pathways are enriched in the genes regulated by PR under no E2 condition?
    use putative_PR_noE2_target_genes.csv
    
**3. Finding genes that are both regulated by PR+TET2 and are differentially expressed in two conditions.**

                              PR+TET2 under E2           PR_TET2 under no E2
      
       Up regulated in E2        20                             33
       
       
       Down regulated in E2      64                             67
       
       
  if wanted can further analysis the GO/pathway of these genes.  
