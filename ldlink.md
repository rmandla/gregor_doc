## LDlink API

####  Explored by: 

`Ravi Mandla`,`Eric Ham`-`(Bioinformatics 201, Fall-2023, UCLA)`

---------

![img](img/ldlink.png)

--------

### Description: 

LDlink is a an online database to identify variants in LD with an specified input variant within different populations of 1000G. There are several modules within LDlink with different
tasks, including:

1. LDproxy - Identify variants in LD with a specified variant
2. LDtrait - Test if a specified variant, or a variant in LD, has been identified as associated with a phenotype.
3. LDexpression - Test if a specified variant, or a variant in LD, has been identified as associated with gene expression.
4. etc...

A full list of all the modules available at LDlink can be found [here](https://ldlink.nih.gov/?tab=home). This NIH supported resource also provides API code to programmatically search
different modules for specific data. Instructions on getting access to this API and example use cases can be found [here](https://ldlink.nih.gov/?tab=apiaccess).

### Tutorial: 

We created a tutorial to use LDlink to download a list of variants in LD with a specified variant [at this link](https://colab.research.google.com/drive/1iwNnEjuJbJ9pyQ9KG7inCQt1LQzlJxTQ?usp=sharing)

### Use cases: 

1. **Task**: Given a list of variants identified in an eQTL, identify which are associated with a trait.
    * **Background**: A majority of variants associated with a trait are non-coding, raising the possibility they may be involved in gene regulation. 
    * **Goal**: Identify traits which have an overlap of associations with eQTL from a specific tissue.
    * **Method**: Pull all variants, or LD proxy variants, associated with an eQTL and a different set of traits. 
    * **Outcome**: Variant IDs and LD information, and the number of associations in both an eQTL and a specified set of traits.
