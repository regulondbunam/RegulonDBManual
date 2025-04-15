# Documentation of Standards and Ontologies Used in RegulonDB

This document outlines the community standards, ontologies, and controlled vocabularies adopted by **RegulonDB** to ensure metadata consistency, data interoperability, and alignment with FAIR principles.



## 1. Gene Ontology (GO)
RegulonDB integrates **Gene Ontology** annotations to describe:
- **Molecular Function**: e.g., ATP binding (GO:0005524), kinase activity  
- **Biological Process**: e.g., glycolate cycle, transcriptional regulation  
- **Cellular Component**: e.g., cytoplasm (GO:0005737)

Each gene product entry in RegulonDB includes a detailed list of GO terms, with links to GO databases. These annotations enable integration with resources such as UniProt and enhance semantic search and analysis.



## 2. Evidence Code Ontology (ECO)
All curated objects in RegulonDB are associated with a defined **evidence code**, following the ECO standard. Examples include:
- **EXP-IDA** (Inferred from Direct Assay)  
- **EXP-IPI** (Inferred from Physical Interaction)  
- **IC** (Inferred by Curator)  

These evidence types are displayed for each object, providing traceability and enabling users to assess the **confidence level** of the annotations.



## 3. Microbial Conditions Ontology (MCO)
For datasets derived from experimental evidence (e.g., ChIP-seq), metadata includes standardized conditions using the **Microbial Conditions Ontology**, such as:
- Organism: *Escherichia coli* K-12 MG1655  
- Medium: MOPS minimal medium + 0.2% glucose  
- Aeration: 95% N₂ / 5% CO₂  
- Temperature: 37°C  

This allows integration with GEO datasets (e.g., GSM1010219) and reproducibility of experimental context.



## 4. File and Format Standards
- **Sequence Formats**: FASTA and GenBank are available for all genes and transcription units.  
- **Tabular Downloads**: TSV and CSV formats are provided across gene, regulatory interaction, and network datasets.  
- **Data Dumps**: Available for Regulatory Interactions (RISet), Regulators (TFSet), and Network views.

---

## 5. External Identifiers and Cross-References
Each gene, product, or interaction object in RegulonDB is linked to external databases using persistent identifiers:
- **UniProt** (e.g., P76052)  
- **RefSeq** (e.g., NP_415853)  
- **EcoCyc**, **InterPro**, **Pfam**, **EcoliWiki**  
- **AlphaFold**, **PRIDE**, **ModBase**

These links support interoperability and citation tracking.



## 6. Tools and Visualization Standards
- **Cytoscape-compatible** network files for visualizing gene regulatory networks.  
- **Gensor Unit diagrams** to represent complex transcriptional regulatory cascades.  
- Downloads in standard graphical and JSON formats to support external analysis.



## 7. Confidence Classification System
All regulatory objects (e.g., interactions, operons) are assigned a **confidence level** (e.g., weak, strong, confirmed), based on the supporting evidence codes.


