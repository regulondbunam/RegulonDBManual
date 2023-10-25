#  Evidence Classification in RegulonDB 

Scientific knowledge advances incrementally. At any point, we base broad conclusions on assertions of varying degrees of confidence. RegulonDB classifies evidence supporting particular assertions essentially based on the methods used to generate them. We do so to make explicit the complex mixture of more or less well supported specific claims that support broader conclusions (Weiss et al., 2013) In RegulonDB version 11.1 we made several changes to the collection of evidence types. We made changes to the evidence codes to make them more informative and more precise since we indicate the corresponding method. We increased the number of high throughput evidence types. Finally, we updated the collection of combinations of independent methods that increase the confidence levels. The details can be found in the sections on additive evidence below.

### Evidence supporting knowledge as ’Weak’, ’Strong ’ or ’Confirmed ’.



- **Weak evidence**: Single evidence with more ambiguous conclusions, where alternative explanations, indirect effects, or potential false positives are prevalent, as well as computational predictions; for instance gel mobility shift assays with cell extracts or gene expression analysis.
- **Strong evidence**: Single evidence with direct physical interaction or solid genetic evidence with a low probability for alternative explanations; for instance, footprinting with purified protein or site mutation.
- **Confirmed**: is assigned, if objects are supported by at least two independent types of strong evidence with mutually excluding false positives. This approach is based essentially on the methods used to validate results and exclude alternative explanations in scientific research.



### Confidence is assigned in two stages:

- **In stage I**: we classify single evidence into weak or strong.
- **In stage II**: we define combinations of independent evidence in a process termed “additive evidence” (previously described as Cross-Validation in (Weiss et al., 2013), that enable multiple weak evidence types to support an object with a strong (S) confidence level, as well as multiple strong types to support the higher “confirmed (C)” level of an object.

#### Stage I. Classification of Individual Evidence Types

As mentioned before, in RegulonDB version 11.1 we made changes to the collection of evidence types; we changed the evidence codes so now they indicate the corresponding method ((for instance Transcription initiation mapping is now encoded as primer extension assay for transcription start site determination evidence or S1 nuclease protection assay evidence for transcription start site determination evidence ).
    

**Description**

Single evidence is classified into weak or strong evidence (see above), depending on the confidence level of the associated methodologies. 


1. **Promoters and transcription start sites (TSSs)**

Promoters are defined in bacteria by the DNA region specifically bound by RNA polymerase to initiate transcription.
A TSS is the precise first nucleotide that is transcribed, different methods identify promoters or TSSs. They are jointly classified here.

<table><thead><tr>  <th>1)confidence_level</th><th>2)evidence_name</th><th>3)evidence_code</th><th>4)evidence_category</th><th>5)evidence_group</th><th>6)object_type</th><th>
</th></tr></thead><tbody id="data-table">  <tr>    <td>S</td>    <td>Site mutation</td>    <td>EXP-IMP-SITE-MUTATION</td>    <td>Classical binding</td>    <td>1</td>    <td>Promoter;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>S</td>    <td>Transcription initiation mapping</td>    <td>EXP-IDA-TRANSCRIPTION-INIT-MAPPING</td>    <td>Classical experiment</td>    <td>15</td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td>S</td>    <td>RNA polymerase footprinting</td>    <td>EXP-IDA-RNA-POLYMERASE-FOOTPRINTING</td>    <td>Classical experiment</td>    <td>9</td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Traceable author statement to experimental support</td>    <td>EXP-TAS</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from mutant phenotype</td>    <td>EXP-IMP</td>    <td>Classical binding</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from direct assay</td>    <td>EXP-IDA</td>    <td>Classical binding</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from physical interaction</td>    <td>EXP-IPI</td>    <td>Classical experiment</td>    <td></td>    <td>Promoter;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from expression pattern</td>    <td>EXP-IEP</td>    <td>Classical expression</td>    <td>3</td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>High-throughput RNA-seq evidence</td>    <td>EXP-IEP-RNA-SEQ</td>    <td>High-throughput expression</td>    <td>3</td>    <td>Promoter;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred by computational analysis</td>    <td>COMP</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Human inference of promoter position</td>    <td>COMP-HINF-POSITIONAL-IDENTIFICATION</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Traceable author statement</td>    <td>AS-TAS</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred by curator</td>    <td>IC</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Automated inference based on sequence pattern discovery</td>    <td>COMP-AINF-PATTERN-DISCOVERY</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Author hypothesis</td>    <td>AS-HYPO</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Automated inference of promoter position</td>    <td>COMP-AINF-POSITIONAL-IDENTIFICATION</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred computationally without human oversight</td>    <td>COMP-AINF</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Non-traceable author statement</td>    <td>AS-NAS</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred by a human based on computational evidence</td>    <td>COMP-HINF</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>High-throughput transcription initiation mapping</td>    <td>EXP-IDA-HPT-TRANSCR-INIT-M-RACE-MAP</td>    <td>High-throughput protocol</td>    <td>10</td>    <td>Promoter</td>    <td></td>  </tr>  <tr>    <td></td>    <td>Primer extension assay for transcription start site determination</td>    <td>EXP-IDA-TRANSCRIPTION-INIT-MAPPING-PRIMER-EXTENSION-TSS</td>    <td></td>    <td></td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td></td>    <td>Northern blot for expression pattern analysis evidence</td>    <td>EXP-IEP-NORTHERN</td>    <td></td>    <td></td>    <td>Promoter;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Traceable author statement to experimental support</td>    <td>EXP-TAS</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from mutant phenotype</td>    <td>EXP-IMP</td>    <td>Classical binding</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from direct assay</td>    <td>EXP-IDA</td>    <td>Classical binding</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from physical interaction</td>    <td>EXP-IPI</td>    <td>Classical experiment</td>    <td></td>    <td>Promoter;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred from expression pattern</td>    <td>EXP-IEP</td>    <td>Classical expression</td>    <td>3</td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>High-throughput RNA-seq evidence</td>    <td>EXP-IEP-RNA-SEQ</td>    <td>High-throughput expression</td>    <td>3</td>    <td>Promoter;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred by computational analysis</td>    <td>COMP</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Human inference of promoter position</td>    <td>COMP-HINF-POSITIONAL-IDENTIFICATION</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Traceable author statement</td>    <td>AS-TAS</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred by curator</td>    <td>IC</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Automated inference based on sequence pattern discovery</td>    <td>COMP-AINF-PATTERN-DISCOVERY</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Author hypothesis</td>    <td>AS-HYPO</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Automated inference of promoter position</td>    <td>COMP-AINF-POSITIONAL-IDENTIFICATION</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred computationally without human oversight</td>    <td>COMP-AINF</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Non-traceable author statement</td>    <td>AS-NAS</td>    <td>non-experimental</td>    <td></td>    <td>Promoter;Transcription Units;Regulatory Interactions </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>Inferred by a human based on computational evidence</td>    <td>COMP-HINF</td>    <td>non-experimental</td>    <td>7</td>    <td>Promoter;Transcription Units;Regulatory Interactions;Transcription Factors </td>    <td>
</td>  </tr>  <tr>    <td></td>    <td>in vitro transcription reconstitution assay evidence</td>    <td>EXP-IDA-IN-VITRO-TRANSCRIPTION</td>    <td></td>    <td></td>    <td>Promoter </td>    <td>
</td>  </tr>  <tr>    <td>W</td>    <td>High-throughput transcription initiation mapping</td>    <td>EXP-IDA-HPT-TRANSCR-INIT-M-RACE-MAP</td>    <td>High-throughput protocol</td>    <td>10</td>    <td>Promoter</td>    <td></td>  </tr></tbody>
  </table>

2. **Regulatory Interactions**

A regulatory interaction is defined, depending on the type of evidence, as the transcription factor (TF)-regulated gene interaction (TF-gene), or more specifically as the TF-DNA binding site interaction.

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);border-radius:2px;" width="900" height="450" src="https://zs7yfm-3000.csb.app/tsv-ris" allowfullscreen></iframe>

3. **Transcription Factor**

Most dedicated TFs have usually two conformations, one with a non-covalent bound allosteric metabolite, or a covalent phosphorylation (holo conformation), and one as a free protein or multimer (the apo conformation). There are exceptions to this statement. We call functional conformation the one that is capable of binding to its specific binding sites and perform its activation or repression activity. For the sake of functional conformation evidence the experiments below have to be considered with and without effector. 
<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);border-radius:2px;" width="900" height="450" src="https://zs7yfm-3000.csb.app/tsv-TF" allowfullscreen></iframe>


4. **Transcription Units**

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);border-radius:2px;" width="900" height="450" src="https://zs7yfm-3000.csb.app/tsv-TU" allowfullscreen></iframe>




####  Stage II. Assignment of confidence level based on additive evidence types

Following the same logic described in ([Weiss et al., 2013](https://pubmed.ncbi.nlm.nih.gov/23327937/)) we integrate multiple evidence by combining independent types of evidence, with the intention to confirm individual objects and mutually exclude false positives. It follows the same principles of science as applied by wet-lab scientists, where data are confirmed by repetitions on the one hand, and by additional experimental strategies to exclude alternative explanations on the other. This approach allows us to combine classic methods from molecular biology and genomic high throughput (HT) methods.

Additive evidence (called "cross-validation" in previous releases of RegulonDB) requires that the combined methods are independent, that is, do not share major sources of false positives or common raw materials. In this version the evidence codes were assigned to an evidence group, different evidence groups correspond to independent methods. Evidence codes from the same evidence group cannot be combined to upgrade the object confidence level. Some evidence groups are shared among diverse object types, i.e. EXP-IMP-SITE-MUTATION is associated with regulatory interactions and also with promoters, while other classes are exclusive of an object type.

Objects that are supported by multiple types of independent weak (W) evidence are classified as strong evidence (S). A third confidence score "confirmed"(C) is assigned to objects that are supported by two types of independent strong evidence. In the table below are indicated the combinations of evidence groups that result in upgrade to strong or confirmed confidence level of an object. i.e. the combination (8/10/7) results in a confirmed confidence level; it happens when the object has at least one evidence code from the evidence groups 8, 10 and 7.

The downloadable datasets contain all the individual evidence types so users can either construct their own combinations or use the three confidence levels (W,S,C). 


1. **Promoters and transcription start sites (TSSs)**

| Additive Evidence Rule  | Evidences|
|:--      |:--       |
| **Confirmed Evidence** |    |
| Additive Evidence (1/9) |	1: (EXP-IMP-SITE-MUTATION) <br> 9: (EXP-IDA-RNA-POLYMERASE-FOOTPRINTING) |
| Additive Evidence (1/10/7) |	1: (EXP-IMP-SITE-MUTATION) <br> 10: (EXP-IDA-HPT-TRANSCR-INIT-M-RACE-MAP) <br> 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-AINF-POSITIONAL-IDENTIFICATION, COMP-HINF-POSITIONAL-IDENTIFICATION, COMP-HINF, COMP, COMP-AINF) |
| Additive Evidence (9/10/7) |	9: (EXP-IDA-RNA-POLYMERASE-FOOTPRINTING) <br> 10: (EXP-IDA-HPT-TRANSCR-INIT-M-RACE-MAP) <br> 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-AINF-POSITIONAL-IDENTIFICATION, COMP-HINF-POSITIONAL-IDENTIFICATION, COMP-HINF, COMP, COMP-AINF) |
| **Strong Evidence** | |
| Additive Evidence (10/7) | 10: (EXP-IDA-HPT-TRANSCR-INIT-M-RACE-MAP) <br> 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-AINF-POSITIONAL-IDENTIFICATION, COMP-HINF-POSITIONAL-IDENTIFICATION, COMP-HINF, COMP, COMP-AINF) |




2. **Regulatory interactions**

| Additive Evidence Rule  | Evidences|
|:--      |:--       |
| **Confirmed Evidence** 	| |
| Additive Evidence (1/2) | 1: (EXP-IMP-SITE-MUTATION) <br> 2: (EXP-IDA-BINDING-OF-PURIFIED-PROTEINS) |
| Additive Evidence (4/5/3/1) | 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 5: (EXP-GSELEX) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 1: (EXP-IMP-SITE-MUTATION) |
| Additive Evidence (7/4/3/1) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 1: (EXP-IMP-SITE-MUTATION) |
| Additive Evidence (7/5/3/1)  | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 5: (EXP-GSELEX) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 1: (EXP-IMP-SITE-MUTATION) |
| Additive Evidence(6/4/3/1) | 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 1: (EXP-IMP-SITE-MUTATION) |
|Additive Evidence (6/5/3/1) | 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 5: (EXP-GSELEX) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 1: (EXP-IMP-SITE-MUTATION) |
| Additive Evidence(7/6/3/1) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 1: (EXP-IMP-SITE-MUTATION) |
| Additive Evidence (4/5/3/2) | 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 5: (EXP-GSELEX) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 2: (EXP-IDA-BINDING-OF-PURIFIED-PROTEINS) |
| Additive Evidence (7/4/3/2) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 2: (EXP-IDA-BINDING-OF-PURIFIED-PROTEINS) | 
| Additive Evidence (7/5/3/2) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 5: (EXP-GSELEX) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 2: (EXP-IDA-BINDING-OF-PURIFIED-PROTEINS) |
| Additive Evidence (6/4/3/2) | 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 2: (EXP-IDA-BINDING-OF-PURIFIED-PROTEINS) |
| Additive Evidence (6/5/3/2) | 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 5: (EXP-GSELEX) <br>  3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 2: (EXP-IDA-BINDING-OF-PURIFIED-PROTEINS) |
| Additive Evidence(7/6/3/2) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) <br> 2: (EXP-IDA-BINDING-OF-PURIFIED-PROTEINS)  |
| **Strong Evidence** | |
| Additive Evidence(4/5/3) | 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 5: (EXP-GSELEX) <br>  3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) |
| Additive Evidence(7/4/3) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) |
| Additive Evidence(7/5/3) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 5: (EXP-GSELEX) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) |
| Additive Evidence (6/4/3) | 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 4: (EXP-CHIP-PCR-MANUAL, EXP-CHIP-CHIP-MANUAL, EXP-CHIP-EXO-MANUAL, EXP-CHIP-SEQ-MANUAL, EXP-CHIP-CHIP, EXP-CHIP-EXO, EXP-CHIP-SEQ) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) |
| Additive Evidence(6/5/3) | 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 5: (EXP-GSELEX) <br>  3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) |
| Additive Evidence(7/6/3) | 7: (COMP-HINF-SIMILAR-TO-CONSENSUS, COMP-AINF-PATTERN-DISCOVERY, COMP-AINF-SIMILAR-TO-CONSENSUS, COMP-HINF, COMP, COMP-AINF, COMP-HINF-PATTERN-DISCOVERY) <br> 6: (EXP-IDA-BINDING-OF-CELLULAR-EXTRACTS) <br> 3: (EXP-IEP-GENE-EXPRESSION-ANALYSIS, EXP-IEP, EXP-IEP-RNA-SEQ, EXP-IEP-MICROARRAY) |




3. **Transcription units**




