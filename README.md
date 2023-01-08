# WGCNA-Turorial

This is a tutorial of the weighted gene correlation network analysis (WGCNA) package from Dept. of Human Genetics, UC Los Angeles. 

WGCNA begins with the understanding that the information captured by microarray experiments is far richer than
a list of differentially expressed genes. Rather, microarray data are more completely represented by considering the
relationships between measured transcripts, which can be assessed by pair-wise correlations between gene expression
profiles. In most microarray data analyses, however, these relationships go essentially unexplored. WGCNA starts
from the level of thousands of genes, identifies clinically interesting gene modules, and finally uses intramodular
connectivity, gene significance (e.g. based on the correlation of a gene expression profile with a sample trait) to
identify key genes in the disease pathways for further validation. WGCNA alleviates the multiple testing problem
inherent in microarray data analysis. Instead of relating thousands of genes to a microarray sample trait, it focuses
on the relationship between a few (typically less than 10) modules and the sample trait. Toward this end, it calculates
the eigengene significance (correlation between sample trait and eigengene) and the corresponding p-value for each
module. The module definition does not make use of a priori defined gene sets. Instead, modules are constructed from
the expression data by using hierarchical clustering. Although it is advisable to relate the resulting modules to gene
ontology information to assess their biological plausibility, it is not required. Because the modules may correspond
to biological pathways, focusing the analysis on intramodular hub genes (or the module eigengenes) amounts to a
biologically motivated data reduction scheme. Because the expression profiles of intramodular hub genes are highly
correlated, typically dozens of candidate biomarkers result. Although these candidates are statistically equivalent,
they may differ in terms of biological plausibility or clinical utility. Gene ontology information can be useful for further
prioritizing intramodular hub genes.

![image](https://user-images.githubusercontent.com/89398186/211225324-8b958bcb-c625-4b62-8d8a-b262d1fd2bcf.png)

I. Network analysis of expression data: finding modules related to trait

![image](https://user-images.githubusercontent.com/89398186/211225354-ee75f2c8-94d4-4af8-b7b8-f8d59a0ca217.png)

II. Consensus analysis of expression data

![image](https://user-images.githubusercontent.com/89398186/211225379-39f7e7c6-b277-49ff-b568-2aab6a615d5b.png)

III. Analysis of simulated data

IV. Meta-analysis of several data sets
