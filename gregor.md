## Gregor API

####  Explored by: 

`Ravi Mandla`,`Eric Ham`-`(Bioinformatics 201, Fall-2023, UCLA)`

---------

![img](img/gregor.png)

--------

### Description: 

GREGOR is a tool to test for the enrichment of variants associated with a phenotype within annotated epigenomic regions. It works by doing the following: 

1. Accounting for LD between variants and regions
2. Picking control variants matching the input variants by the number of variants in LD, MAF, and distance to the nearest gene

GREGOR can be downloaded from the [wiki](https://genome.sph.umich.edu/wiki/GREGOR), where further documentation can also be found. The original paper can also be found [here](https://doi.org/10.1093/bioinformatics/btv201).

### Tutorial: 

We created a tutorial to use GREGOR to test for enrichment between association statistics and genomic regions available UPDATE LINK TO GREGOR TUTORIAL [at this link](https://colab.research.google.com/drive/1iwNnEjuJbJ9pyQ9KG7inCQt1LQzlJxTQ?usp=sharing)

### Use cases: 

We present two cases focused on identifying enrichment between association results and genomic regions.

1. **Task**: Given the summary statistics from a GWAS for a specific trait, identify the cell or tissue types involved in the trait.
    * **Background**: To understand the biology underlying complex traits, we can see which cell types are likely involved in the association
    * **Goal**: Identify cell or tissue types underlying a GWAS
    * **Method**: Test for enrichment between index variants from a GWAS with epigenomic regions for different cell or tissue types. 
    * **Outcome**: P-value and size of the SNP intersection for each epigenomic dataset.
2. **Task**: Given the summary statistics from a GWAS for a specific trait, identify the cell or tissue types involved in the trait.
    * **Background**: To understand the biology underlying complex traits, we can see which cell types are likely involved in the association
    * **Goal**: Identify cell or tissue types underlying a GWAS
    * **Method**: Test for enrichment between index variants from a GWAS with epigenomic regions for different cell or tissue types. 
    * **Outcome**: P-value and size of the SNP intersection for each epigenomic dataset.
