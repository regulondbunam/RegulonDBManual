# **RegulonDB Search**


RegulonDB Search  
[Searching](#searching)  
&nbsp;&nbsp;&nbsp;&nbsp;[By term](#by-term)  
&nbsp;&nbsp;&nbsp;&nbsp;[Searching by Coexpression](#by-coexpression)  
&nbsp;&nbsp;&nbsp;&nbsp;[Gene](#by-gene)  
&nbsp;&nbsp;&nbsp;&nbsp;[Gensor Unit](#by-gu)  
&nbsp;&nbsp;&nbsp;&nbsp;[Growth Condition](#by-gc)  
&nbsp;&nbsp;&nbsp;&nbsp;[Operon](#by-operon)  
&nbsp;&nbsp;&nbsp;&nbsp;[Regulon](#by-regulon)  
&nbsp;&nbsp;&nbsp;&nbsp;[Sigmulon](#by-sigmulon)  
&nbsp;&nbsp;&nbsp;&nbsp;[sRNA](#by-srna)  
[Browsing](#browsing)  
&nbsp;&nbsp;&nbsp;&nbsp;[Coexpression Browser](#coexpression-browser)  
&nbsp;&nbsp;&nbsp;&nbsp;[Gensor Unit Groups](#gu-groups)  
&nbsp;&nbsp;&nbsp;&nbsp;[Microbial Condition Ontology Browser](#mco-browser)  
&nbsp;&nbsp;&nbsp;&nbsp;[TF-Matrix Browser](#tf-matrix-browser)  
&nbsp;&nbsp;&nbsp;&nbsp;[Transcription Factor Browser](#tf-browser)  
&nbsp;&nbsp;&nbsp;&nbsp;[Transcription Factor Family Browser](#tf-family-browser)  

 
## <a name="searching">Searching</a>


## <a name="by-term">By term</a>


### <a name="by-coexpression">Searching by Coexpression</a>

A list of genes (gene name), separated by space or commas, can be introduced.

 araA araB araD AraC _coexpression_

 soda, soxS, soxR _coexpression_

RegulonDB uses ElasticSearch as a full-text search engine.


### <a name="by-gene">Gene</a>

You can use gene name, synonyms, identifiers, gene product, and GOs with the gene keyword. To get the complete list of the genes use only the keyword. 

araC _gene_

arabinose AND transporter AND _gene_

transcriptional regulator _gene_

b0012 _gene_

_gene_


### <a name="by-gu">Gensor Unit</a>

You can use the gensor unit name, the gensor unit identifier or the reaction name, with the gensor unit or gu keyword. To get the complete list of gensor units use only the keyword. 

araC _gensor unit_

PurR-hypoxanthine _gu_

_gensor unit_


### <a name="by-gc">Growth Condition</a>

You can use the condition identifier, the control, experimental and global condition with the growth condition keyword. To get the complete list of conditions use only the keyword. 

heat shock _growth condition_

glucose _growth condition_

_growth condition_


### <a name="by-operon">Operon</a>

You can use operon identifier, operon name, synonyms, transcription unit name, promoter name, promoter sequence with the operon keyword. To get the complete list of operons use only the keyword. 

lactose _operon_

metJ _operon_

glnALG _transcription unit_

_operon_


### <a name="by-regulon">Regulon</a>

You can use regulon identifier, regulon name, synonyms, transcription factor name, effector name, conformation of TFs with the operon keyword. To get the complete list of regulons use only the keyword, and you will get a table with the regulons and useful statistics. 

CRP _regulon_

Arabinose _regulon_

TyrR-tyrosine _regulon_

transcription AND factor AND repressor _regulon_

_regulon_


### <a name="by-sigmulon">Sigmulon</a>

You can use sigma name, sigma gene name and synonyms, with the sigmulon keyword. To get the complete list of sigmas use only the keyword. 

sigma19 _sigmulon_

rpoD _sigmulon_

_sigmulon_


### <a name="by-srna">sRNA</a>

You can use sRNA name, product name and synonyms, with the sRNA or small RNA keywords. To get the complete list of sRNA use only the keyword. 

micF _sRNA_

omrB _small RNA_

_sRNA_


## <a name="browsing">Browsing</a>


### <a name="coexpression-browser">Coexpression Browser</a>


### <a name="gu-groups">Gensor Unit Groups</a>

Access to each of the Gensor Unit (GUs) curated to date, here grouped either on the transduction mechanism or to the signal that initiates a flux of regulated processes.


### <a name="mco-browser">Microbial Condition Ontology Browser</a>


### <a name="tf-matrix-browser">TF-Matrix Browser</a>


### <a name="tf-browser">Transcription Factor Browser</a> 


### <a name="tf-family-browser">Transcription Factor Family Browser</a>
