# GNF1 File Format - Definition and supported options

The GNF (General Network Format) format consists of one line per regulatory interaction, each containing 7 columns of data, 
plus optional track definition lines. The following documentation is based on the Version 1 specifications.


## Fields

The first line of a GNF1 file must be a comment that identifies the version, e.g.

```
##gnf-version 1
```

Fields must be tab-separated. Also, all but the final field in each feature line must contain a value; "empty" columns should be denoted with a '.'

1. **regulatorId**. Regulator Identifier
2. **regulatorName**. Regulator Name
3. **regulatedId**. Regulated entity Identifier
4. **regulatedName**. Regulated entity name
5. **function**. Regulatory function of the regulator on the regulated entity
6. **tfrsEvidence**. Evidence that supports the existence of the entity, interaction or other property.
7. **riEvidence** Evidence of the function of the Regulatory interaction (RI)
8. **additiveEvidence** Additive evidence is obtained from the relationship of 2 or more evidence that, when combined, generate a greater degree of confidence.
9. **confidence**. Object confidence level based on  its evidence (Values: Confirmed, Strong, Weak)

The regulator can represent regualtory genes, transcription factor, proteins, sRNAs, sigma factors. 


# [TF - gene Regulatory Network Interactions](http://regulondb.ccg.unam.mx/menu/download/datasets/files/network_tf_gene.txt)

> The tf-gene dataset is obtained from three types of interactions reported in scientific articles: a) regulatory interactions between tf and the promoters it regulates, 2) regulatory interactions between tf and transcriptional units without knowing the promoter, c) the interactions between the TF and the regulated genes, without knowing the promoter and if the regulated genes are part of a tu.
Columns:

1. **regulatorId** Transcription Factor (TF) identifier
2. **regulatorName** Transcription Factor (TF) Name
3. **regulatedId** Gene ID regulated by the TF (regulated gene)
4. **regulatedName** Gene regulated by the TF (regulated gene)
5. **function** Regulatory Function of the TF on the regulated gene (+ activator, - repressor, +- dual, ? unknown) 
6. **tfrsEvidence** Evidence that supports the existence of the TFRS [Evidence code | evidence confidence level | evidence name]
7. **riEvidence** Evidence of the function of the RI [Evidence code | evidence confidence level | evidence name]
8. **additiveEvidence** Additive Evidence of the RI [Evidence code | evidence confidence level | evidence name]
9. **confidence** RI confidence level based on its evidence (Values: Confirmed, Strong, Weak)


**Details**

- **additiveEvidence** 

An additive evidence is obtained from the relationship of 2 or more evidence that, when combined, generate a greater degree of confidence. [Evidence code | evidence confidence level | evidence name]



### [TF - TU Regulatory Network Interactions](http://regulondb.ccg.unam.mx/menu/download/datasets/files/network_tf_tu.txt)

> The TF-TU dataset dataset is obtained from .......

Columns:

1. **regulatorName** Transcription Factor (TF) Name
2. **regulatedName** Transcription Unit Name (regulated)
3. **function** Regulatory Function of the TF on the regulated gene (+ activator, - repressor, +- dual, ? unknown) 
4. **tfrsEvidence** Evidence that supports the existence of the TFRS [Evidence code | evidence confidence level | evidence name]
5. **confidence** RI confidence level based on its evidence (Values: Confirmed, Strong, Weak)


**Details**


### [Sigma - gene Network Interactions Sigma ](http://regulondb.ccg.unam.mx/menu/download/datasets/files/network_sigma_gene.txt)

> The sigma-gene dataset is obtained from .......

Columns:

1. **regulatorName** Sigma Factor name
2. **regulatedName** Gene regulated by the Sigma Factor (regulated gene)
3. **function** Regulatory Function of the TF on the regulated gene (+ activator, - repressor, +- dual, ? unknown) 
4. **tfrsEvidence** Evidence that supports the existence of the TFRS [Evidence code | evidence confidence level | evidence name]
5. **confidence** RI confidence level based on its evidence (Values: Confirmed, Strong, Weak)


**Details**



### [sRNA - gene Regulatory Network Interactions](http://regulondb.ccg.unam.mx/menu/download/datasets/files/sRNABindingSiteSet.txt)

> The sRNA-gene dataset is obtained from .......

Columns:

1. **regulatorId**.  Identifier assigned by RegulonDB to the small RNA interaction (temporal identifier)
2. **regulatorName**. Gene regulator related to small RNA
3. **regulatedId**. Gene regulated by the small RNA
4. **regulatedName**. Object regulated (Gene or Transcription Unit regulated by the small RNA)
5. **leftPosition**. sRNA binding site left end position in the genome
6. **rightPosition**. sRNA binding site right end position in the genome
7. **strand**. DNA strand of the regulated gene
8. **function**. Function (+ activation, - repression, +- dual, ? unknown)
9. **sequence**. sRNA binding site sequence
10. **mechanism**. Regulation Mechanism
11. **tfrsEvidence**. Evidence that supports the existence of the small RNA regulation
12. **confidence**. Evidence confidence level (Confirmed, Strong, Weak)


**Details**
