# RIF1 File Format - Definition and supported options

The RIF1 (Regulatory Interaction Format) format consists of one line per regulatory interaction, each containing # columns of data, 
plus optional track definition lines. The following documentation is based on the Version 1 specifications.


## Format

The first line of a RIF1 file must be a comment that identifies the version, e.g.

```
##rif-version 1
```

The columns of the file are:

1. **tfid**. Transcription Factor (TF) identifier assigned by RegulonDB
2. **tfName**. TF name
3. **cnfName**. TF active conformation name
5. **tfrs**. Transcription Factor regulatory site (TFRS) identifier assigned by RegulonDB
6. **tfrsLeft**. TFRS left end position in the genome
7. **tfrsright**. TFRS right end position in the genome
8. **strand**. DNA strand where the  TFRS is located
9. **riId**. Regulatory interaction (RI) identifier assigned by RegulonDB
10. **tuId**. Transcription unit id regulated by the TF
11. **tuName**. Transcription unit name regulated by the TF
12. **function**. Gene expression effect caused by the TF bound to the  TFRS (+ activation, - repression, +- dual, ? unknown) (TF function)
13. **pmName**. Promoter name
14. **distToPm**. Center position of TFRS, relative to the Transcription Start Site
15. **tfrsSeq**. TFRS sequence (upper case)
16. **distTo1Gene**. Distance from center position of TFRS to the  first gene
17. **tfrsEvidence**. Evidence that supports the existence of the TFRS [evidence code, evidence type: W weak, S strong, C confirmed, evidence name]
18. **riEvidence**. Evidence that supports the RI function [evidence code, evidence type: W weak, S strong, C confirmed, evidence name]
19. **addEvidence**. Additive Evidence [Evidence code | evidence confidence level | evidence name]
20. **confidence**. RI confidence level (Values: Confirmed, Strong, Weak)
21. **riEvTech**. Evidence related to the type of  technology  used to determine the RI function
22. **tfrsEvTech**. Evidence related to the type of  technology  used to determine the TFRS



Fields must be tab-separated. Also, all but the final field in each feature line must contain a value; "empty" columns should be denoted with a '.'

The data file displays the columns description as comments in the head of the file, also a line wirh the name of the columns are included:

```
(1) riId. Regulatory interaction (RI) identifier assigned by RegulonDB
# (2) riType. Regulatory interaction type [tf-promoter, tf-tu, tf-gene]
# (3) tfid. Transcription Factor (TF) identifier assigned by RegulonDB
# (4) tfName. TF name
# (5) cnfName. TF active conformation name
# (6) tfrsID. Transcription Factor regulatory site (TFRS) identifier assigned by RegulonDB
# (7) tfrsLeft. TFRS left end position in the genome
# (8) tfrsright. TFRS right end position in the genome
# (9) strand. DNA strand where the TFRS is located
# (10) tfrsSeq. TFRS sequence (upper case)
# (11) function. Gene expression effect caused by the TF bound to the TFRS (+ activation, - repression, +- dual, ? unknown) (TF function)
# (12) distToPm. Center position of TFRS, relative to the Transcription Start Site
# (13) PromoterID. Promoter Identifier assigned by RegulonDB
# (14) pmName. Promoter name
# (15) distTo1Gene. Distance from center position of TFRS to the first gene
# (16) targetName. Transcription unit or gene (id,name) regulated by the TF
# (17) tfrsEvidence. Evidence that supports the existence of the TFRS [evidence code, evidence type: W weak, S strong, C confirmed, evidence name]
# (18) riEvidence. Evidence that supports the RI function [evidence code, evidence type: W weak, S strong, C confirmed, evidence name]
# (19) addEvidence. Additive Evidence [Evidence code | evidence confidence level | evidence name]
# (20) confidence. RI confidence level (Values: Confirmed, Strong, Weak)
# (21) tfrsEvTech. Evidence related to the type of technology used to determine the TFRS
# (22) riEvTech. Evidence related to the type of technology used to determine the RI function





# (1) tfid. Transcription Factor (TF) identifier assigned by RegulonDB
# (2) tfName. TF name
# (3) cnfName. TF conformation name
# (4) tfrs. Transcription Factor regulatory site (TFRS) identifier assigned by RegulonDB
# (5) tfrsLeft. TFRS left end position in the genome
# (6) tfrsright. TFRS right end position in the genome
# (7) strand. DNA strand where the  TFRS is located
# (8) riId. Regulatory interaction (RI) identifier assigned by RegulonDB
# (9) tuId. Transcription unit id regulated by the TF
# (10) tuName. Transcription unit name regulated by the TF
# (11) function. Gene expression effect caused by the TF bound to the  TFRS (+ activation, - repression, +- dual, ? unknown) (TF function)
# (12) pmName. Promoter name
# (13) distToPm. Center position of TFRS, relative to the Transcription Start Site
# (14) tfrsSeq. TFRS sequence (upper case)
# (15) distTo1Gene. Distance from center position of TFRS to the  first gene
# (16) tfrsEvidence. Evidence that supports the existence of the TFRS [evidence code, evidence type: W weak, S strong, C confirmed, evidence name]
# (17) riEvidence. Evidence that supports the RI function [evidence code, evidence type: W weak, S strong, C confirmed, evidence name]
# (18) addEvidence. Additive Evidence [Evidence code | evidence confidence level | evidence name]
# (19) confidence. RI confidence level (Values: Confirmed, Strong, Weak)
# (20) riEvTech. Evidence related to the type of  technology  used to determine the RI function
# (21) tfrsEvTech. Evidence related to the type of  technology  used to determine the TFRS
1)tfid  2)tfName  3)cnfName 4)tfrs  5)tfrsLeft  6)tfrsright 7)strand  8)riId  9)tuId  10)tuName 11)function 12)pmName 13)distToPm 14)tfrsSeq  15)distTo1Gene  16)tfrsEvidence 17)riEvidence 18)addEvidence  19)confidence 20)riEvTech 21)tfrsEvTech
```


### Column Details

16.  Evidencias del TFRS - site
17.  Evidencias de la funcion -ri PERO SIN LAS CROSS VALIDATION -- where 
18.  Son las evidencias CROSS VALIDATION exclusivamente de la RI
19. Evidencias de Site + RI -- determinar el confidence level
